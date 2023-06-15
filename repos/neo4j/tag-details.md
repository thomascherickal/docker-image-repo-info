<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `neo4j`

-	[`neo4j:4.4`](#neo4j44)
-	[`neo4j:4.4-community`](#neo4j44-community)
-	[`neo4j:4.4-enterprise`](#neo4j44-enterprise)
-	[`neo4j:4.4.21`](#neo4j4421)
-	[`neo4j:4.4.21-community`](#neo4j4421-community)
-	[`neo4j:4.4.21-enterprise`](#neo4j4421-enterprise)
-	[`neo4j:5`](#neo4j5)
-	[`neo4j:5-community`](#neo4j5-community)
-	[`neo4j:5-enterprise`](#neo4j5-enterprise)
-	[`neo4j:5.9`](#neo4j59)
-	[`neo4j:5.9-community`](#neo4j59-community)
-	[`neo4j:5.9-enterprise`](#neo4j59-enterprise)
-	[`neo4j:5.9.0`](#neo4j590)
-	[`neo4j:5.9.0-community`](#neo4j590-community)
-	[`neo4j:5.9.0-enterprise`](#neo4j590-enterprise)
-	[`neo4j:community`](#neo4jcommunity)
-	[`neo4j:enterprise`](#neo4jenterprise)
-	[`neo4j:latest`](#neo4jlatest)

## `neo4j:4.4`

```console
$ docker pull neo4j@sha256:82ac6ab02d981e73692151098bea6e08e8fdeaadc03b6025869de22f7939db77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4` - linux; amd64

```console
$ docker pull neo4j@sha256:dd4318b651ad983378861962a03bdf438d5e4987113072c351680c97d239febd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.5 MB (347524747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab1a7ce42f4b7e3fb946a9a24074d511e0b91bd3e8642656c1a7f621d7e4f66`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 07:09:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:46 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 07:09:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:57 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:57 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52bbd3276d540815ed2fcc39902019efa9c5867b71d96349503f4cbdac6492f`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa7ce1a38a8958cb0f1411cb1233dba1800c24433c556180ca07052390abb74`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 8.7 KB (8705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aebbd90d9d90e3fad994486634f455689c6790f7520d7467626d0da181c7034`  
		Last Modified: Tue, 13 Jun 2023 07:11:24 GMT  
		Size: 117.5 MB (117545083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:882619ea1656ca3e2a879d880558a547bd061b5e5f95cfd8790e337c820e0ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.8 MB (342801825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57508b9e3f04cf1b3f5fd889b72975bbeaabf1528443da28ef6add09310dd7a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:29:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:29:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 04:29:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:29:51 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 04:30:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:30:05 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:30:05 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:30:05 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:30:05 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:30:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:30:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb3aff3312dad546a13b7cadda0e8304af81bc20b06808891143c7689be71a`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b971fd90025b95bc3ba69c758b39b44947d875f1dc73d3c533a6af08be2357ec`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77645ef2b460d888bdaa9cf1de282f67faabbfcf435b00968c1c8d8954eecb73`  
		Last Modified: Tue, 13 Jun 2023 04:31:46 GMT  
		Size: 117.4 MB (117402192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-community`

```console
$ docker pull neo4j@sha256:82ac6ab02d981e73692151098bea6e08e8fdeaadc03b6025869de22f7939db77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-community` - linux; amd64

```console
$ docker pull neo4j@sha256:dd4318b651ad983378861962a03bdf438d5e4987113072c351680c97d239febd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.5 MB (347524747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab1a7ce42f4b7e3fb946a9a24074d511e0b91bd3e8642656c1a7f621d7e4f66`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 07:09:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:46 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 07:09:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:57 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:57 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52bbd3276d540815ed2fcc39902019efa9c5867b71d96349503f4cbdac6492f`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa7ce1a38a8958cb0f1411cb1233dba1800c24433c556180ca07052390abb74`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 8.7 KB (8705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aebbd90d9d90e3fad994486634f455689c6790f7520d7467626d0da181c7034`  
		Last Modified: Tue, 13 Jun 2023 07:11:24 GMT  
		Size: 117.5 MB (117545083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:882619ea1656ca3e2a879d880558a547bd061b5e5f95cfd8790e337c820e0ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.8 MB (342801825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57508b9e3f04cf1b3f5fd889b72975bbeaabf1528443da28ef6add09310dd7a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:29:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:29:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 04:29:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:29:51 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 04:30:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:30:05 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:30:05 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:30:05 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:30:05 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:30:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:30:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb3aff3312dad546a13b7cadda0e8304af81bc20b06808891143c7689be71a`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b971fd90025b95bc3ba69c758b39b44947d875f1dc73d3c533a6af08be2357ec`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77645ef2b460d888bdaa9cf1de282f67faabbfcf435b00968c1c8d8954eecb73`  
		Last Modified: Tue, 13 Jun 2023 04:31:46 GMT  
		Size: 117.4 MB (117402192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4-enterprise`

```console
$ docker pull neo4j@sha256:9bfc4ca0662b912b4ffcc0640ad76850f3af4e5aeb019172841e0cf3cb411dfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b43ceec4ae9093d66ed9bc80bfe1f5ab3d39b5a09c47d9a1c19a09b7a8fda05f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.2 MB (447190718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64677e7cdb3c3677a2fdd774c4bb7390c10a32e3d1729daba20fd779f511df8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:10:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0305b7bdefa4efae16d0a72e19bda6e79150b7423e739d789dd945e355a389f4 NEO4J_TARBALL=neo4j-enterprise-4.4.21-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:10:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 07:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:10:03 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 07:10:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:10:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:10:16 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:10:16 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:10:16 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:10:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:10:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d603ac12862fbba9d6667403f36662fed465b1b377f7a332d8a08aa5c3762c5b`  
		Last Modified: Tue, 13 Jun 2023 07:11:36 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e9e22a40fc8e754e2ecf4b730ad54a6cb54bc8561a6eb1d53b27101ae0ead3`  
		Last Modified: Tue, 13 Jun 2023 07:11:36 GMT  
		Size: 8.7 KB (8702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9274fe3db45b0aa387aae79ee4c99fd5efb13811df124b91eefa8654c3f9d01c`  
		Last Modified: Tue, 13 Jun 2023 07:11:45 GMT  
		Size: 217.2 MB (217211057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8ff16c279dc81812523f36e5d5793313056a663e54560dd3bab38f770d81f17e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.5 MB (442467390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e75c529f455dd292372ecaa96cf2ea0d9d768f3652c1ecedd0bf9746ef9bb26`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:30:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0305b7bdefa4efae16d0a72e19bda6e79150b7423e739d789dd945e355a389f4 NEO4J_TARBALL=neo4j-enterprise-4.4.21-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:30:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 04:30:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:30:08 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 04:30:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:30:28 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:30:28 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:30:28 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:30:28 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:30:28 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:30:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153ffc746d57b906cf25db5eee3b952b15657583885830f135a863cd9065271`  
		Last Modified: Tue, 13 Jun 2023 04:32:03 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308495ae9eb8fb9840d3601c664483326c5211adc308d856f086dcb32082417b`  
		Last Modified: Tue, 13 Jun 2023 04:32:03 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5126f9252c113ec5cebd7c0498eeac85bd9a94dca7101e2e3845b8b6fc6c9c`  
		Last Modified: Tue, 13 Jun 2023 04:32:12 GMT  
		Size: 217.1 MB (217067747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.21`

```console
$ docker pull neo4j@sha256:82ac6ab02d981e73692151098bea6e08e8fdeaadc03b6025869de22f7939db77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.21` - linux; amd64

```console
$ docker pull neo4j@sha256:dd4318b651ad983378861962a03bdf438d5e4987113072c351680c97d239febd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.5 MB (347524747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab1a7ce42f4b7e3fb946a9a24074d511e0b91bd3e8642656c1a7f621d7e4f66`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 07:09:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:46 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 07:09:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:57 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:57 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52bbd3276d540815ed2fcc39902019efa9c5867b71d96349503f4cbdac6492f`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa7ce1a38a8958cb0f1411cb1233dba1800c24433c556180ca07052390abb74`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 8.7 KB (8705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aebbd90d9d90e3fad994486634f455689c6790f7520d7467626d0da181c7034`  
		Last Modified: Tue, 13 Jun 2023 07:11:24 GMT  
		Size: 117.5 MB (117545083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.21` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:882619ea1656ca3e2a879d880558a547bd061b5e5f95cfd8790e337c820e0ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.8 MB (342801825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57508b9e3f04cf1b3f5fd889b72975bbeaabf1528443da28ef6add09310dd7a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:29:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:29:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 04:29:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:29:51 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 04:30:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:30:05 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:30:05 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:30:05 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:30:05 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:30:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:30:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb3aff3312dad546a13b7cadda0e8304af81bc20b06808891143c7689be71a`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b971fd90025b95bc3ba69c758b39b44947d875f1dc73d3c533a6af08be2357ec`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77645ef2b460d888bdaa9cf1de282f67faabbfcf435b00968c1c8d8954eecb73`  
		Last Modified: Tue, 13 Jun 2023 04:31:46 GMT  
		Size: 117.4 MB (117402192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.21-community`

```console
$ docker pull neo4j@sha256:82ac6ab02d981e73692151098bea6e08e8fdeaadc03b6025869de22f7939db77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.21-community` - linux; amd64

```console
$ docker pull neo4j@sha256:dd4318b651ad983378861962a03bdf438d5e4987113072c351680c97d239febd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.5 MB (347524747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab1a7ce42f4b7e3fb946a9a24074d511e0b91bd3e8642656c1a7f621d7e4f66`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:45 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 07:09:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:46 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 07:09:56 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:56 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:57 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:57 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:57 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:57 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:57 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52bbd3276d540815ed2fcc39902019efa9c5867b71d96349503f4cbdac6492f`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa7ce1a38a8958cb0f1411cb1233dba1800c24433c556180ca07052390abb74`  
		Last Modified: Tue, 13 Jun 2023 07:11:19 GMT  
		Size: 8.7 KB (8705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aebbd90d9d90e3fad994486634f455689c6790f7520d7467626d0da181c7034`  
		Last Modified: Tue, 13 Jun 2023 07:11:24 GMT  
		Size: 117.5 MB (117545083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.21-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:882619ea1656ca3e2a879d880558a547bd061b5e5f95cfd8790e337c820e0ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.8 MB (342801825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57508b9e3f04cf1b3f5fd889b72975bbeaabf1528443da28ef6add09310dd7a4`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:29:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=ba7cef86b9b2f0743f3855f4543f81fa46d07c5c724a56e5f4e0f437e20cc3a5 NEO4J_TARBALL=neo4j-community-4.4.21-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:29:50 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 04:29:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:29:51 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 04:30:04 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:30:05 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:30:05 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:30:05 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:30:05 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:30:05 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:30:05 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccb3aff3312dad546a13b7cadda0e8304af81bc20b06808891143c7689be71a`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b971fd90025b95bc3ba69c758b39b44947d875f1dc73d3c533a6af08be2357ec`  
		Last Modified: Tue, 13 Jun 2023 04:31:41 GMT  
		Size: 8.7 KB (8704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77645ef2b460d888bdaa9cf1de282f67faabbfcf435b00968c1c8d8954eecb73`  
		Last Modified: Tue, 13 Jun 2023 04:31:46 GMT  
		Size: 117.4 MB (117402192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:4.4.21-enterprise`

```console
$ docker pull neo4j@sha256:9bfc4ca0662b912b4ffcc0640ad76850f3af4e5aeb019172841e0cf3cb411dfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:4.4.21-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:b43ceec4ae9093d66ed9bc80bfe1f5ab3d39b5a09c47d9a1c19a09b7a8fda05f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.2 MB (447190718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64677e7cdb3c3677a2fdd774c4bb7390c10a32e3d1729daba20fd779f511df8`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:47:29 GMT
COPY dir:99fc054d8f67589023f9478fc6ae691114aff76e696d34d4988a30c767727d32 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:10:02 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0305b7bdefa4efae16d0a72e19bda6e79150b7423e739d789dd945e355a389f4 NEO4J_TARBALL=neo4j-enterprise-4.4.21-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:10:02 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 07:10:02 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:10:03 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 07:10:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:10:16 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:10:16 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:10:16 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:10:16 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:10:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:10:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c93dc0976ab0e1cedf14e59a533cbc8c624427cdfc4ff4080297f31ee3a366`  
		Last Modified: Tue, 13 Jun 2023 03:57:23 GMT  
		Size: 198.5 MB (198549694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d603ac12862fbba9d6667403f36662fed465b1b377f7a332d8a08aa5c3762c5b`  
		Last Modified: Tue, 13 Jun 2023 07:11:36 GMT  
		Size: 3.9 KB (3855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e9e22a40fc8e754e2ecf4b730ad54a6cb54bc8561a6eb1d53b27101ae0ead3`  
		Last Modified: Tue, 13 Jun 2023 07:11:36 GMT  
		Size: 8.7 KB (8702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9274fe3db45b0aa387aae79ee4c99fd5efb13811df124b91eefa8654c3f9d01c`  
		Last Modified: Tue, 13 Jun 2023 07:11:45 GMT  
		Size: 217.2 MB (217211057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:4.4.21-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:8ff16c279dc81812523f36e5d5793313056a663e54560dd3bab38f770d81f17e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.5 MB (442467390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e75c529f455dd292372ecaa96cf2ea0d9d768f3652c1ecedd0bf9746ef9bb26`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:29:47 GMT
COPY dir:26a87923e6280eb6d7e3200000ba2b8bbfa8612b133801ac6abaec9535613186 in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:30:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0305b7bdefa4efae16d0a72e19bda6e79150b7423e739d789dd945e355a389f4 NEO4J_TARBALL=neo4j-enterprise-4.4.21-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:30:07 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
# Tue, 13 Jun 2023 04:30:08 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:30:08 GMT
COPY multi:444df161c1a5ee60f2235df18d0f75c88fbf992084b1774572a5350de0772b1f in /startup/ 
# Tue, 13 Jun 2023 04:30:26 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-4.4.21-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && ln -s /startup/docker-entrypoint.sh /docker-entrypoint.sh     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:30:28 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:30:28 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:30:28 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:30:28 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:30:28 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:30:28 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95c7296223cd8d65203506b7cc022a934e2af6937394ef0f20e9a9d29a67dc4`  
		Last Modified: Tue, 13 Jun 2023 04:31:52 GMT  
		Size: 195.3 MB (195324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f153ffc746d57b906cf25db5eee3b952b15657583885830f135a863cd9065271`  
		Last Modified: Tue, 13 Jun 2023 04:32:03 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308495ae9eb8fb9840d3601c664483326c5211adc308d856f086dcb32082417b`  
		Last Modified: Tue, 13 Jun 2023 04:32:03 GMT  
		Size: 8.7 KB (8707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5126f9252c113ec5cebd7c0498eeac85bd9a94dca7101e2e3845b8b6fc6c9c`  
		Last Modified: Tue, 13 Jun 2023 04:32:12 GMT  
		Size: 217.1 MB (217067747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5`

```console
$ docker pull neo4j@sha256:3bf8dbbda1ef52063693b245c06bf5e9d2768195f082b1b1aed9933475470540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5` - linux; amd64

```console
$ docker pull neo4j@sha256:dc272726680f27f10425e6697cc405103478e358968976515aadfa11b319cbd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338698875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad022bbe615bdf0661ab86f40e73af636e0c6e870e3c60d844b9562397fbefc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 07:09:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:02 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 07:09:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:15 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:15 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:15 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8134a37330edefa0a033fee2d31970e964caeab4aa96bb417e63fb3c0a8e14c`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384b9f2bbf845f7870bc14fa917d7af3ee40d6142a2610c7ed042beb35caaab`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cca560702bb0d53e76d67b7c780c1a7a368d00966c9fd3074d917380e1fd11`  
		Last Modified: Tue, 13 Jun 2023 07:10:35 GMT  
		Size: 114.7 MB (114688458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7dd07e2a806fc23110252785bf391d326ae3302b5398dbddace99dd805c6c16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (336008316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e89cfbba3028caa9c5f7c9e882d0e9b7e5c040d9299cde2c1f91b23816d1191`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:28:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:28:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 04:28:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:28:55 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 04:29:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:29:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:29:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:29:07 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:29:07 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:29:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0a981bd793b3c89ab46f2f6bd1114add130d3116491701e31f0d53f8f12fc7`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539f80e3d71c865200143adaa99ddd5e103f310fe461b2b53d6eaab5e022a22`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ace878b15edfb608ab92fa81107f69cd2c890e1eaec38702cc19dc7a59a74d`  
		Last Modified: Tue, 13 Jun 2023 04:30:46 GMT  
		Size: 114.5 MB (114545124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:3bf8dbbda1ef52063693b245c06bf5e9d2768195f082b1b1aed9933475470540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:dc272726680f27f10425e6697cc405103478e358968976515aadfa11b319cbd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338698875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad022bbe615bdf0661ab86f40e73af636e0c6e870e3c60d844b9562397fbefc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 07:09:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:02 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 07:09:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:15 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:15 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:15 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8134a37330edefa0a033fee2d31970e964caeab4aa96bb417e63fb3c0a8e14c`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384b9f2bbf845f7870bc14fa917d7af3ee40d6142a2610c7ed042beb35caaab`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cca560702bb0d53e76d67b7c780c1a7a368d00966c9fd3074d917380e1fd11`  
		Last Modified: Tue, 13 Jun 2023 07:10:35 GMT  
		Size: 114.7 MB (114688458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7dd07e2a806fc23110252785bf391d326ae3302b5398dbddace99dd805c6c16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (336008316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e89cfbba3028caa9c5f7c9e882d0e9b7e5c040d9299cde2c1f91b23816d1191`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:28:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:28:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 04:28:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:28:55 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 04:29:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:29:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:29:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:29:07 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:29:07 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:29:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0a981bd793b3c89ab46f2f6bd1114add130d3116491701e31f0d53f8f12fc7`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539f80e3d71c865200143adaa99ddd5e103f310fe461b2b53d6eaab5e022a22`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ace878b15edfb608ab92fa81107f69cd2c890e1eaec38702cc19dc7a59a74d`  
		Last Modified: Tue, 13 Jun 2023 04:30:46 GMT  
		Size: 114.5 MB (114545124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5-enterprise`

```console
$ docker pull neo4j@sha256:434f6d6881ff88ff4b7cee78c77fa384e4a87c18fe0a202ca11474201e233f59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ad5059312602da31f495de528acd61a02792211ba7f6afe6a237c28c2bd83dc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603693681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fe6db03b9bb80cb21f732d449caa760ac83ffeb0ffe2dbd730f5021c5e724b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 07:09:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:22 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 07:09:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:39 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:39 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:39 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99699bd121b4a8e64f15735f4d0ef691635afc9777ee9e5b73073c94a8214638`  
		Last Modified: Tue, 13 Jun 2023 07:10:52 GMT  
		Size: 3.9 KB (3851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5059e97d213de7dade187caa587fceb9b23f57db3e6caf64e09af2c39f35ce`  
		Last Modified: Tue, 13 Jun 2023 07:10:53 GMT  
		Size: 8.8 KB (8767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14dbbfd6f8869fa267d5919c8ecbacdbb013106b99f179b389e724d5f3c8822`  
		Last Modified: Tue, 13 Jun 2023 07:11:07 GMT  
		Size: 379.7 MB (379683265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:beed155222ae1f4e0863bc0ec29c3f77b3f17318a4ffe2ec101f2a6864c79e94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.0 MB (601004543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc60798e3794bc19227cce0943e89daf6c16c55acda863d78b4888b091dbd60`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:29:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:29:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 04:29:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:29:11 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 04:29:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:29:40 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:29:40 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:29:40 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:29:41 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:29:41 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:41 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8c0f56f0edd204dd07e721377ffe1fa3b4a6593019f5e83dff05ada292b3e7`  
		Last Modified: Tue, 13 Jun 2023 04:31:15 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf3f09cefbb2f5fd58d3a43b66da125f5d716a929f6b7631f83f886f3da76dc`  
		Last Modified: Tue, 13 Jun 2023 04:31:15 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db23f413388e2fc9cdda0c1b366db473e92dd32bbb3bd89de28cc9a2356acb2`  
		Last Modified: Tue, 13 Jun 2023 04:31:27 GMT  
		Size: 379.5 MB (379541351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:5.9`

**does not exist** (yet?)

## `neo4j:5.9-community`

**does not exist** (yet?)

## `neo4j:5.9-enterprise`

**does not exist** (yet?)

## `neo4j:5.9.0`

**does not exist** (yet?)

## `neo4j:5.9.0-community`

**does not exist** (yet?)

## `neo4j:5.9.0-enterprise`

**does not exist** (yet?)

## `neo4j:community`

```console
$ docker pull neo4j@sha256:3bf8dbbda1ef52063693b245c06bf5e9d2768195f082b1b1aed9933475470540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:community` - linux; amd64

```console
$ docker pull neo4j@sha256:dc272726680f27f10425e6697cc405103478e358968976515aadfa11b319cbd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338698875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad022bbe615bdf0661ab86f40e73af636e0c6e870e3c60d844b9562397fbefc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 07:09:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:02 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 07:09:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:15 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:15 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:15 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8134a37330edefa0a033fee2d31970e964caeab4aa96bb417e63fb3c0a8e14c`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384b9f2bbf845f7870bc14fa917d7af3ee40d6142a2610c7ed042beb35caaab`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cca560702bb0d53e76d67b7c780c1a7a368d00966c9fd3074d917380e1fd11`  
		Last Modified: Tue, 13 Jun 2023 07:10:35 GMT  
		Size: 114.7 MB (114688458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7dd07e2a806fc23110252785bf391d326ae3302b5398dbddace99dd805c6c16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (336008316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e89cfbba3028caa9c5f7c9e882d0e9b7e5c040d9299cde2c1f91b23816d1191`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:28:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:28:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 04:28:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:28:55 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 04:29:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:29:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:29:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:29:07 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:29:07 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:29:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0a981bd793b3c89ab46f2f6bd1114add130d3116491701e31f0d53f8f12fc7`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539f80e3d71c865200143adaa99ddd5e103f310fe461b2b53d6eaab5e022a22`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ace878b15edfb608ab92fa81107f69cd2c890e1eaec38702cc19dc7a59a74d`  
		Last Modified: Tue, 13 Jun 2023 04:30:46 GMT  
		Size: 114.5 MB (114545124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:434f6d6881ff88ff4b7cee78c77fa384e4a87c18fe0a202ca11474201e233f59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:ad5059312602da31f495de528acd61a02792211ba7f6afe6a237c28c2bd83dc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **603.7 MB (603693681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72fe6db03b9bb80cb21f732d449caa760ac83ffeb0ffe2dbd730f5021c5e724b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:21 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 07:09:22 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:22 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 07:09:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:39 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:39 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:39 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:39 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:39 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:40 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99699bd121b4a8e64f15735f4d0ef691635afc9777ee9e5b73073c94a8214638`  
		Last Modified: Tue, 13 Jun 2023 07:10:52 GMT  
		Size: 3.9 KB (3851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5059e97d213de7dade187caa587fceb9b23f57db3e6caf64e09af2c39f35ce`  
		Last Modified: Tue, 13 Jun 2023 07:10:53 GMT  
		Size: 8.8 KB (8767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14dbbfd6f8869fa267d5919c8ecbacdbb013106b99f179b389e724d5f3c8822`  
		Last Modified: Tue, 13 Jun 2023 07:11:07 GMT  
		Size: 379.7 MB (379683265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:beed155222ae1f4e0863bc0ec29c3f77b3f17318a4ffe2ec101f2a6864c79e94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **601.0 MB (601004543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bc60798e3794bc19227cce0943e89daf6c16c55acda863d78b4888b091dbd60`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:29:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=851d82c37c2d90784a5a2382880935d09b0784a6d2ea16c1062a6191ccd34c98 NEO4J_TARBALL=neo4j-enterprise-5.8.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:29:10 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 04:29:11 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:29:11 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 04:29:38 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:29:40 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:29:40 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:29:40 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:29:41 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:29:41 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:41 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8c0f56f0edd204dd07e721377ffe1fa3b4a6593019f5e83dff05ada292b3e7`  
		Last Modified: Tue, 13 Jun 2023 04:31:15 GMT  
		Size: 3.9 KB (3883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf3f09cefbb2f5fd58d3a43b66da125f5d716a929f6b7631f83f886f3da76dc`  
		Last Modified: Tue, 13 Jun 2023 04:31:15 GMT  
		Size: 8.8 KB (8769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db23f413388e2fc9cdda0c1b366db473e92dd32bbb3bd89de28cc9a2356acb2`  
		Last Modified: Tue, 13 Jun 2023 04:31:27 GMT  
		Size: 379.5 MB (379541351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `neo4j:latest`

```console
$ docker pull neo4j@sha256:3bf8dbbda1ef52063693b245c06bf5e9d2768195f082b1b1aed9933475470540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:dc272726680f27f10425e6697cc405103478e358968976515aadfa11b319cbd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.7 MB (338698875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad022bbe615bdf0661ab86f40e73af636e0c6e870e3c60d844b9562397fbefc`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:44:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 03:50:15 GMT
COPY dir:3373f6afb162f98a7f4cbaf8f00acdb618287ff4fa7a1aab9b85d36a1c441565 in /opt/java/openjdk 
# Tue, 13 Jun 2023 07:09:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 07:09:01 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 07:09:01 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 07:09:02 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 07:09:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:09:15 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:09:15 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 07:09:15 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 07:09:15 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 07:09:16 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 07:09:16 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bb32e3062db1c890af593910b7980b172f50d98a42b947310bdadd85c41440`  
		Last Modified: Tue, 13 Jun 2023 03:59:06 GMT  
		Size: 192.6 MB (192580388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8134a37330edefa0a033fee2d31970e964caeab4aa96bb417e63fb3c0a8e14c`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 3.9 KB (3853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a384b9f2bbf845f7870bc14fa917d7af3ee40d6142a2610c7ed042beb35caaab`  
		Last Modified: Tue, 13 Jun 2023 07:10:29 GMT  
		Size: 8.8 KB (8766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9cca560702bb0d53e76d67b7c780c1a7a368d00966c9fd3074d917380e1fd11`  
		Last Modified: Tue, 13 Jun 2023 07:10:35 GMT  
		Size: 114.7 MB (114688458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:7dd07e2a806fc23110252785bf391d326ae3302b5398dbddace99dd805c6c16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (336008316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e89cfbba3028caa9c5f7c9e882d0e9b7e5c040d9299cde2c1f91b23816d1191`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:28:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 13 Jun 2023 04:28:50 GMT
COPY dir:61701986201ad0602f1c757565ae6dd6ea34364a0201d8cacf0d9cb6de78ccff in /opt/java/openjdk 
# Tue, 13 Jun 2023 04:28:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=96d728c337804a255151c23ced29994a890ee4d4015fa3916e34a358f0d1cbd6 NEO4J_TARBALL=neo4j-community-5.8.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Tue, 13 Jun 2023 04:28:54 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
# Tue, 13 Jun 2023 04:28:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Tue, 13 Jun 2023 04:28:55 GMT
COPY multi:3bc0fa696e81224d7ba1974735ef93fe90797d02a5971b859ddbbdf878ae6a57 in /startup/ 
# Tue, 13 Jun 2023 04:29:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.8.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:29:06 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:29:07 GMT
WORKDIR /var/lib/neo4j
# Tue, 13 Jun 2023 04:29:07 GMT
VOLUME [/data /logs]
# Tue, 13 Jun 2023 04:29:07 GMT
EXPOSE 7473 7474 7687
# Tue, 13 Jun 2023 04:29:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:29:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44f1d77eefd6a268a661d8baa5ffc1f6d77b6b4e27e034496d0fb5928e86485`  
		Last Modified: Tue, 13 Jun 2023 04:30:57 GMT  
		Size: 191.4 MB (191387706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0a981bd793b3c89ab46f2f6bd1114add130d3116491701e31f0d53f8f12fc7`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 3.9 KB (3882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b539f80e3d71c865200143adaa99ddd5e103f310fe461b2b53d6eaab5e022a22`  
		Last Modified: Tue, 13 Jun 2023 04:30:41 GMT  
		Size: 8.8 KB (8770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ace878b15edfb608ab92fa81107f69cd2c890e1eaec38702cc19dc7a59a74d`  
		Last Modified: Tue, 13 Jun 2023 04:30:46 GMT  
		Size: 114.5 MB (114545124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
