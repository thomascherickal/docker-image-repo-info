<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.18`](#neo4j4418)
-	[`neo4j:4.4.18-community`](#neo4j4418-community)
-	[`neo4j:4.4.18-enterprise`](#neo4j4418-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.5`](#neo4j55)
-	[`neo4j:5.5-enterprise`](#neo4j55-enterprise)
-	[`neo4j:5.5.0`](#neo4j550)
-	[`neo4j:5.5.0-community`](#neo4j550-community)
-	[`neo4j:5.5.0-enterprise`](#neo4j550-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:6cefb732a03904dc604262c0768a67f8f5bd8c655055b8375af6b0e49d20ed1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:49420f700211821aafc8fe36f93f42c2d1a06550b173bbb8b40b228a9d85f6d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c376c2df22bca82454206679dfe66192798c2d69efee778333fa3093bd2e57`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Fri, 24 Feb 2023 23:20:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Feb 2023 23:20:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Fri, 24 Feb 2023 23:20:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Feb 2023 23:20:08 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Fri, 24 Feb 2023 23:20:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Feb 2023 23:20:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Feb 2023 23:20:26 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Feb 2023 23:20:26 GMT
VOLUME [/data /logs]
# Fri, 24 Feb 2023 23:20:26 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Feb 2023 23:20:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:20:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f0aa56bd87b7901051196bb1b7620f1ff34dc92263f0d184df0a08d7aeb82c`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b60a999bdf32267c36abeded1e6cd14311a682ab7f25f380a25af3f018c7d1`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f5e9ca57723073c75a95f8c7a46fa320974a0943f5207c7e3c2e4036d68ab`  
		Last Modified: Fri, 24 Feb 2023 23:21:22 GMT  
		Size: 136.9 MB (136902167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:002cacd59f121b62b476015d9e5ccc2eaba34211159156648656eff82b28a9c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362068760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ea78b6727ebbd43a5cc469cc9d9d2825d5d8c9ad48a7ec3ee8548dda1164c3f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:21:30 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 10:04:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 09 Feb 2023 10:04:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Thu, 09 Feb 2023 10:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 09 Feb 2023 10:04:52 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Thu, 09 Feb 2023 10:05:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:05:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:05:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 09 Feb 2023 10:05:08 GMT
VOLUME [/data /logs]
# Thu, 09 Feb 2023 10:05:08 GMT
EXPOSE 7473 7474 7687
# Thu, 09 Feb 2023 10:05:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:05:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf483a916e651ca447c4add0da489b56284ef3ab648f7c4b8b28762f912a1e`  
		Last Modified: Thu, 09 Feb 2023 09:32:44 GMT  
		Size: 195.2 MB (195240411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01438cdba11b6d21a13104549ee0b8ba44748efc074d67731a68667192a381d`  
		Last Modified: Thu, 09 Feb 2023 10:06:33 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba0b44d8962a0fd1acba8a42e2c7bdc4619dcc348d3df60eed3bf424123768e`  
		Last Modified: Thu, 09 Feb 2023 10:06:33 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fef6f883040e0802fc4e22e2ffa23d6beb8f1b184bb4a64d62f87cb6f6d95c`  
		Last Modified: Thu, 09 Feb 2023 10:06:39 GMT  
		Size: 136.8 MB (136753782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:6cefb732a03904dc604262c0768a67f8f5bd8c655055b8375af6b0e49d20ed1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:49420f700211821aafc8fe36f93f42c2d1a06550b173bbb8b40b228a9d85f6d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c376c2df22bca82454206679dfe66192798c2d69efee778333fa3093bd2e57`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Fri, 24 Feb 2023 23:20:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Feb 2023 23:20:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Fri, 24 Feb 2023 23:20:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Feb 2023 23:20:08 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Fri, 24 Feb 2023 23:20:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Feb 2023 23:20:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Feb 2023 23:20:26 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Feb 2023 23:20:26 GMT
VOLUME [/data /logs]
# Fri, 24 Feb 2023 23:20:26 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Feb 2023 23:20:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:20:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f0aa56bd87b7901051196bb1b7620f1ff34dc92263f0d184df0a08d7aeb82c`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b60a999bdf32267c36abeded1e6cd14311a682ab7f25f380a25af3f018c7d1`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f5e9ca57723073c75a95f8c7a46fa320974a0943f5207c7e3c2e4036d68ab`  
		Last Modified: Fri, 24 Feb 2023 23:21:22 GMT  
		Size: 136.9 MB (136902167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:002cacd59f121b62b476015d9e5ccc2eaba34211159156648656eff82b28a9c7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362068760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ea78b6727ebbd43a5cc469cc9d9d2825d5d8c9ad48a7ec3ee8548dda1164c3f`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:21:30 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 10:04:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=d87379c14a90ec9790ff081438688025b36bda8bb10a85e85fbeff09274c2801 NEO4J_TARBALL=neo4j-community-4.4.17-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 09 Feb 2023 10:04:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
# Thu, 09 Feb 2023 10:04:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 09 Feb 2023 10:04:52 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Thu, 09 Feb 2023 10:05:07 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:05:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:05:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 09 Feb 2023 10:05:08 GMT
VOLUME [/data /logs]
# Thu, 09 Feb 2023 10:05:08 GMT
EXPOSE 7473 7474 7687
# Thu, 09 Feb 2023 10:05:08 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:05:08 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf483a916e651ca447c4add0da489b56284ef3ab648f7c4b8b28762f912a1e`  
		Last Modified: Thu, 09 Feb 2023 09:32:44 GMT  
		Size: 195.2 MB (195240411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01438cdba11b6d21a13104549ee0b8ba44748efc074d67731a68667192a381d`  
		Last Modified: Thu, 09 Feb 2023 10:06:33 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba0b44d8962a0fd1acba8a42e2c7bdc4619dcc348d3df60eed3bf424123768e`  
		Last Modified: Thu, 09 Feb 2023 10:06:33 GMT  
		Size: 8.2 KB (8171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fef6f883040e0802fc4e22e2ffa23d6beb8f1b184bb4a64d62f87cb6f6d95c`  
		Last Modified: Thu, 09 Feb 2023 10:06:39 GMT  
		Size: 136.8 MB (136753782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:ba61c9c66a13a4f705c8f0e4fe6dcb389f6360f7e3bff57b379457f4e25b2006
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:d5ec99c2e2d4b6e188b0ad16c878bbad5259359221ecb643b5017ea29a2b4ba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463205192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f02cea60ed2f60134725833b5cdac895d65993ec3af416f921de51fae504d49`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Fri, 24 Feb 2023 23:20:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=79d7283199af9e4830dbf79ff36b98d8851b342724edd741785b91bad33f7d73 NEO4J_TARBALL=neo4j-enterprise-4.4.18-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Feb 2023 23:20:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
# Fri, 24 Feb 2023 23:20:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Feb 2023 23:20:33 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Fri, 24 Feb 2023 23:20:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Feb 2023 23:20:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Feb 2023 23:20:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Feb 2023 23:20:48 GMT
VOLUME [/data /logs]
# Fri, 24 Feb 2023 23:20:48 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Feb 2023 23:20:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:20:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778e2f222523e1c1dd355bd0939e03e50dab1dacec2c2336abd79ea32cf39de`  
		Last Modified: Fri, 24 Feb 2023 23:21:35 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9da32a54015c12a92955440d5595420e145a7f8b283ae9da164d93a53eee447`  
		Last Modified: Fri, 24 Feb 2023 23:21:35 GMT  
		Size: 8.4 KB (8424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d90ec3e928ac12a1eedeb96f5a82e3b3808471eb723ea7591de5301dfaf217f`  
		Last Modified: Fri, 24 Feb 2023 23:21:46 GMT  
		Size: 233.3 MB (233305675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:789e87168e3eca2b577b3d40655cbcf190c4b901dd2d640f83ddb74053a7b0f3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.4 MB (458405635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb4c150ef507a7dbc758af5cf65cab0dd451a4bccce63f01bcd29dd2c8a5614`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:21:30 GMT
COPY dir:b661686bf8d434588756c45f2ef6e7f314f32f753cf180ef8fb45397388f098c in /opt/java/openjdk 
# Thu, 09 Feb 2023 10:05:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4dc791d8b779f7006ef18672fae7b61cb05761df6e7f603ab5a4a1664e06bb41 NEO4J_TARBALL=neo4j-enterprise-4.4.17-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 09 Feb 2023 10:05:11 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
# Thu, 09 Feb 2023 10:05:12 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 09 Feb 2023 10:05:12 GMT
COPY multi:bcdd0bea98c64e6ecaf1a248e9edc31123c2bb38e4099e0a080dab2e2d5a11a8 in /startup/ 
# Thu, 09 Feb 2023 10:05:24 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.17-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:05:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Feb 2023 10:05:26 GMT
WORKDIR /var/lib/neo4j
# Thu, 09 Feb 2023 10:05:26 GMT
VOLUME [/data /logs]
# Thu, 09 Feb 2023 10:05:26 GMT
EXPOSE 7473 7474 7687
# Thu, 09 Feb 2023 10:05:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 10:05:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0acf483a916e651ca447c4add0da489b56284ef3ab648f7c4b8b28762f912a1e`  
		Last Modified: Thu, 09 Feb 2023 09:32:44 GMT  
		Size: 195.2 MB (195240411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5022758777785a1dbb502cbc8b4a2c80974ed7b16dbf1c8df3f7a1f65c838e45`  
		Last Modified: Thu, 09 Feb 2023 10:06:51 GMT  
		Size: 3.9 KB (3886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07a91cad901bee4f9dbfbc19b97e2d6aa4a23800fb1d45d07cb34a35876bf49`  
		Last Modified: Thu, 09 Feb 2023 10:06:51 GMT  
		Size: 8.2 KB (8172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b383a211a2a19b8b0208b486ed02b2a8e4518cb0a8ffd0e313fc5fea07e31246`  
		Last Modified: Thu, 09 Feb 2023 10:07:00 GMT  
		Size: 233.1 MB (233090657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.18`

```console
$ docker pull neo4j@sha256:9b70f8f1e75778a781c520a4e2dfba85e2ca8dbb796fa732260f12a586c9a9e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.4.18` - linux; amd64

```console
$ docker pull neo4j@sha256:49420f700211821aafc8fe36f93f42c2d1a06550b173bbb8b40b228a9d85f6d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c376c2df22bca82454206679dfe66192798c2d69efee778333fa3093bd2e57`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Fri, 24 Feb 2023 23:20:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Feb 2023 23:20:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Fri, 24 Feb 2023 23:20:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Feb 2023 23:20:08 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Fri, 24 Feb 2023 23:20:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Feb 2023 23:20:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Feb 2023 23:20:26 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Feb 2023 23:20:26 GMT
VOLUME [/data /logs]
# Fri, 24 Feb 2023 23:20:26 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Feb 2023 23:20:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:20:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f0aa56bd87b7901051196bb1b7620f1ff34dc92263f0d184df0a08d7aeb82c`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b60a999bdf32267c36abeded1e6cd14311a682ab7f25f380a25af3f018c7d1`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f5e9ca57723073c75a95f8c7a46fa320974a0943f5207c7e3c2e4036d68ab`  
		Last Modified: Fri, 24 Feb 2023 23:21:22 GMT  
		Size: 136.9 MB (136902167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.18-community`

```console
$ docker pull neo4j@sha256:9b70f8f1e75778a781c520a4e2dfba85e2ca8dbb796fa732260f12a586c9a9e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.4.18-community` - linux; amd64

```console
$ docker pull neo4j@sha256:49420f700211821aafc8fe36f93f42c2d1a06550b173bbb8b40b228a9d85f6d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c376c2df22bca82454206679dfe66192798c2d69efee778333fa3093bd2e57`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Fri, 24 Feb 2023 23:20:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Feb 2023 23:20:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Fri, 24 Feb 2023 23:20:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Feb 2023 23:20:08 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Fri, 24 Feb 2023 23:20:25 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Feb 2023 23:20:26 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Feb 2023 23:20:26 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Feb 2023 23:20:26 GMT
VOLUME [/data /logs]
# Fri, 24 Feb 2023 23:20:26 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Feb 2023 23:20:26 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:20:26 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f0aa56bd87b7901051196bb1b7620f1ff34dc92263f0d184df0a08d7aeb82c`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b60a999bdf32267c36abeded1e6cd14311a682ab7f25f380a25af3f018c7d1`  
		Last Modified: Fri, 24 Feb 2023 23:21:14 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f5e9ca57723073c75a95f8c7a46fa320974a0943f5207c7e3c2e4036d68ab`  
		Last Modified: Fri, 24 Feb 2023 23:21:22 GMT  
		Size: 136.9 MB (136902167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.18-enterprise`

```console
$ docker pull neo4j@sha256:48d73b1ae16e5c87f5404b8e528ead4720518f5e263e32cb39d9ca5d11bc1285
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neo4j:4.4.18-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:d5ec99c2e2d4b6e188b0ad16c878bbad5259359221ecb643b5017ea29a2b4ba4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463205192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f02cea60ed2f60134725833b5cdac895d65993ec3af416f921de51fae504d49`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:25:37 GMT
COPY dir:fdbc5e9dec2946fa124877176e92a68dd3fe3a70def5bb906a6040c4a1303a2d in /opt/java/openjdk 
# Fri, 24 Feb 2023 23:20:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=79d7283199af9e4830dbf79ff36b98d8851b342724edd741785b91bad33f7d73 NEO4J_TARBALL=neo4j-enterprise-4.4.18-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Feb 2023 23:20:32 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
# Fri, 24 Feb 2023 23:20:33 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Feb 2023 23:20:33 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Fri, 24 Feb 2023 23:20:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Feb 2023 23:20:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Feb 2023 23:20:48 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Feb 2023 23:20:48 GMT
VOLUME [/data /logs]
# Fri, 24 Feb 2023 23:20:48 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Feb 2023 23:20:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Feb 2023 23:20:48 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9435812fc8d62eb5597536e4d415bb190bf5bd388839bf4cae0567b76b0a6a`  
		Last Modified: Thu, 09 Feb 2023 09:38:48 GMT  
		Size: 198.5 MB (198475423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6778e2f222523e1c1dd355bd0939e03e50dab1dacec2c2336abd79ea32cf39de`  
		Last Modified: Fri, 24 Feb 2023 23:21:35 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9da32a54015c12a92955440d5595420e145a7f8b283ae9da164d93a53eee447`  
		Last Modified: Fri, 24 Feb 2023 23:21:35 GMT  
		Size: 8.4 KB (8424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d90ec3e928ac12a1eedeb96f5a82e3b3808471eb723ea7591de5301dfaf217f`  
		Last Modified: Fri, 24 Feb 2023 23:21:46 GMT  
		Size: 233.3 MB (233305675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:1f05a4acd266f8b39b8fcaa05ff62bd054a5f70a9c07f294ccff3e32ec1d3a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:a8a7afa92f31bf58da7422d882efa84be2de9a919a2ae87b5c96dca12bc031cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.0 MB (543986579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a525ff2773cfecf77ab98ef5b38d9064c088b212f738edb47eda3c1b2c94744`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:48 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:48 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f683d23c8000af4790740d027cddb8a3c16a2a11135523aa79075bc8cdb730f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a524c124e12bdba79a04ca134324ad2dcd2dd2de74bbe800ba370198e13879`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc36a20b297d00d83d52323ae3a0e3513f5bae7979193f041a8d5d472aaad16`  
		Last Modified: Thu, 16 Feb 2023 21:37:55 GMT  
		Size: 320.1 MB (320124296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:48ef22c4c33e72700e09bff0f4ec657228d3a8d6f4a4cf8e475f1b018cca6a0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.3 MB (541317252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435f93b1eb0a4159c965848d19b1c55d2a606b693d6bec4f47d5d1e5d0e2ceb8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:48:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:48:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:48:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:48:15 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:37 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:37 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:37 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:37 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe18f4fcfc9b2a0eee34e23cfb3f536ffdf7f1c760e3ef3fbcab9f5c84c9c58`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c062c8daab34245a145264bee40a7949990c648517657c66da24306f97351d0`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c43b86d2e90a12dd93aca549e441caed90c418000eaf29f761555e82266344`  
		Last Modified: Thu, 16 Feb 2023 20:49:47 GMT  
		Size: 320.0 MB (319981998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.5`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.5` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.5-enterprise`

```console
$ docker pull neo4j@sha256:1f05a4acd266f8b39b8fcaa05ff62bd054a5f70a9c07f294ccff3e32ec1d3a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:a8a7afa92f31bf58da7422d882efa84be2de9a919a2ae87b5c96dca12bc031cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.0 MB (543986579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a525ff2773cfecf77ab98ef5b38d9064c088b212f738edb47eda3c1b2c94744`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:48 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:48 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f683d23c8000af4790740d027cddb8a3c16a2a11135523aa79075bc8cdb730f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a524c124e12bdba79a04ca134324ad2dcd2dd2de74bbe800ba370198e13879`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc36a20b297d00d83d52323ae3a0e3513f5bae7979193f041a8d5d472aaad16`  
		Last Modified: Thu, 16 Feb 2023 21:37:55 GMT  
		Size: 320.1 MB (320124296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:48ef22c4c33e72700e09bff0f4ec657228d3a8d6f4a4cf8e475f1b018cca6a0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.3 MB (541317252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435f93b1eb0a4159c965848d19b1c55d2a606b693d6bec4f47d5d1e5d0e2ceb8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:48:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:48:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:48:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:48:15 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:37 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:37 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:37 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:37 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe18f4fcfc9b2a0eee34e23cfb3f536ffdf7f1c760e3ef3fbcab9f5c84c9c58`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c062c8daab34245a145264bee40a7949990c648517657c66da24306f97351d0`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c43b86d2e90a12dd93aca549e441caed90c418000eaf29f761555e82266344`  
		Last Modified: Thu, 16 Feb 2023 20:49:47 GMT  
		Size: 320.0 MB (319981998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.5.0`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.5.0` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.5.0` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.5.0-community`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.5.0-community` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.5.0-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.5.0-enterprise`

```console
$ docker pull neo4j@sha256:1f05a4acd266f8b39b8fcaa05ff62bd054a5f70a9c07f294ccff3e32ec1d3a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.5.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:a8a7afa92f31bf58da7422d882efa84be2de9a919a2ae87b5c96dca12bc031cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.0 MB (543986579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a525ff2773cfecf77ab98ef5b38d9064c088b212f738edb47eda3c1b2c94744`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:48 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:48 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f683d23c8000af4790740d027cddb8a3c16a2a11135523aa79075bc8cdb730f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a524c124e12bdba79a04ca134324ad2dcd2dd2de74bbe800ba370198e13879`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc36a20b297d00d83d52323ae3a0e3513f5bae7979193f041a8d5d472aaad16`  
		Last Modified: Thu, 16 Feb 2023 21:37:55 GMT  
		Size: 320.1 MB (320124296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.5.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:48ef22c4c33e72700e09bff0f4ec657228d3a8d6f4a4cf8e475f1b018cca6a0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.3 MB (541317252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435f93b1eb0a4159c965848d19b1c55d2a606b693d6bec4f47d5d1e5d0e2ceb8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:48:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:48:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:48:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:48:15 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:37 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:37 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:37 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:37 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe18f4fcfc9b2a0eee34e23cfb3f536ffdf7f1c760e3ef3fbcab9f5c84c9c58`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c062c8daab34245a145264bee40a7949990c648517657c66da24306f97351d0`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c43b86d2e90a12dd93aca549e441caed90c418000eaf29f761555e82266344`  
		Last Modified: Thu, 16 Feb 2023 20:49:47 GMT  
		Size: 320.0 MB (319981998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:1f05a4acd266f8b39b8fcaa05ff62bd054a5f70a9c07f294ccff3e32ec1d3a56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:a8a7afa92f31bf58da7422d882efa84be2de9a919a2ae87b5c96dca12bc031cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.0 MB (543986579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a525ff2773cfecf77ab98ef5b38d9064c088b212f738edb47eda3c1b2c94744`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:29 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:47 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:48 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:48 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:48 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:48 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:48 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:49 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f683d23c8000af4790740d027cddb8a3c16a2a11135523aa79075bc8cdb730f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 3.9 KB (3862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a524c124e12bdba79a04ca134324ad2dcd2dd2de74bbe800ba370198e13879`  
		Last Modified: Thu, 16 Feb 2023 21:37:41 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc36a20b297d00d83d52323ae3a0e3513f5bae7979193f041a8d5d472aaad16`  
		Last Modified: Thu, 16 Feb 2023 21:37:55 GMT  
		Size: 320.1 MB (320124296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:48ef22c4c33e72700e09bff0f4ec657228d3a8d6f4a4cf8e475f1b018cca6a0a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.3 MB (541317252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:435f93b1eb0a4159c965848d19b1c55d2a606b693d6bec4f47d5d1e5d0e2ceb8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:48:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:48:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:48:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:48:15 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:37 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:37 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:37 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:37 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:37 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:37 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe18f4fcfc9b2a0eee34e23cfb3f536ffdf7f1c760e3ef3fbcab9f5c84c9c58`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c062c8daab34245a145264bee40a7949990c648517657c66da24306f97351d0`  
		Last Modified: Thu, 16 Feb 2023 20:49:34 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c43b86d2e90a12dd93aca549e441caed90c418000eaf29f761555e82266344`  
		Last Modified: Thu, 16 Feb 2023 20:49:47 GMT  
		Size: 320.0 MB (319981998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:dd579952b0639dfbe559053639017bf1732e5edb8af1eba7c8074bd9521004cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:1d0ca23fd444ceab6542b8af934d2bfc87b89397df179de1d7e0d67a70281a12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.1 MB (339058531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4beb50fc1d19385dfbc02a659fefbb02a5fa6854ede6c3db9f56954d1e3dd5cc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:22:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:28:39 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Thu, 16 Feb 2023 21:36:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 21:36:08 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 21:36:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 21:36:09 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 21:36:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 21:36:23 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 21:36:23 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 21:36:23 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 21:36:23 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 21:36:23 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 21:36:23 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c81d82cb4b2b71263b3117ae53e60d87a90991c692f5ff54bea94797fdf512`  
		Last Modified: Thu, 09 Feb 2023 09:40:40 GMT  
		Size: 192.4 MB (192438189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42f5373c79918fd2f553b9511df2e214ffa396d75e4f96ec68dc1bdfaf782fa`  
		Last Modified: Thu, 16 Feb 2023 21:37:15 GMT  
		Size: 3.9 KB (3857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd618b137adbcedbfcfbcf161d77766d95c01201a01e80d8b3b5778afb0a96f3`  
		Last Modified: Thu, 16 Feb 2023 21:37:16 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadcee6ab63b9229cbc7ed64e799d23549368d2cc27b1e143ab88f07948dd9c1`  
		Last Modified: Thu, 16 Feb 2023 21:37:22 GMT  
		Size: 115.2 MB (115196258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b24e256750ed580a0364815791affd19100d3ebf763cdaa16a4a588346b6c45a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336386453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecd558ea15aa12243377394ca7b493cba15d989a3668e714841f7592e3c275d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:18:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 09 Feb 2023 09:23:59 GMT
COPY dir:a1bd99c3d82513db94430c73467e1e5c69ea4624d0489571d594afe503e15dc5 in /opt/java/openjdk 
# Thu, 16 Feb 2023 20:47:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3834cf8393f11d02e96e37b15ceeb4319f56cf1d323076ca242a35750c94bd99 NEO4J_TARBALL=neo4j-community-5.5.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 16 Feb 2023 20:47:57 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
# Thu, 16 Feb 2023 20:47:58 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 16 Feb 2023 20:47:58 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 16 Feb 2023 20:48:09 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Feb 2023 20:48:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Feb 2023 20:48:10 GMT
WORKDIR /var/lib/neo4j
# Thu, 16 Feb 2023 20:48:10 GMT
VOLUME [/data /logs]
# Thu, 16 Feb 2023 20:48:10 GMT
EXPOSE 7473 7474 7687
# Thu, 16 Feb 2023 20:48:10 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 16 Feb 2023 20:48:10 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7586f864daee85da340c78373323940ea5aadab0913592ab630744b3a8d6605`  
		Last Modified: Thu, 09 Feb 2023 09:34:26 GMT  
		Size: 191.3 MB (191260427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b462ee3a9b270432d663174ae48473e4201a7a1b3edffed1ece6f4bd0efc000e`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2696509009deedf3202ab2612962baa8209f4d5cf74b9ccaa98b939ae1778116`  
		Last Modified: Thu, 16 Feb 2023 20:49:08 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d484aafea870e517fd22ee57f47ec6c802a9366fe5984cd784780b27d7e8d`  
		Last Modified: Thu, 16 Feb 2023 20:49:13 GMT  
		Size: 115.1 MB (115051204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
