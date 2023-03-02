## `neo4j:enterprise`

```console
$ docker pull neo4j@sha256:9b4be4cf76fb6a59da2a7101c669679553e22d0500cb93a0bbf50b67df984475
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neo4j:enterprise` - linux; amd64

```console
$ docker pull neo4j@sha256:e6bc6a29ddf9ea2c569de646c4a6f6e771c8d17084ce01ffea9eb3b8df80b87f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.0 MB (543986287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5beac6477ea0dec6914fe01a6578c198ae2a20639c027a477f3319de0545e751`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:41:22 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Mar 2023 07:47:19 GMT
COPY dir:5cf52f938fe415b0022fbccb8cf978562c503c0b8313cc9dedf46c1c4edb35cf in /opt/java/openjdk 
# Wed, 01 Mar 2023 08:20:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Wed, 01 Mar 2023 08:20:19 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Wed, 01 Mar 2023 08:20:20 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Wed, 01 Mar 2023 08:20:20 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Wed, 01 Mar 2023 08:20:46 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 08:20:46 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 08:20:47 GMT
WORKDIR /var/lib/neo4j
# Wed, 01 Mar 2023 08:20:47 GMT
VOLUME [/data /logs]
# Wed, 01 Mar 2023 08:20:47 GMT
EXPOSE 7473 7474 7687
# Wed, 01 Mar 2023 08:20:47 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 08:20:47 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f039bcab9992b3a477fd101e656d4f5ad27c8c30323fd021475c390e3d41213e`  
		Last Modified: Wed, 01 Mar 2023 07:58:57 GMT  
		Size: 192.4 MB (192438214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca1af8f3a01f7749b92769536fc106427a633bb36190683b234dc4330400267`  
		Last Modified: Wed, 01 Mar 2023 08:22:20 GMT  
		Size: 3.9 KB (3859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0f676aae6225fe504ac8fdd5d213beb9b530c89a678f4b9919bd61b34379a7`  
		Last Modified: Wed, 01 Mar 2023 08:22:20 GMT  
		Size: 8.4 KB (8422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3612cb7eb7eb0aed8e3a57e41fe69f415ca2f97e5b1ecd345f887259581594d`  
		Last Modified: Wed, 01 Mar 2023 08:22:33 GMT  
		Size: 320.1 MB (320124389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neo4j:enterprise` - linux; arm64 variant v8

```console
$ docker pull neo4j@sha256:1c72e0fd371f9c714089012adcf6c98ed8080f4deff364d7a44de73ff3461adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.3 MB (541317672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a8986d4118bbbad30dc006f061f1a1a5b0a87432c21eec2616480cf9d2d62c`
-	Entrypoint: `["tini","-g","--","\/startup\/docker-entrypoint.sh"]`
-	Default Command: `["neo4j"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:02:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 07:07:04 GMT
COPY dir:47c117bbc947c5c1164b5a20eeec0ba16c306f5991a85f22c54db31ca24ce4a8 in /opt/java/openjdk 
# Thu, 02 Mar 2023 07:36:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin NEO4J_SHA256=4e7a26d5ed0a89fce2c7f94dc756586f0e666f7d756e3fd1c4a0fddea98bfa46 NEO4J_TARBALL=neo4j-enterprise-5.5.0-unix.tar.gz NEO4J_EDITION=enterprise NEO4J_HOME=/var/lib/neo4j
# Thu, 02 Mar 2023 07:36:51 GMT
ARG NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
# Thu, 02 Mar 2023 07:36:52 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN addgroup --gid 7474 --system neo4j && adduser --uid 7474 --system --no-create-home --home "${NEO4J_HOME}" --ingroup neo4j neo4j
# Thu, 02 Mar 2023 07:36:52 GMT
COPY multi:0673d6d1ec30168cf718a05272e8f73bf29e38f3da625fb17d18eb955eb48a71 in /startup/ 
# Thu, 02 Mar 2023 07:37:15 GMT
# ARGS: NEO4J_URI=https://dist.neo4j.org/neo4j-enterprise-5.5.0-unix.tar.gz
RUN apt update     && apt install -y curl gosu jq tini wget     && curl --fail --silent --show-error --location --remote-name ${NEO4J_URI}     && echo "${NEO4J_SHA256}  ${NEO4J_TARBALL}" | sha256sum -c --strict --quiet     && tar --extract --file ${NEO4J_TARBALL} --directory /var/lib     && mv /var/lib/neo4j-* "${NEO4J_HOME}"     && rm ${NEO4J_TARBALL}     && mv "${NEO4J_HOME}"/data /data     && mv "${NEO4J_HOME}"/logs /logs     && chown -R neo4j:neo4j /data     && chmod -R 777 /data     && chown -R neo4j:neo4j /logs     && chmod -R 777 /logs     && chown -R neo4j:neo4j "${NEO4J_HOME}"     && chmod -R 777 "${NEO4J_HOME}"     && ln -s /data "${NEO4J_HOME}"/data     && ln -s /logs "${NEO4J_HOME}"/logs     && apt-get -y purge --auto-remove curl     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:37:17 GMT
ENV PATH=/var/lib/neo4j/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:37:17 GMT
WORKDIR /var/lib/neo4j
# Thu, 02 Mar 2023 07:37:17 GMT
VOLUME [/data /logs]
# Thu, 02 Mar 2023 07:37:17 GMT
EXPOSE 7473 7474 7687
# Thu, 02 Mar 2023 07:37:17 GMT
ENTRYPOINT ["tini" "-g" "--" "/startup/docker-entrypoint.sh"]
# Thu, 02 Mar 2023 07:37:17 GMT
CMD ["neo4j"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee2a535b626ac45b3b701a33ede28cb7ec44388615e651313d6818cbca5d626`  
		Last Modified: Thu, 02 Mar 2023 07:20:21 GMT  
		Size: 191.3 MB (191260449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e67562eaa79cf5c3d0c20d52a796769a8e752042a88822c034467fde45f9f`  
		Last Modified: Thu, 02 Mar 2023 07:38:39 GMT  
		Size: 3.9 KB (3887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b373918e7ca45f4b0a3e6774b789a7119c3b3f11bf8a31a4bffb5eedd5ba0983`  
		Last Modified: Thu, 02 Mar 2023 07:38:39 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f830c2b3bca661c9eb4fa6b1c768bc4c8a9c06f9edfdc18d2c1efa5f7ebf6f`  
		Last Modified: Thu, 02 Mar 2023 07:38:51 GMT  
		Size: 320.0 MB (319982101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
