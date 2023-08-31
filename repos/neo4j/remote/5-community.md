## `neo4j:5-community`

```console
$ docker pull neo4j@sha256:3452812fa1986f3c17eca6fb8c7ccf5c6ce71a9c985bf73f4e377a50568c47f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-community` - linux; amd64

```console
$ docker pull neo4j@sha256:9a39fb3df061a082bf400507f857ffd78af2e7ac39bf3964b3e9df9ddbea4dac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293722286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db463f6cc7764a98a89c21226b932f481a609ed66efcf540cd6c05f8548ed6b`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 31 Aug 2023 20:48:51 GMT
COPY dir:6777d1f77166c2ecdd8f4eb23f5fd82574aa8a90fd65d6dff981fbb31778a3d1 in /opt/java/openjdk 
# Thu, 31 Aug 2023 20:48:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 31 Aug 2023 20:48:52 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 31 Aug 2023 20:48:53 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 31 Aug 2023 20:48:53 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 31 Aug 2023 20:49:06 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Aug 2023 20:49:07 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 20:49:07 GMT
WORKDIR /var/lib/neo4j
# Thu, 31 Aug 2023 20:49:07 GMT
VOLUME [/data /logs]
# Thu, 31 Aug 2023 20:49:07 GMT
EXPOSE 7473 7474 7687
# Thu, 31 Aug 2023 20:49:07 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 31 Aug 2023 20:49:07 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65006a4851e206ccc53a9bf891b081e6fefbdbe0fcb897d670970fc7f2eff9ea`  
		Last Modified: Thu, 31 Aug 2023 20:51:41 GMT  
		Size: 144.8 MB (144775820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c565599f1dc1ddf97deb3cc8e05ab94f2057bf0398afc2cbdadc75350bc9f77b`  
		Last Modified: Thu, 31 Aug 2023 20:51:29 GMT  
		Size: 3.9 KB (3863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4b4f83dfc50acec6110f72c3d3d4470034c0c4a212b82659c59afe6a94ecf8`  
		Last Modified: Thu, 31 Aug 2023 20:51:29 GMT  
		Size: 9.3 KB (9345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1aabf964f5b827b641a2f7fd4843589e5ccd89491ba1ea623ff3d6b6d4041f`  
		Last Modified: Thu, 31 Aug 2023 20:51:36 GMT  
		Size: 117.5 MB (117515580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-community` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:74f04472ca76e214b38413f9279ab38e560f06ef423605e7591494f939f26b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291022736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7035a56efda51b7c25845c37e854a1725379b06089d1dccd720a3ef570e8f6c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 17:25:53 GMT
COPY dir:5a6bdf68753afdd79dcc6e0d47fad53f85321d9f35fef7ea9a683b5f91d77eec in /opt/java/openjdk 
# Thu, 17 Aug 2023 01:25:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=3a206271d01ff337ab64e99a9ea90b17733416ec17c093b5be7bfb9342b0dacd NEO4J_TARBALL=neo4j-community-5.11.0-unix.tar.gz NEO4J_EDITION=community NEO4J_HOME=/var/lib/neo4j
# Thu, 17 Aug 2023 01:25:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
# Thu, 17 Aug 2023 01:25:39 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 17 Aug 2023 01:25:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Thu, 17 Aug 2023 01:25:51 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-community-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:25:52 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 01:25:52 GMT
WORKDIR /var/lib/neo4j
# Thu, 17 Aug 2023 01:25:52 GMT
VOLUME [/data /logs]
# Thu, 17 Aug 2023 01:25:52 GMT
EXPOSE 7473 7474 7687
# Thu, 17 Aug 2023 01:25:52 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 17 Aug 2023 01:25:52 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e1713a1018eae13a831df1ed9b8fd5e8788a4ef59b3f122c903b9e1c2857b`  
		Last Modified: Wed, 16 Aug 2023 17:34:20 GMT  
		Size: 143.5 MB (143538106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c45056d1f2d245cc4191f75a1c781742c9ef7c945ce0eb49741ff03afd7d5`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd67db71629e8e1e567670cc55d5b342eb40c6ae2dabe9876ad7ec90888abb6`  
		Last Modified: Thu, 17 Aug 2023 01:27:35 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fc6630778fadae75a2193c0fab3b707927f5b9701ba797b5bfd5b627c3d6`  
		Last Modified: Thu, 17 Aug 2023 01:27:42 GMT  
		Size: 117.4 MB (117408576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
