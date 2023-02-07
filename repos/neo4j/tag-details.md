<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.17`](#neo4j4417)
-	[`neo4j:4.4.17-community`](#neo4j4417-community)
-	[`neo4j:4.4.17-enterprise`](#neo4j4417-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.4`](#neo4j54)
-	[`neo4j:5.4-enterprise`](#neo4j54-enterprise)
-	[`neo4j:5.4.0`](#neo4j540)
-	[`neo4j:5.4.0-community`](#neo4j540-community)
-	[`neo4j:5.4.0-enterprise`](#neo4j540-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:475876f081b3f56495edbaf50101b55f66ba7bd5b03ccd9c9e739ab6914f18cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:cf6e7b3ad620936702da10eaf84db24ed8c86bd0d8c298fc0d4369f339bb465e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366781190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f8ee7c77d2acfc94390788a25f9cb09171da812f9b272431be2b8bfb14d83e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:09:02 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:51:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 14:51:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 14:51:23 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 14:51:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:51:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:51:35 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 14:51:35 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 14:51:35 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 14:51:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:51:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e30efc225d57cd9e62995f1d0420aa7db3d1ee71af748e8f579251b162ca44`  
		Last Modified: Sat, 04 Feb 2023 14:22:08 GMT  
		Size: 198.5 MB (198475569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd4843d60a840f0a38dd0e445138a436318f3a9ed1209c041501ad0484404`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec415156d42901e9a163f82367076bc04fe102400f63aabf71d74d3f99e5a1d`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 8.2 KB (8168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abb88de7055a2d656e736c2f4952ecc842613817050da51026ece59c1cb7c4`  
		Last Modified: Sat, 04 Feb 2023 14:53:12 GMT  
		Size: 136.9 MB (136896677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:354f525aa3bb446643ee8dcd04a39be94026317a775ecde42ce9dd2799a9bfc8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362050989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74762a2a5b533e3c3d2ff0d66133a6904381119cf44f04fec3da91881e01ab19`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:45:37 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 08:45:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 08:45:40 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 08:45:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:45:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 08:45:56 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 08:45:56 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 08:45:56 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 08:45:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:45:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6cab391fa4078e01d740a8b8f1dd48285df4066fdd71923d0588beb66395ce`  
		Last Modified: Sat, 04 Feb 2023 08:47:42 GMT  
		Size: 195.2 MB (195240323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ae35235a80a830ea46876b6c5d5cdc749dfd6d108125c8fb22af3793962ac5`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f85d3543b833cdef6bc64b78d8b66a066f52f4ad48b2a177d52262c13d3579`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589c2e60be8266b7f69230ac400b2652a3e237f655420ac131655c6a44c10ec3`  
		Last Modified: Sat, 04 Feb 2023 08:47:36 GMT  
		Size: 136.8 MB (136753816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:475876f081b3f56495edbaf50101b55f66ba7bd5b03ccd9c9e739ab6914f18cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:cf6e7b3ad620936702da10eaf84db24ed8c86bd0d8c298fc0d4369f339bb465e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366781190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f8ee7c77d2acfc94390788a25f9cb09171da812f9b272431be2b8bfb14d83e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:09:02 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:51:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 14:51:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 14:51:23 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 14:51:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:51:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:51:35 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 14:51:35 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 14:51:35 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 14:51:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:51:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e30efc225d57cd9e62995f1d0420aa7db3d1ee71af748e8f579251b162ca44`  
		Last Modified: Sat, 04 Feb 2023 14:22:08 GMT  
		Size: 198.5 MB (198475569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd4843d60a840f0a38dd0e445138a436318f3a9ed1209c041501ad0484404`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec415156d42901e9a163f82367076bc04fe102400f63aabf71d74d3f99e5a1d`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 8.2 KB (8168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abb88de7055a2d656e736c2f4952ecc842613817050da51026ece59c1cb7c4`  
		Last Modified: Sat, 04 Feb 2023 14:53:12 GMT  
		Size: 136.9 MB (136896677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:354f525aa3bb446643ee8dcd04a39be94026317a775ecde42ce9dd2799a9bfc8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362050989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74762a2a5b533e3c3d2ff0d66133a6904381119cf44f04fec3da91881e01ab19`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:45:37 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 08:45:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 08:45:40 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 08:45:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:45:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 08:45:56 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 08:45:56 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 08:45:56 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 08:45:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:45:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6cab391fa4078e01d740a8b8f1dd48285df4066fdd71923d0588beb66395ce`  
		Last Modified: Sat, 04 Feb 2023 08:47:42 GMT  
		Size: 195.2 MB (195240323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ae35235a80a830ea46876b6c5d5cdc749dfd6d108125c8fb22af3793962ac5`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f85d3543b833cdef6bc64b78d8b66a066f52f4ad48b2a177d52262c13d3579`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589c2e60be8266b7f69230ac400b2652a3e237f655420ac131655c6a44c10ec3`  
		Last Modified: Sat, 04 Feb 2023 08:47:36 GMT  
		Size: 136.8 MB (136753816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:5d44b6ccc35d14d27466e799b4e52446e92229c302ae73a1650d1b9f8dfc39ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b2fcea8c7dc86f2b4b9d4dbc47c1d1dfa2fe285a34d068b2e8e534b37516d366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463116081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca2de4a4a878df936e54c307beba30c125c824f545199735a22cde37068bf31`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:09:02 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:51:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4dc791d8b779f7006ef18672fae7b61cb05761df6e7f603ab5a4a1664e06bb41 NEO4J_TARBALL=neo4j-enterprise-4.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 14:51:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 14:51:40 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 14:51:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:51:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:51:55 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 14:51:55 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 14:51:55 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 14:51:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:51:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e30efc225d57cd9e62995f1d0420aa7db3d1ee71af748e8f579251b162ca44`  
		Last Modified: Sat, 04 Feb 2023 14:22:08 GMT  
		Size: 198.5 MB (198475569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfdf3e1ad6d598ca8de93be823cc105ff7542af0a259233931326d678b9083e`  
		Last Modified: Sat, 04 Feb 2023 14:53:24 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463b8338bd19057055a2903f5da250ee1c5b5f4ac9782bd8fa9fb70e92e20e5e`  
		Last Modified: Sat, 04 Feb 2023 14:53:24 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f666e88da889221d22f146b7e7ba1f8eda9191cb591af82b14a51d4275fe683`  
		Last Modified: Sat, 04 Feb 2023 14:53:36 GMT  
		Size: 233.2 MB (233231554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f9527658bc4ca1bbca815fd66f7a3e3d2e8fad6dedb853f0764c6a87725a9dc0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458387846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c9a2c4eab0849a72c260becce3b14ac7eaa22748a2ca03a8b1b3fe8f8f9d940`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:45:37 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:46:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4dc791d8b779f7006ef18672fae7b61cb05761df6e7f603ab5a4a1664e06bb41 NEO4J_TARBALL=neo4j-enterprise-4.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:46:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 08:46:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 08:46:02 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 08:46:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:46:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 08:46:15 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 08:46:15 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 08:46:16 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 08:46:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:46:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6cab391fa4078e01d740a8b8f1dd48285df4066fdd71923d0588beb66395ce`  
		Last Modified: Sat, 04 Feb 2023 08:47:42 GMT  
		Size: 195.2 MB (195240323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3da774ddc3575a0e4c198252f272b4e4ecf8244f22bf6f56ad316a91299fec`  
		Last Modified: Sat, 04 Feb 2023 08:47:54 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52ae38aa6d96b7b55e2ed139c6106e731a461d1fb1a9cd024fd5d1f01b49318`  
		Last Modified: Sat, 04 Feb 2023 08:47:55 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10533d9817bc40a187bec47251da299dba2840c65f744758bd8fef172f8e32f1`  
		Last Modified: Sat, 04 Feb 2023 08:48:04 GMT  
		Size: 233.1 MB (233090674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.17`

```console
$ docker pull neo4j@sha256:475876f081b3f56495edbaf50101b55f66ba7bd5b03ccd9c9e739ab6914f18cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.17` - linux; amd64

```console
$ docker pull neo4j@sha256:cf6e7b3ad620936702da10eaf84db24ed8c86bd0d8c298fc0d4369f339bb465e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366781190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f8ee7c77d2acfc94390788a25f9cb09171da812f9b272431be2b8bfb14d83e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:09:02 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:51:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 14:51:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 14:51:23 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 14:51:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:51:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:51:35 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 14:51:35 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 14:51:35 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 14:51:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:51:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e30efc225d57cd9e62995f1d0420aa7db3d1ee71af748e8f579251b162ca44`  
		Last Modified: Sat, 04 Feb 2023 14:22:08 GMT  
		Size: 198.5 MB (198475569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd4843d60a840f0a38dd0e445138a436318f3a9ed1209c041501ad0484404`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec415156d42901e9a163f82367076bc04fe102400f63aabf71d74d3f99e5a1d`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 8.2 KB (8168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abb88de7055a2d656e736c2f4952ecc842613817050da51026ece59c1cb7c4`  
		Last Modified: Sat, 04 Feb 2023 14:53:12 GMT  
		Size: 136.9 MB (136896677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.17` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:354f525aa3bb446643ee8dcd04a39be94026317a775ecde42ce9dd2799a9bfc8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362050989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74762a2a5b533e3c3d2ff0d66133a6904381119cf44f04fec3da91881e01ab19`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:45:37 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 08:45:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 08:45:40 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 08:45:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:45:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 08:45:56 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 08:45:56 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 08:45:56 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 08:45:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:45:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6cab391fa4078e01d740a8b8f1dd48285df4066fdd71923d0588beb66395ce`  
		Last Modified: Sat, 04 Feb 2023 08:47:42 GMT  
		Size: 195.2 MB (195240323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ae35235a80a830ea46876b6c5d5cdc749dfd6d108125c8fb22af3793962ac5`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f85d3543b833cdef6bc64b78d8b66a066f52f4ad48b2a177d52262c13d3579`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589c2e60be8266b7f69230ac400b2652a3e237f655420ac131655c6a44c10ec3`  
		Last Modified: Sat, 04 Feb 2023 08:47:36 GMT  
		Size: 136.8 MB (136753816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.17-community`

```console
$ docker pull neo4j@sha256:475876f081b3f56495edbaf50101b55f66ba7bd5b03ccd9c9e739ab6914f18cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.17-community` - linux; amd64

```console
$ docker pull neo4j@sha256:cf6e7b3ad620936702da10eaf84db24ed8c86bd0d8c298fc0d4369f339bb465e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366781190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f8ee7c77d2acfc94390788a25f9cb09171da812f9b272431be2b8bfb14d83e`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:09:02 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:51:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:22 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 14:51:23 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 14:51:23 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 14:51:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:51:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:51:35 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 14:51:35 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 14:51:35 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 14:51:36 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:51:36 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e30efc225d57cd9e62995f1d0420aa7db3d1ee71af748e8f579251b162ca44`  
		Last Modified: Sat, 04 Feb 2023 14:22:08 GMT  
		Size: 198.5 MB (198475569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd4843d60a840f0a38dd0e445138a436318f3a9ed1209c041501ad0484404`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec415156d42901e9a163f82367076bc04fe102400f63aabf71d74d3f99e5a1d`  
		Last Modified: Sat, 04 Feb 2023 14:53:05 GMT  
		Size: 8.2 KB (8168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abb88de7055a2d656e736c2f4952ecc842613817050da51026ece59c1cb7c4`  
		Last Modified: Sat, 04 Feb 2023 14:53:12 GMT  
		Size: 136.9 MB (136896677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.17-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:354f525aa3bb446643ee8dcd04a39be94026317a775ecde42ce9dd2799a9bfc8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362050989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74762a2a5b533e3c3d2ff0d66133a6904381119cf44f04fec3da91881e01ab19`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:45:37 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 08:45:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 08:45:40 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 08:45:55 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:45:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 08:45:56 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 08:45:56 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 08:45:56 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 08:45:56 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:45:56 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6cab391fa4078e01d740a8b8f1dd48285df4066fdd71923d0588beb66395ce`  
		Last Modified: Sat, 04 Feb 2023 08:47:42 GMT  
		Size: 195.2 MB (195240323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ae35235a80a830ea46876b6c5d5cdc749dfd6d108125c8fb22af3793962ac5`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f85d3543b833cdef6bc64b78d8b66a066f52f4ad48b2a177d52262c13d3579`  
		Last Modified: Sat, 04 Feb 2023 08:47:30 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589c2e60be8266b7f69230ac400b2652a3e237f655420ac131655c6a44c10ec3`  
		Last Modified: Sat, 04 Feb 2023 08:47:36 GMT  
		Size: 136.8 MB (136753816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.17-enterprise`

```console
$ docker pull neo4j@sha256:5d44b6ccc35d14d27466e799b4e52446e92229c302ae73a1650d1b9f8dfc39ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.17-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b2fcea8c7dc86f2b4b9d4dbc47c1d1dfa2fe285a34d068b2e8e534b37516d366
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463116081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca2de4a4a878df936e54c307beba30c125c824f545199735a22cde37068bf31`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:06:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 14:09:02 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Sat, 04 Feb 2023 14:51:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4dc791d8b779f7006ef18672fae7b61cb05761df6e7f603ab5a4a1664e06bb41 NEO4J_TARBALL=neo4j-enterprise-4.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 14:51:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 14:51:40 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 14:51:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:51:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 14:51:55 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 14:51:55 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 14:51:55 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 14:51:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 14:51:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e30efc225d57cd9e62995f1d0420aa7db3d1ee71af748e8f579251b162ca44`  
		Last Modified: Sat, 04 Feb 2023 14:22:08 GMT  
		Size: 198.5 MB (198475569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfdf3e1ad6d598ca8de93be823cc105ff7542af0a259233931326d678b9083e`  
		Last Modified: Sat, 04 Feb 2023 14:53:24 GMT  
		Size: 3.9 KB (3867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463b8338bd19057055a2903f5da250ee1c5b5f4ac9782bd8fa9fb70e92e20e5e`  
		Last Modified: Sat, 04 Feb 2023 14:53:24 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f666e88da889221d22f146b7e7ba1f8eda9191cb591af82b14a51d4275fe683`  
		Last Modified: Sat, 04 Feb 2023 14:53:36 GMT  
		Size: 233.2 MB (233231554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.17-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:f9527658bc4ca1bbca815fd66f7a3e3d2e8fad6dedb853f0764c6a87725a9dc0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458387846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c9a2c4eab0849a72c260becce3b14ac7eaa22748a2ca03a8b1b3fe8f8f9d940`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:44:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 04 Feb 2023 08:45:37 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Sat, 04 Feb 2023 08:46:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4dc791d8b779f7006ef18672fae7b61cb05761df6e7f603ab5a4a1664e06bb41 NEO4J_TARBALL=neo4j-enterprise-4.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:46:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
# Sat, 04 Feb 2023 08:46:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 04 Feb 2023 08:46:02 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Sat, 04 Feb 2023 08:46:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:46:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 08:46:15 GMT
WORKDIR /var/lib/neo4j
# Sat, 04 Feb 2023 08:46:15 GMT
VOLUME [/data /logs]
# Sat, 04 Feb 2023 08:46:16 GMT
EXPOSE 7473 7474 7687
# Sat, 04 Feb 2023 08:46:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 08:46:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6cab391fa4078e01d740a8b8f1dd48285df4066fdd71923d0588beb66395ce`  
		Last Modified: Sat, 04 Feb 2023 08:47:42 GMT  
		Size: 195.2 MB (195240323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3da774ddc3575a0e4c198252f272b4e4ecf8244f22bf6f56ad316a91299fec`  
		Last Modified: Sat, 04 Feb 2023 08:47:54 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52ae38aa6d96b7b55e2ed139c6106e731a461d1fb1a9cd024fd5d1f01b49318`  
		Last Modified: Sat, 04 Feb 2023 08:47:55 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10533d9817bc40a187bec47251da299dba2840c65f744758bd8fef172f8e32f1`  
		Last Modified: Sat, 04 Feb 2023 08:48:04 GMT  
		Size: 233.1 MB (233090674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

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

### `neo4j:5` - linux; arm64 variant v8

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

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:d56261532787dab7c5ac4bb71841a67b4a045148e8f519b0411dff006c4d4b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:5d2ae397d11cd4b910af7bc34de4dbd7eea04d6c2c5dea83b7ad5d3d3044f460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a06a85cdd4f3f78c4199adda23ed151c8ddf2b081ce9d0698da56be8815ec1`
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
# Sat, 04 Feb 2023 14:51:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 14:51:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:26:43 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:26:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:26:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:26:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:26:58 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:26:58 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:26:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:26:58 GMT
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
	-	`sha256:9f1cba5f1490d525243831a75eaa3ea517c7653be91862a25ff7f9b551f375ff`  
		Last Modified: Sat, 04 Feb 2023 14:52:42 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac28bfe5fd4906f041a818562271c889ed82315d1ebba0b9f560e2c8b027b2`  
		Last Modified: Tue, 07 Feb 2023 20:27:50 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9766f0fc6876367ca4beb47a4bd63f79ca596cd7bcc963a0dae8f13823e54c`  
		Last Modified: Tue, 07 Feb 2023 20:28:00 GMT  
		Size: 211.4 MB (211383765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:36642e0ff1ba719407631a61a49cd9d75ce36e0e13740ad2d299d9ff69495151
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355c0481e05053f7e2bc84ba42a76d14153c0d1d00468f87df6b0a8b6636f86e`
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
# Sat, 04 Feb 2023 08:45:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 08:45:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:45:04 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:45:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:45:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:45:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:45:17 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:45:17 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:45:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:45:17 GMT
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
	-	`sha256:2e7464a747e9f0e18f88a7ff3ada695d5e288adcb35f574fe0d62fac196f815e`  
		Last Modified: Sat, 04 Feb 2023 08:47:09 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41990a3fa67f63be0d6a2f8d69e0e57015192d55a636bdc3c9e954b9fe6d00a`  
		Last Modified: Tue, 07 Feb 2023 20:46:08 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3eab990376b02be41886b0f8d118c3c743474f82b8f834a81d089d126b2a13`  
		Last Modified: Tue, 07 Feb 2023 20:46:17 GMT  
		Size: 211.2 MB (211241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4` - linux; amd64

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

### `neo4j:5.4` - linux; arm64 variant v8

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

## `neo4j:5.4-enterprise`

```console
$ docker pull neo4j@sha256:d56261532787dab7c5ac4bb71841a67b4a045148e8f519b0411dff006c4d4b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:5d2ae397d11cd4b910af7bc34de4dbd7eea04d6c2c5dea83b7ad5d3d3044f460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a06a85cdd4f3f78c4199adda23ed151c8ddf2b081ce9d0698da56be8815ec1`
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
# Sat, 04 Feb 2023 14:51:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 14:51:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:26:43 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:26:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:26:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:26:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:26:58 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:26:58 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:26:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:26:58 GMT
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
	-	`sha256:9f1cba5f1490d525243831a75eaa3ea517c7653be91862a25ff7f9b551f375ff`  
		Last Modified: Sat, 04 Feb 2023 14:52:42 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac28bfe5fd4906f041a818562271c889ed82315d1ebba0b9f560e2c8b027b2`  
		Last Modified: Tue, 07 Feb 2023 20:27:50 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9766f0fc6876367ca4beb47a4bd63f79ca596cd7bcc963a0dae8f13823e54c`  
		Last Modified: Tue, 07 Feb 2023 20:28:00 GMT  
		Size: 211.4 MB (211383765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:36642e0ff1ba719407631a61a49cd9d75ce36e0e13740ad2d299d9ff69495151
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355c0481e05053f7e2bc84ba42a76d14153c0d1d00468f87df6b0a8b6636f86e`
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
# Sat, 04 Feb 2023 08:45:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 08:45:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:45:04 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:45:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:45:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:45:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:45:17 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:45:17 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:45:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:45:17 GMT
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
	-	`sha256:2e7464a747e9f0e18f88a7ff3ada695d5e288adcb35f574fe0d62fac196f815e`  
		Last Modified: Sat, 04 Feb 2023 08:47:09 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41990a3fa67f63be0d6a2f8d69e0e57015192d55a636bdc3c9e954b9fe6d00a`  
		Last Modified: Tue, 07 Feb 2023 20:46:08 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3eab990376b02be41886b0f8d118c3c743474f82b8f834a81d089d126b2a13`  
		Last Modified: Tue, 07 Feb 2023 20:46:17 GMT  
		Size: 211.2 MB (211241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.4.0`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4.0` - linux; amd64

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

### `neo4j:5.4.0` - linux; arm64 variant v8

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

## `neo4j:5.4.0-community`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4.0-community` - linux; amd64

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

### `neo4j:5.4.0-community` - linux; arm64 variant v8

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

## `neo4j:5.4.0-enterprise`

```console
$ docker pull neo4j@sha256:d56261532787dab7c5ac4bb71841a67b4a045148e8f519b0411dff006c4d4b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.4.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:5d2ae397d11cd4b910af7bc34de4dbd7eea04d6c2c5dea83b7ad5d3d3044f460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a06a85cdd4f3f78c4199adda23ed151c8ddf2b081ce9d0698da56be8815ec1`
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
# Sat, 04 Feb 2023 14:51:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 14:51:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:26:43 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:26:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:26:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:26:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:26:58 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:26:58 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:26:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:26:58 GMT
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
	-	`sha256:9f1cba5f1490d525243831a75eaa3ea517c7653be91862a25ff7f9b551f375ff`  
		Last Modified: Sat, 04 Feb 2023 14:52:42 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac28bfe5fd4906f041a818562271c889ed82315d1ebba0b9f560e2c8b027b2`  
		Last Modified: Tue, 07 Feb 2023 20:27:50 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9766f0fc6876367ca4beb47a4bd63f79ca596cd7bcc963a0dae8f13823e54c`  
		Last Modified: Tue, 07 Feb 2023 20:28:00 GMT  
		Size: 211.4 MB (211383765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.4.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:36642e0ff1ba719407631a61a49cd9d75ce36e0e13740ad2d299d9ff69495151
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355c0481e05053f7e2bc84ba42a76d14153c0d1d00468f87df6b0a8b6636f86e`
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
# Sat, 04 Feb 2023 08:45:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 08:45:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:45:04 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:45:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:45:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:45:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:45:17 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:45:17 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:45:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:45:17 GMT
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
	-	`sha256:2e7464a747e9f0e18f88a7ff3ada695d5e288adcb35f574fe0d62fac196f815e`  
		Last Modified: Sat, 04 Feb 2023 08:47:09 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41990a3fa67f63be0d6a2f8d69e0e57015192d55a636bdc3c9e954b9fe6d00a`  
		Last Modified: Tue, 07 Feb 2023 20:46:08 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3eab990376b02be41886b0f8d118c3c743474f82b8f834a81d089d126b2a13`  
		Last Modified: Tue, 07 Feb 2023 20:46:17 GMT  
		Size: 211.2 MB (211241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

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

### `neo4j:community` - linux; arm64 variant v8

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

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:d56261532787dab7c5ac4bb71841a67b4a045148e8f519b0411dff006c4d4b06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:5d2ae397d11cd4b910af7bc34de4dbd7eea04d6c2c5dea83b7ad5d3d3044f460
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **435.2 MB (435231178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a06a85cdd4f3f78c4199adda23ed151c8ddf2b081ce9d0698da56be8815ec1`
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
# Sat, 04 Feb 2023 14:51:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 14:51:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 14:51:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:26:43 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:26:57 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:26:57 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:26:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:26:58 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:26:58 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:26:58 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:26:58 GMT
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
	-	`sha256:9f1cba5f1490d525243831a75eaa3ea517c7653be91862a25ff7f9b551f375ff`  
		Last Modified: Sat, 04 Feb 2023 14:52:42 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac28bfe5fd4906f041a818562271c889ed82315d1ebba0b9f560e2c8b027b2`  
		Last Modified: Tue, 07 Feb 2023 20:27:50 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9766f0fc6876367ca4beb47a4bd63f79ca596cd7bcc963a0dae8f13823e54c`  
		Last Modified: Tue, 07 Feb 2023 20:28:00 GMT  
		Size: 211.4 MB (211383765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:36642e0ff1ba719407631a61a49cd9d75ce36e0e13740ad2d299d9ff69495151
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.6 MB (432558572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355c0481e05053f7e2bc84ba42a76d14153c0d1d00468f87df6b0a8b6636f86e`
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
# Sat, 04 Feb 2023 08:45:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=732518510f1ee501fc6398a2fa22fb7bf970cbae47a7c5a94425258ac204fa48 NEO4J_TARBALL=neo4j-enterprise-5.4.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 04 Feb 2023 08:45:09 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
# Sat, 04 Feb 2023 08:45:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 07 Feb 2023 20:45:04 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Tue, 07 Feb 2023 20:45:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.4.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Feb 2023 20:45:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Feb 2023 20:45:17 GMT
WORKDIR /var/lib/neo4j
# Tue, 07 Feb 2023 20:45:17 GMT
VOLUME [/data /logs]
# Tue, 07 Feb 2023 20:45:17 GMT
EXPOSE 7473 7474 7687
# Tue, 07 Feb 2023 20:45:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 07 Feb 2023 20:45:17 GMT
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
	-	`sha256:2e7464a747e9f0e18f88a7ff3ada695d5e288adcb35f574fe0d62fac196f815e`  
		Last Modified: Sat, 04 Feb 2023 08:47:09 GMT  
		Size: 3.9 KB (3884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41990a3fa67f63be0d6a2f8d69e0e57015192d55a636bdc3c9e954b9fe6d00a`  
		Last Modified: Tue, 07 Feb 2023 20:46:08 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3eab990376b02be41886b0f8d118c3c743474f82b8f834a81d089d126b2a13`  
		Last Modified: Tue, 07 Feb 2023 20:46:17 GMT  
		Size: 211.2 MB (211241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:b99ccc63b8b900a7c5fee373bdb4e5b22e9865326928e0502733004bcc7f9678
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

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

### `neo4j:latest` - linux; arm64 variant v8

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
