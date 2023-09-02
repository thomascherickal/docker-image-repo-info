## `neo4j:5-enterprise-bullseye`

```console
$ docker pull neo4j@sha256:ff1e26fd1fc337775d677d807e23a755fa7adfd24073cee59a140778866f8dd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:5-enterprise-bullseye` - linux; amd64

```console
$ docker pull neo4j@sha256:f7428228aa7405664df091327843cfd6525ec7fb6bc16a42598a215b8b5a5a38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579906808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ca685150fcf5161ecd1cbcfae4df5a7f42069888792f45fcd99fb59a0553f5`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:55 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 02:46:18 GMT
COPY dir:61bbef45bd137d5078f6a6f774d9bc49d275ae5fe27274294232d075ae1a5bf2 in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:46:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Sep 2023 02:46:39 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Sat, 02 Sep 2023 02:46:40 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Sep 2023 02:46:40 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Sat, 02 Sep 2023 02:46:59 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 02:46:59 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 02:46:59 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Sep 2023 02:47:00 GMT
VOLUME [/data /logs]
# Sat, 02 Sep 2023 02:47:00 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Sep 2023 02:47:00 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Sep 2023 02:47:00 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d4946b1998501e173a27b5106ab354beefe3a0cead8354e4f41fc3bc266f22`  
		Last Modified: Sat, 02 Sep 2023 02:48:51 GMT  
		Size: 144.8 MB (144775778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72cbb8ac4acc0a221d8f8167ac7a6575056bafca264d337effb783712940b46`  
		Last Modified: Sat, 02 Sep 2023 02:49:23 GMT  
		Size: 3.9 KB (3860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5074e388b1e9b7dc7c82720092a4d0bf552179e02de9fabead9049f6e2fba20e`  
		Last Modified: Sat, 02 Sep 2023 02:49:23 GMT  
		Size: 9.4 KB (9351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c2e6c278c94b4cbb69509a409ba326982431e1c9923638afd0286cddecbd47`  
		Last Modified: Sat, 02 Sep 2023 02:49:40 GMT  
		Size: 403.7 MB (403700141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:5-enterprise-bullseye` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:a36ea8716306d2ac82e63cd7b645297d17d68119f0483476baaee726f7b16228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **577.2 MB (577211386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e653846987a9d18250f5a4734bd51e34f3b186cfc5e78b358996bf021e4d6d`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 01:48:00 GMT
COPY dir:ffc7dc4725a3524e0b294e59a90d1e58e69ec448374b50aef6bef0cfa219cb0f in /opt/java/openjdk 
# Sat, 02 Sep 2023 02:38:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=0de7579b9b307dbd24793368415ccac799911705ede4a8f70275e4b4eb94c05c NEO4J_TARBALL=neo4j-enterprise-5.11.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Sat, 02 Sep 2023 02:38:59 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
# Sat, 02 Sep 2023 02:39:00 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Sat, 02 Sep 2023 02:39:00 GMT
COPY multi:d939a3d156891be9a8e359f0c5c2adbad24c093f1ca53494ce82d0acd2b2613d in /startup/ 
# Sat, 02 Sep 2023 02:39:18 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.11.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq procps tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && mv /startup/neo4j-admin-report.sh "${NEO4J_HOME}"/bin/neo4j-admin-report     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 02:39:20 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 02:39:20 GMT
WORKDIR /var/lib/neo4j
# Sat, 02 Sep 2023 02:39:20 GMT
VOLUME [/data /logs]
# Sat, 02 Sep 2023 02:39:21 GMT
EXPOSE 7473 7474 7687
# Sat, 02 Sep 2023 02:39:21 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Sat, 02 Sep 2023 02:39:21 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75390d7bc4a96162e240272aeff28881955f7af498179aa85faecd879748f913`  
		Last Modified: Sat, 02 Sep 2023 01:55:46 GMT  
		Size: 143.5 MB (143543515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763af09bb41dc8d87316dced3fb9254d518eaa856dac78aacdeea77ba0f76c4c`  
		Last Modified: Sat, 02 Sep 2023 02:41:38 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338e19d97f77ce1f0c1fe3252496a3f7ad8494c3c83e2824a78994b0e7549456`  
		Last Modified: Sat, 02 Sep 2023 02:41:38 GMT  
		Size: 9.3 KB (9349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a53d7ef2ad80e8b196413f350945ccaf481ce52cdca436ef14ef5aefde49f2`  
		Last Modified: Sat, 02 Sep 2023 02:41:53 GMT  
		Size: 403.6 MB (403591816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
