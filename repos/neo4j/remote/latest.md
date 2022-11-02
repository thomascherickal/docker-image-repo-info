## `neo4j:latest`

```console
$ docker pull neo4j@sha256:fc99f5721a0badff3376526670a25a71f524dabb48f19ca383c1d2ff5db3c9b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:latest` - linux; amd64

```console
$ docker pull neo4j@sha256:b780c8381e7f1ab5ca8fe737276dbefbe7525bbd31cdc009b5d3810938dcba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334277794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b92f0b7f95023408457dd46c1832f690f17828af1ec34a4a2b5328f2f2e0ce`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:33:26 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:15:23 GMT
COPY dir:58adc2a0817e042696a68e5783ea1d9db89b18bd838f66f2ddc3c99acbc84106 in /opt/java/openjdk 
# Wed, 02 Nov 2022 20:53:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 20:53:40 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 20:53:41 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 20:53:41 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 20:53:54 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 20:53:55 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 20:53:55 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 20:53:55 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 20:53:55 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 20:53:55 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 20:53:55 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9b9477aacca86981c880c8ed7c4dbb56574cdcda91a39effa9c2332b96765`  
		Last Modified: Wed, 02 Nov 2022 20:27:47 GMT  
		Size: 192.1 MB (192137557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3112b4ae6e1a6961c3b59de4b733095baef2a2ac136c1fad7d9c2ae6c42492d`  
		Last Modified: Wed, 02 Nov 2022 20:56:11 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c89cfb52d22682f78babb4c91e0091ab16e91e38a29acbcc8a924c6e0a2059`  
		Last Modified: Wed, 02 Nov 2022 20:56:12 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129efcacc87bccae32585727944036d41362d927953efc157220609baa63f6ec`  
		Last Modified: Wed, 02 Nov 2022 20:56:18 GMT  
		Size: 110.7 MB (110708707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:latest` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:26c2bac6ae0667ebbae325805848a20b6037c7ed6d450190d97db28091be20b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.5 MB (331545745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86073f4afd276e313eac90b043f954f932c77e8eb1a843a26bfdc24206cbcb9b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 20:50:40 GMT
COPY dir:527d7e3a362e3a52ce4ecffbf599fb9423f60f5fcdccc64d800fcfec8666f5b8 in /opt/java/openjdk 
# Wed, 02 Nov 2022 21:26:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=c8086d1f8558376754e7248a7d12838f024ca2699aa59e0aba30816b229ed4f4 NEO4J_TARBALL=neo4j-community-5.1.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
# Wed, 02 Nov 2022 21:26:19 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 02 Nov 2022 21:26:19 GMT
COPY multi:a11635e58e35f289c454771630762b2132b546d160631e2fe7ed78f034b4cc21 in /startup/ 
# Wed, 02 Nov 2022 21:26:29 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.1.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Nov 2022 21:26:29 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 21:26:29 GMT
WORKDIR /var/lib/neo4j
# Wed, 02 Nov 2022 21:26:29 GMT
VOLUME [/data /logs]
# Wed, 02 Nov 2022 21:26:30 GMT
EXPOSE 7473 7474 7687
# Wed, 02 Nov 2022 21:26:30 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 02 Nov 2022 21:26:30 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23c78a656ff98cd4a277e3c01f4d0eb067085f7d111e0f4a4c913c75ed384c0`  
		Last Modified: Wed, 02 Nov 2022 21:01:35 GMT  
		Size: 190.9 MB (190904092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449edc3d08e467ce37d14ad7fa99aac6b03a0517ba1199eff5c63e54cf7add1c`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b0f871a10e6921abeb9ee66ec6092c30fca9379c1f7f428047eb46ff850cf`  
		Last Modified: Wed, 02 Nov 2022 21:27:42 GMT  
		Size: 7.6 KB (7632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c44bbd671eb7f05a3596c9a2ed39098a38c3b7ec17520fcd09550a3cec5fd`  
		Last Modified: Wed, 02 Nov 2022 21:27:47 GMT  
		Size: 110.6 MB (110566224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
