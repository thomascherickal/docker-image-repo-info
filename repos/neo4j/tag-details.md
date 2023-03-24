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
-	[`neo4j:5.6`](#neo4j56)
-	[`neo4j:5.6-community`](#neo4j56-community)
-	[`neo4j:5.6-enterprise`](#neo4j56-enterprise)
-	[`neo4j:5.6.0`](#neo4j560)
-	[`neo4j:5.6.0-community`](#neo4j560-community)
-	[`neo4j:5.6.0-enterprise`](#neo4j560-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:5fd30c52a8c347334641ea62954a420104b40253535a8018ec3cc91fb0713c9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:35132e250f369f65317669dd9a40764d53a9a7d73e74fd164e2ad1edcf79ea7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a033f94824db94dcf441e958594fac226f0fde3a969450735f601e6569f630`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 11:03:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 11:03:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 11:03:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 11:03:05 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 11:03:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:03:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 11:03:16 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 11:03:16 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 11:03:16 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 11:03:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:03:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07b6107ad6cad1f26945f3e6842250014d744b27daed70785fda7260e61f947`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ecdcb03eefdaebde879a8821ef1e1d8bfb9a83f6ae18d4c9bfd0b7d388ee3e`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8317950f49265fb09e6120506b1443ca4231d58ada059cf8ae30dddc803cb21`  
		Last Modified: Thu, 23 Mar 2023 11:04:46 GMT  
		Size: 136.9 MB (136902037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:974d2bc993a5bccc6d18281df20dfcfb9882d31c103c81fb9325062fe32fa0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362075588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efcdeb05932c0864beea579ba99a38a67d5bfdbd172ff4867d003475fbd5a1ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 09:27:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 09:27:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 09:27:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 09:27:56 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 09:28:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:28:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:28:11 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 09:28:11 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 09:28:11 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 09:28:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:28:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c17b3e1003a25ccc751bf8e2bfd321a5c1fd7659987ef911e46304299e175a`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e567401fb087731dab7280300ba60e3d4eb092c6d35c92496bae2277307258`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 8.4 KB (8426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569a5e1cf6f904f2a144d63ec10347e392f71b2513d540b2abdaa5d3d4524d8e`  
		Last Modified: Thu, 23 Mar 2023 09:29:30 GMT  
		Size: 136.8 MB (136758068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:5fd30c52a8c347334641ea62954a420104b40253535a8018ec3cc91fb0713c9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:35132e250f369f65317669dd9a40764d53a9a7d73e74fd164e2ad1edcf79ea7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a033f94824db94dcf441e958594fac226f0fde3a969450735f601e6569f630`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 11:03:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 11:03:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 11:03:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 11:03:05 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 11:03:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:03:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 11:03:16 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 11:03:16 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 11:03:16 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 11:03:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:03:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07b6107ad6cad1f26945f3e6842250014d744b27daed70785fda7260e61f947`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ecdcb03eefdaebde879a8821ef1e1d8bfb9a83f6ae18d4c9bfd0b7d388ee3e`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8317950f49265fb09e6120506b1443ca4231d58ada059cf8ae30dddc803cb21`  
		Last Modified: Thu, 23 Mar 2023 11:04:46 GMT  
		Size: 136.9 MB (136902037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:974d2bc993a5bccc6d18281df20dfcfb9882d31c103c81fb9325062fe32fa0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362075588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efcdeb05932c0864beea579ba99a38a67d5bfdbd172ff4867d003475fbd5a1ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 09:27:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 09:27:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 09:27:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 09:27:56 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 09:28:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:28:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:28:11 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 09:28:11 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 09:28:11 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 09:28:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:28:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c17b3e1003a25ccc751bf8e2bfd321a5c1fd7659987ef911e46304299e175a`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e567401fb087731dab7280300ba60e3d4eb092c6d35c92496bae2277307258`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 8.4 KB (8426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569a5e1cf6f904f2a144d63ec10347e392f71b2513d540b2abdaa5d3d4524d8e`  
		Last Modified: Thu, 23 Mar 2023 09:29:30 GMT  
		Size: 136.8 MB (136758068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:50e1e681d198cf65e3f0139f39f472c4b443092ca3069cb8d1b8457baeb98a71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ad18ca24513387e22d15608629a839d149e39b357f1a8777eb26fc340341c73a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463205313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2dd6d28c1194314e0d3420d893daa6cf8499fd11912e5e77808c7b62aa83a3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 11:03:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=79d7283199af9e4830dbf79ff36b98d8851b342724edd741785b91bad33f7d73 NEO4J_TARBALL=neo4j-enterprise-4.4.18-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 11:03:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 11:03:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 11:03:21 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 11:03:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:03:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 11:03:35 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 11:03:35 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 11:03:35 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 11:03:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:03:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cc28c0b5bddc8a52b63c308dcf86e3e55043280bfd511006320714612e6b97`  
		Last Modified: Thu, 23 Mar 2023 11:04:59 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ecbac13782f0360baafd099a307bb2a5983a72cf0d7b9c45f9548155300a53`  
		Last Modified: Thu, 23 Mar 2023 11:04:59 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdca2b0bf78527bc412657e5b1402f215abf46840a1e5ce0d0d1b2f26e8567a`  
		Last Modified: Thu, 23 Mar 2023 11:05:09 GMT  
		Size: 233.3 MB (233305625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:20b1e9c75f507e236151c9e247d49d960a5958043fd88e8c4e02e586df270d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.5 MB (458481365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bcdb99cbc1c91aae520330c7c5aa887e589b8dd56aa18b8b2effc1393474bb`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 09:28:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=79d7283199af9e4830dbf79ff36b98d8851b342724edd741785b91bad33f7d73 NEO4J_TARBALL=neo4j-enterprise-4.4.18-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 09:28:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 09:28:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 09:28:15 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 09:28:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:28:28 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:28:28 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 09:28:28 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 09:28:28 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 09:28:28 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:28:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dc2e6de40d5d91dd188ca6ecc199e44aff752442a01c2c97de35deb4c99924`  
		Last Modified: Thu, 23 Mar 2023 09:29:41 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc013b8d2427506ef55ea39d2a3122118e13ef9eccc5b22be5920b7d63b31024`  
		Last Modified: Thu, 23 Mar 2023 09:29:41 GMT  
		Size: 8.4 KB (8426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca4e7af447a0b1498062f6498f3af24f12839bc630131e2ab7fa6fbb26a18ce`  
		Last Modified: Thu, 23 Mar 2023 09:29:50 GMT  
		Size: 233.2 MB (233163847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.18`

```console
$ docker pull neo4j@sha256:5fd30c52a8c347334641ea62954a420104b40253535a8018ec3cc91fb0713c9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.18` - linux; amd64

```console
$ docker pull neo4j@sha256:35132e250f369f65317669dd9a40764d53a9a7d73e74fd164e2ad1edcf79ea7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a033f94824db94dcf441e958594fac226f0fde3a969450735f601e6569f630`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 11:03:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 11:03:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 11:03:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 11:03:05 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 11:03:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:03:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 11:03:16 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 11:03:16 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 11:03:16 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 11:03:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:03:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07b6107ad6cad1f26945f3e6842250014d744b27daed70785fda7260e61f947`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ecdcb03eefdaebde879a8821ef1e1d8bfb9a83f6ae18d4c9bfd0b7d388ee3e`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8317950f49265fb09e6120506b1443ca4231d58ada059cf8ae30dddc803cb21`  
		Last Modified: Thu, 23 Mar 2023 11:04:46 GMT  
		Size: 136.9 MB (136902037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.18` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:974d2bc993a5bccc6d18281df20dfcfb9882d31c103c81fb9325062fe32fa0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362075588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efcdeb05932c0864beea579ba99a38a67d5bfdbd172ff4867d003475fbd5a1ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 09:27:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 09:27:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 09:27:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 09:27:56 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 09:28:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:28:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:28:11 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 09:28:11 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 09:28:11 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 09:28:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:28:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c17b3e1003a25ccc751bf8e2bfd321a5c1fd7659987ef911e46304299e175a`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e567401fb087731dab7280300ba60e3d4eb092c6d35c92496bae2277307258`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 8.4 KB (8426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569a5e1cf6f904f2a144d63ec10347e392f71b2513d540b2abdaa5d3d4524d8e`  
		Last Modified: Thu, 23 Mar 2023 09:29:30 GMT  
		Size: 136.8 MB (136758068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.18-community`

```console
$ docker pull neo4j@sha256:5fd30c52a8c347334641ea62954a420104b40253535a8018ec3cc91fb0713c9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.18-community` - linux; amd64

```console
$ docker pull neo4j@sha256:35132e250f369f65317669dd9a40764d53a9a7d73e74fd164e2ad1edcf79ea7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.8 MB (366801731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14a033f94824db94dcf441e958594fac226f0fde3a969450735f601e6569f630`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 11:03:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 11:03:04 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 11:03:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 11:03:05 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 11:03:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:03:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 11:03:16 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 11:03:16 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 11:03:16 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 11:03:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:03:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07b6107ad6cad1f26945f3e6842250014d744b27daed70785fda7260e61f947`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ecdcb03eefdaebde879a8821ef1e1d8bfb9a83f6ae18d4c9bfd0b7d388ee3e`  
		Last Modified: Thu, 23 Mar 2023 11:04:39 GMT  
		Size: 8.4 KB (8427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8317950f49265fb09e6120506b1443ca4231d58ada059cf8ae30dddc803cb21`  
		Last Modified: Thu, 23 Mar 2023 11:04:46 GMT  
		Size: 136.9 MB (136902037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.18-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:974d2bc993a5bccc6d18281df20dfcfb9882d31c103c81fb9325062fe32fa0e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362075588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efcdeb05932c0864beea579ba99a38a67d5bfdbd172ff4867d003475fbd5a1ef`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 09:27:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=a57309da7081c89969d8763d6f41353ede93cc7fa3f65bf7b240571e13757c7e NEO4J_TARBALL=neo4j-community-4.4.18-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 09:27:55 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 09:27:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 09:27:56 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 09:28:10 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:28:10 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:28:11 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 09:28:11 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 09:28:11 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 09:28:11 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:28:11 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c17b3e1003a25ccc751bf8e2bfd321a5c1fd7659987ef911e46304299e175a`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e567401fb087731dab7280300ba60e3d4eb092c6d35c92496bae2277307258`  
		Last Modified: Thu, 23 Mar 2023 09:29:24 GMT  
		Size: 8.4 KB (8426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569a5e1cf6f904f2a144d63ec10347e392f71b2513d540b2abdaa5d3d4524d8e`  
		Last Modified: Thu, 23 Mar 2023 09:29:30 GMT  
		Size: 136.8 MB (136758068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.18-enterprise`

```console
$ docker pull neo4j@sha256:50e1e681d198cf65e3f0139f39f472c4b443092ca3069cb8d1b8457baeb98a71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.18-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ad18ca24513387e22d15608629a839d149e39b357f1a8777eb26fc340341c73a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.2 MB (463205313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2dd6d28c1194314e0d3420d893daa6cf8499fd11912e5e77808c7b62aa83a3`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:17:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:20:31 GMT
COPY dir:e649a995635d4b28f1458e8ccc09f5f71440b52479cfda5ea11e99ab14d0ce82 in /opt/java/openjdk 
# Thu, 23 Mar 2023 11:03:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=79d7283199af9e4830dbf79ff36b98d8851b342724edd741785b91bad33f7d73 NEO4J_TARBALL=neo4j-enterprise-4.4.18-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 11:03:20 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 11:03:21 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 11:03:21 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 11:03:35 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:03:35 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 11:03:35 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 11:03:35 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 11:03:35 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 11:03:35 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 11:03:35 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1504cbd1d7ea21f45a7c90d9e13b13742e330dcd47fdbe975ca32319c2681080`  
		Last Modified: Thu, 23 Mar 2023 06:31:09 GMT  
		Size: 198.5 MB (198476003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cc28c0b5bddc8a52b63c308dcf86e3e55043280bfd511006320714612e6b97`  
		Last Modified: Thu, 23 Mar 2023 11:04:59 GMT  
		Size: 3.9 KB (3861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ecbac13782f0360baafd099a307bb2a5983a72cf0d7b9c45f9548155300a53`  
		Last Modified: Thu, 23 Mar 2023 11:04:59 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdca2b0bf78527bc412657e5b1402f215abf46840a1e5ce0d0d1b2f26e8567a`  
		Last Modified: Thu, 23 Mar 2023 11:05:09 GMT  
		Size: 233.3 MB (233305625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.18-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:20b1e9c75f507e236151c9e247d49d960a5958043fd88e8c4e02e586df270d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **458.5 MB (458481365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bcdb99cbc1c91aae520330c7c5aa887e589b8dd56aa18b8b2effc1393474bb`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:52:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 23 Mar 2023 06:55:00 GMT
COPY dir:d446509417048b798354227404c222c2c6031477a91cb1b64eded33f5e598adf in /opt/java/openjdk 
# Thu, 23 Mar 2023 09:28:14 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=79d7283199af9e4830dbf79ff36b98d8851b342724edd741785b91bad33f7d73 NEO4J_TARBALL=neo4j-enterprise-4.4.18-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 23 Mar 2023 09:28:14 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
# Thu, 23 Mar 2023 09:28:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 23 Mar 2023 09:28:15 GMT
COPY multi:04123c94ab9ad8cef3e56e409d388ad61ce6394c2b8e0f4e659e18f898d77e6b in /startup/ 
# Thu, 23 Mar 2023 09:28:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.18-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:28:28 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 09:28:28 GMT
WORKDIR /var/lib/neo4j
# Thu, 23 Mar 2023 09:28:28 GMT
VOLUME [/data /logs]
# Thu, 23 Mar 2023 09:28:28 GMT
EXPOSE 7473 7474 7687
# Thu, 23 Mar 2023 09:28:28 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 09:28:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10110f881fd4b5d631a0d4a395c31433fb4f28f016302e6eac7248a1e22335b`  
		Last Modified: Thu, 23 Mar 2023 07:04:27 GMT  
		Size: 195.2 MB (195242507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dc2e6de40d5d91dd188ca6ecc199e44aff752442a01c2c97de35deb4c99924`  
		Last Modified: Thu, 23 Mar 2023 09:29:41 GMT  
		Size: 3.9 KB (3885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc013b8d2427506ef55ea39d2a3122118e13ef9eccc5b22be5920b7d63b31024`  
		Last Modified: Thu, 23 Mar 2023 09:29:41 GMT  
		Size: 8.4 KB (8426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca4e7af447a0b1498062f6498f3af24f12839bc630131e2ab7fa6fbb26a18ce`  
		Last Modified: Thu, 23 Mar 2023 09:29:50 GMT  
		Size: 233.2 MB (233163847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

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

### `neo4j:5` - linux; arm64 variant v8

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

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:f0744f3d4dc7113d067776146fa5c71eb60d6e0d6bb496cf1fd2e386e10f3d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:53844b481ebdf6f8ec3a30264eb15b5b2c6224a0abd53fa3273e7a0f244a3678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.3 MB (545304684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e5c88f53e159b0fd3e045d3b1ae24ddf543d0e92009037f27c7d2647663215`
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
# Fri, 24 Mar 2023 22:20:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 22:20:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 22:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 22:20:02 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 22:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 22:20:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 22:20:17 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 22:20:17 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 22:20:17 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 22:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 22:20:17 GMT
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
	-	`sha256:2c0692f4b94202076aae0fdaa32799b602d20d7d316b72ab0a338a3eda295cdf`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a36de4718fa975adc4387b365227c991e7a785f0b02c87bc529ff9c98358e1`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 8.6 KB (8628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fc6af6b16844b10f73533c4f9df3298ba8538133ea3018628e9c12ec471180`  
		Last Modified: Fri, 24 Mar 2023 22:21:13 GMT  
		Size: 321.4 MB (321442561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b9ca8620bf275c355f1a0c91e08f4021b77d8085688e550f53c5e97a945dd73f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542637385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99f644556f5270209518c368bef28b843eb0e87e0a697ba1ed239291a47797f8`
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
# Fri, 24 Mar 2023 21:39:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 21:39:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 21:39:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 21:39:52 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 21:40:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 21:40:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 21:40:16 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 21:40:16 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 21:40:16 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 21:40:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 21:40:16 GMT
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
	-	`sha256:221fa1e5d51596d29c3be8fc7afb442f3fda7a24f38f5f4fe102298178738f82`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da5b70be19f9d0b9c811a12643a062b324916131ba0c4bb805918970a02d0a9`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 8.6 KB (8630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b455ba0033d00f771eab13d343967e9e9cc42037389afa288c49821243874`  
		Last Modified: Fri, 24 Mar 2023 21:41:07 GMT  
		Size: 321.3 MB (321301752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.6`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.6` - linux; amd64

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

### `neo4j:5.6` - linux; arm64 variant v8

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

## `neo4j:5.6-community`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.6-community` - linux; amd64

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

### `neo4j:5.6-community` - linux; arm64 variant v8

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

## `neo4j:5.6-enterprise`

```console
$ docker pull neo4j@sha256:f0744f3d4dc7113d067776146fa5c71eb60d6e0d6bb496cf1fd2e386e10f3d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.6-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:53844b481ebdf6f8ec3a30264eb15b5b2c6224a0abd53fa3273e7a0f244a3678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.3 MB (545304684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e5c88f53e159b0fd3e045d3b1ae24ddf543d0e92009037f27c7d2647663215`
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
# Fri, 24 Mar 2023 22:20:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 22:20:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 22:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 22:20:02 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 22:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 22:20:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 22:20:17 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 22:20:17 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 22:20:17 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 22:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 22:20:17 GMT
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
	-	`sha256:2c0692f4b94202076aae0fdaa32799b602d20d7d316b72ab0a338a3eda295cdf`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a36de4718fa975adc4387b365227c991e7a785f0b02c87bc529ff9c98358e1`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 8.6 KB (8628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fc6af6b16844b10f73533c4f9df3298ba8538133ea3018628e9c12ec471180`  
		Last Modified: Fri, 24 Mar 2023 22:21:13 GMT  
		Size: 321.4 MB (321442561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.6-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b9ca8620bf275c355f1a0c91e08f4021b77d8085688e550f53c5e97a945dd73f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542637385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99f644556f5270209518c368bef28b843eb0e87e0a697ba1ed239291a47797f8`
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
# Fri, 24 Mar 2023 21:39:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 21:39:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 21:39:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 21:39:52 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 21:40:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 21:40:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 21:40:16 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 21:40:16 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 21:40:16 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 21:40:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 21:40:16 GMT
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
	-	`sha256:221fa1e5d51596d29c3be8fc7afb442f3fda7a24f38f5f4fe102298178738f82`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da5b70be19f9d0b9c811a12643a062b324916131ba0c4bb805918970a02d0a9`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 8.6 KB (8630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b455ba0033d00f771eab13d343967e9e9cc42037389afa288c49821243874`  
		Last Modified: Fri, 24 Mar 2023 21:41:07 GMT  
		Size: 321.3 MB (321301752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.6.0`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.6.0` - linux; amd64

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

### `neo4j:5.6.0` - linux; arm64 variant v8

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

## `neo4j:5.6.0-community`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.6.0-community` - linux; amd64

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

### `neo4j:5.6.0-community` - linux; arm64 variant v8

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

## `neo4j:5.6.0-enterprise`

```console
$ docker pull neo4j@sha256:f0744f3d4dc7113d067776146fa5c71eb60d6e0d6bb496cf1fd2e386e10f3d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5.6.0-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:53844b481ebdf6f8ec3a30264eb15b5b2c6224a0abd53fa3273e7a0f244a3678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.3 MB (545304684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e5c88f53e159b0fd3e045d3b1ae24ddf543d0e92009037f27c7d2647663215`
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
# Fri, 24 Mar 2023 22:20:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 22:20:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 22:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 22:20:02 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 22:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 22:20:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 22:20:17 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 22:20:17 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 22:20:17 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 22:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 22:20:17 GMT
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
	-	`sha256:2c0692f4b94202076aae0fdaa32799b602d20d7d316b72ab0a338a3eda295cdf`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a36de4718fa975adc4387b365227c991e7a785f0b02c87bc529ff9c98358e1`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 8.6 KB (8628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fc6af6b16844b10f73533c4f9df3298ba8538133ea3018628e9c12ec471180`  
		Last Modified: Fri, 24 Mar 2023 22:21:13 GMT  
		Size: 321.4 MB (321442561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5.6.0-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b9ca8620bf275c355f1a0c91e08f4021b77d8085688e550f53c5e97a945dd73f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542637385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99f644556f5270209518c368bef28b843eb0e87e0a697ba1ed239291a47797f8`
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
# Fri, 24 Mar 2023 21:39:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 21:39:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 21:39:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 21:39:52 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 21:40:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 21:40:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 21:40:16 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 21:40:16 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 21:40:16 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 21:40:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 21:40:16 GMT
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
	-	`sha256:221fa1e5d51596d29c3be8fc7afb442f3fda7a24f38f5f4fe102298178738f82`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da5b70be19f9d0b9c811a12643a062b324916131ba0c4bb805918970a02d0a9`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 8.6 KB (8630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b455ba0033d00f771eab13d343967e9e9cc42037389afa288c49821243874`  
		Last Modified: Fri, 24 Mar 2023 21:41:07 GMT  
		Size: 321.3 MB (321301752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:community`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

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

### `neo4j:community` - linux; arm64 variant v8

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

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:f0744f3d4dc7113d067776146fa5c71eb60d6e0d6bb496cf1fd2e386e10f3d89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:53844b481ebdf6f8ec3a30264eb15b5b2c6224a0abd53fa3273e7a0f244a3678
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.3 MB (545304684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e5c88f53e159b0fd3e045d3b1ae24ddf543d0e92009037f27c7d2647663215`
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
# Fri, 24 Mar 2023 22:20:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 22:20:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 22:20:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 22:20:02 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 22:20:16 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 22:20:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 22:20:17 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 22:20:17 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 22:20:17 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 22:20:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 22:20:17 GMT
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
	-	`sha256:2c0692f4b94202076aae0fdaa32799b602d20d7d316b72ab0a338a3eda295cdf`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 3.9 KB (3856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a36de4718fa975adc4387b365227c991e7a785f0b02c87bc529ff9c98358e1`  
		Last Modified: Fri, 24 Mar 2023 22:21:00 GMT  
		Size: 8.6 KB (8628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fc6af6b16844b10f73533c4f9df3298ba8538133ea3018628e9c12ec471180`  
		Last Modified: Fri, 24 Mar 2023 22:21:13 GMT  
		Size: 321.4 MB (321442561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:b9ca8620bf275c355f1a0c91e08f4021b77d8085688e550f53c5e97a945dd73f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.6 MB (542637385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99f644556f5270209518c368bef28b843eb0e87e0a697ba1ed239291a47797f8`
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
# Fri, 24 Mar 2023 21:39:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=01eebdd9a24ea10ab3c863bb11d59faa4d732f84801ff755f1d2d5aad27fad9b NEO4J_TARBALL=neo4j-enterprise-5.6.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Fri, 24 Mar 2023 21:39:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
# Fri, 24 Mar 2023 21:39:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Fri, 24 Mar 2023 21:39:52 GMT
COPY multi:a0d7d5f1f7f5a76cb0c8925dfafbe8943f9d1b1a76afc1b0ac964f6eb93156be in /startup/ 
# Fri, 24 Mar 2023 21:40:14 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.6.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 21:40:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Mar 2023 21:40:16 GMT
WORKDIR /var/lib/neo4j
# Fri, 24 Mar 2023 21:40:16 GMT
VOLUME [/data /logs]
# Fri, 24 Mar 2023 21:40:16 GMT
EXPOSE 7473 7474 7687
# Fri, 24 Mar 2023 21:40:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 21:40:16 GMT
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
	-	`sha256:221fa1e5d51596d29c3be8fc7afb442f3fda7a24f38f5f4fe102298178738f82`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da5b70be19f9d0b9c811a12643a062b324916131ba0c4bb805918970a02d0a9`  
		Last Modified: Fri, 24 Mar 2023 21:40:56 GMT  
		Size: 8.6 KB (8630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625b455ba0033d00f771eab13d343967e9e9cc42037389afa288c49821243874`  
		Last Modified: Fri, 24 Mar 2023 21:41:07 GMT  
		Size: 321.3 MB (321301752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:81ef7aa43a1fb07bf90d1759d5fcd4be1378284cfbafdd398530b6de8e2e63c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

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

### `neo4j:latest` - linux; arm64 variant v8

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
