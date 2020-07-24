<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `open-liberty`

-	[`open-liberty:20.0.0.3-full-java8-openj9`](#open-liberty20003-full-java8-openj9)
-	[`open-liberty:20.0.0.3-kernel-java8-openj9`](#open-liberty20003-kernel-java8-openj9)
-	[`open-liberty:20.0.0.6-full-java8-openj9`](#open-liberty20006-full-java8-openj9)
-	[`open-liberty:20.0.0.6-kernel-java8-openj9`](#open-liberty20006-kernel-java8-openj9)
-	[`open-liberty:20.0.0.7-full-java8-openj9`](#open-liberty20007-full-java8-openj9)
-	[`open-liberty:20.0.0.7-kernel-java8-openj9`](#open-liberty20007-kernel-java8-openj9)
-	[`open-liberty:full`](#open-libertyfull)
-	[`open-liberty:full-java8-openj9`](#open-libertyfull-java8-openj9)
-	[`open-liberty:kernel`](#open-libertykernel)
-	[`open-liberty:kernel-java8-openj9`](#open-libertykernel-java8-openj9)
-	[`open-liberty:latest`](#open-libertylatest)

## `open-liberty:20.0.0.3-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:307e28950ca3389e5f3abe53076dc52222ad0c7f7add738affe26971f7ae7da4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:71dc5369e55114b7029a525a950d38322a6291c470ee39b6f95df71071f4b35d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.8 MB (252828256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd69af0fb30304b838013f40f963db0e0b082df7090cc1ee30f26237b29b8b7a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:56:00 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 17 Jul 2020 22:56:00 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 17 Jul 2020 22:56:01 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 17 Jul 2020 22:56:01 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 17 Jul 2020 22:56:01 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:56:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Fri, 17 Jul 2020 22:56:01 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:56:02 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:56:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:56:13 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:56:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:56:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:56:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:56:36 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:56:36 GMT
USER 1001
# Fri, 17 Jul 2020 22:56:36 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:56:36 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:56:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:56:48 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f98f54810e854ecb60f31726e9cccf3fb615a73d9910ece25e74b1bbae8d54`  
		Last Modified: Fri, 17 Jul 2020 22:57:40 GMT  
		Size: 6.5 KB (6520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dbc3f99f4ad350bca19737fd57cf81b0f2c04631ff774db1292f9fee411cb3`  
		Last Modified: Fri, 17 Jul 2020 22:57:40 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a56a45917d6e0c378373f112b8a0df6241b298bab057c329cbc98d038c41abd`  
		Last Modified: Fri, 17 Jul 2020 22:57:49 GMT  
		Size: 155.1 MB (155084321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4524c1be43b417f3cf8d33e94586aedd087d51d849e7f7cdc6971e44ba4eb1c4`  
		Last Modified: Fri, 17 Jul 2020 22:57:39 GMT  
		Size: 934.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef1d42e5ac14b9c687e2d6ae4e43f100ea955ca0b89854b3b1d49b909455f2a`  
		Last Modified: Fri, 17 Jul 2020 22:57:39 GMT  
		Size: 7.5 KB (7548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a0d9bc818691b6d0a9a9ba4993d84ebf798f69c111bfaecf565c95ad337bd`  
		Last Modified: Fri, 17 Jul 2020 22:57:42 GMT  
		Size: 8.4 MB (8428718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649f88c91d9bbb9feda6da2cb3299b4798be00a8ef34460deb7f452b81d978a3`  
		Last Modified: Fri, 17 Jul 2020 22:57:55 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:141677bb880fda2c23cb4ca88a7cf7400bbbc8b3fe8a69b207a413dbcd0af668
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256105351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2844f23c332e6cf397b259f2fff13cf3ecd465224ad59a4b1df913446e03e95a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:12:44 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Sat, 18 Jul 2020 02:12:54 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Sat, 18 Jul 2020 02:13:09 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Sat, 18 Jul 2020 02:13:18 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Sat, 18 Jul 2020 02:13:34 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:13:47 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Sat, 18 Jul 2020 02:13:50 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:13:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:14:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:14:53 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:15:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:15:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:16:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:16:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:16:52 GMT
USER 1001
# Sat, 18 Jul 2020 02:16:57 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:16:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:17:05 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:17:26 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b24d4ba2d4f44b5f278a3126b13feac6bf05d7cf22285f25cedf2655f082a`  
		Last Modified: Sat, 18 Jul 2020 02:19:30 GMT  
		Size: 6.5 KB (6547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ca09bf893ec44e0ce7f13c819541053854a584e2e95012073046306e1565d`  
		Last Modified: Sat, 18 Jul 2020 02:19:27 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c78e1fc309a7f98873cfec1eff5b0a7346472bd5b88794b1783eaa0d3240fa`  
		Last Modified: Sat, 18 Jul 2020 02:19:39 GMT  
		Size: 155.1 MB (155085697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b03e6fecfa2e5bc8e8ba178afe8b9b207be1237059d16d7821d5b2d9889426`  
		Last Modified: Sat, 18 Jul 2020 02:19:27 GMT  
		Size: 1.0 KB (1005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9bc193965f4fe128a0c4365a4f1e618960b874303f9694836d5530e6c1f08`  
		Last Modified: Sat, 18 Jul 2020 02:19:26 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d039835b7e465c4eb805d091240d98d715692a5c3c8ea5d148a6d8216a9ec61`  
		Last Modified: Sat, 18 Jul 2020 02:19:28 GMT  
		Size: 6.9 MB (6894423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5e8c4c696082aabf083516897eac22153d72e81dd43dea2dfd08baf1d25d2`  
		Last Modified: Sat, 18 Jul 2020 02:19:49 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:5dbbf5d0d1e2fff99026fbbc684317c3c7756e1e74ccd6da7fc21beac5263f97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.7 MB (250715176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68bb43d51ce8bacb8a07c921fa6e4ffdb54400a1e2adfb0f4a252af2ed62e285`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:37:06 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 24 Jul 2020 17:37:06 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 24 Jul 2020 17:37:06 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 24 Jul 2020 17:37:07 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 24 Jul 2020 17:37:07 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:37:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Fri, 24 Jul 2020 17:37:07 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:37:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:37:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:37:22 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:37:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:37:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:37:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:37:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:37:35 GMT
USER 1001
# Fri, 24 Jul 2020 17:37:35 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:37:36 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:37:36 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:37:42 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdbfee9880c5e41794a1ca65edc0a01b942f32e927b4481f7fdb11bd7ab79ca`  
		Last Modified: Fri, 24 Jul 2020 17:38:46 GMT  
		Size: 6.5 KB (6546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74acede404ebf1a4b9981bed002766538fdaabbcc4c4d51de74bc153538c7ed`  
		Last Modified: Fri, 24 Jul 2020 17:38:44 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bd03a0059228291798592da0b97c71d2b91b2092db1a21364cb7beb961abab`  
		Last Modified: Fri, 24 Jul 2020 17:38:52 GMT  
		Size: 155.1 MB (155084786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9693f928dcee984456fc8517688c9b142be7175c7db08e1bfa66141ba7cef86`  
		Last Modified: Fri, 24 Jul 2020 17:38:44 GMT  
		Size: 996.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffefb9990bc9c50a133ba9e64836214f713d56290373c56af50fe70c97a05a`  
		Last Modified: Fri, 24 Jul 2020 17:38:45 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c519bf2dd207613215153e0b3d249eb5d6261535f7f6a2eb754eaab3d654ddb0`  
		Last Modified: Fri, 24 Jul 2020 17:38:45 GMT  
		Size: 8.2 MB (8224263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efacee10bc7cd93cabbefb6544194921644e117a6be3a5a25718b165c8db1438`  
		Last Modified: Fri, 24 Jul 2020 17:38:57 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.3-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:64fabb56ba9c9b1264c01c53dce82c3a17f1c5d85b4e3e6206dfcb457beb999b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:7c773037d384c1c70f7290f0995f51f415238fbb70433de441465695080f579d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.8 MB (252827293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2beda37051c40d4b58ca25e6988b8f4db7c26f8988cfedc9619d95c0bd573f6e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:56:00 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 17 Jul 2020 22:56:00 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 17 Jul 2020 22:56:01 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 17 Jul 2020 22:56:01 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 17 Jul 2020 22:56:01 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:56:01 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Fri, 17 Jul 2020 22:56:01 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:56:02 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:56:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:56:13 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:56:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:56:15 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:56:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:56:36 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:56:36 GMT
USER 1001
# Fri, 17 Jul 2020 22:56:36 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:56:36 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:56:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f98f54810e854ecb60f31726e9cccf3fb615a73d9910ece25e74b1bbae8d54`  
		Last Modified: Fri, 17 Jul 2020 22:57:40 GMT  
		Size: 6.5 KB (6520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dbc3f99f4ad350bca19737fd57cf81b0f2c04631ff774db1292f9fee411cb3`  
		Last Modified: Fri, 17 Jul 2020 22:57:40 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a56a45917d6e0c378373f112b8a0df6241b298bab057c329cbc98d038c41abd`  
		Last Modified: Fri, 17 Jul 2020 22:57:49 GMT  
		Size: 155.1 MB (155084321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4524c1be43b417f3cf8d33e94586aedd087d51d849e7f7cdc6971e44ba4eb1c4`  
		Last Modified: Fri, 17 Jul 2020 22:57:39 GMT  
		Size: 934.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef1d42e5ac14b9c687e2d6ae4e43f100ea955ca0b89854b3b1d49b909455f2a`  
		Last Modified: Fri, 17 Jul 2020 22:57:39 GMT  
		Size: 7.5 KB (7548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a0d9bc818691b6d0a9a9ba4993d84ebf798f69c111bfaecf565c95ad337bd`  
		Last Modified: Fri, 17 Jul 2020 22:57:42 GMT  
		Size: 8.4 MB (8428718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:92124b7406e665f1460d7b54876d63a73ca3b193e1d6d83f3a164e6d67945cd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256104385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d18c0b0f033d88352b1638e5d84645c18aadac62766739582bb9d3f0046ebd5`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:12:44 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Sat, 18 Jul 2020 02:12:54 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Sat, 18 Jul 2020 02:13:09 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Sat, 18 Jul 2020 02:13:18 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Sat, 18 Jul 2020 02:13:34 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:13:47 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Sat, 18 Jul 2020 02:13:50 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:13:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:14:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:14:53 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:15:05 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:15:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:16:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:16:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:16:52 GMT
USER 1001
# Sat, 18 Jul 2020 02:16:57 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:16:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:17:05 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89b24d4ba2d4f44b5f278a3126b13feac6bf05d7cf22285f25cedf2655f082a`  
		Last Modified: Sat, 18 Jul 2020 02:19:30 GMT  
		Size: 6.5 KB (6547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0ca09bf893ec44e0ce7f13c819541053854a584e2e95012073046306e1565d`  
		Last Modified: Sat, 18 Jul 2020 02:19:27 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c78e1fc309a7f98873cfec1eff5b0a7346472bd5b88794b1783eaa0d3240fa`  
		Last Modified: Sat, 18 Jul 2020 02:19:39 GMT  
		Size: 155.1 MB (155085697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b03e6fecfa2e5bc8e8ba178afe8b9b207be1237059d16d7821d5b2d9889426`  
		Last Modified: Sat, 18 Jul 2020 02:19:27 GMT  
		Size: 1.0 KB (1005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9bc193965f4fe128a0c4365a4f1e618960b874303f9694836d5530e6c1f08`  
		Last Modified: Sat, 18 Jul 2020 02:19:26 GMT  
		Size: 7.7 KB (7662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d039835b7e465c4eb805d091240d98d715692a5c3c8ea5d148a6d8216a9ec61`  
		Last Modified: Sat, 18 Jul 2020 02:19:28 GMT  
		Size: 6.9 MB (6894423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.3-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:d7c8ea22a41ad13786a8b47546979d411c157945e4adc8856867c3ed4194d5ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.7 MB (250714213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75e176e7e1bd8bf0270b648edfe935fd29c7d286ef68f4b6dcc64a1b8aeee8c`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:37:06 GMT
ARG LIBERTY_VERSION=20.0.0.3
# Fri, 24 Jul 2020 17:37:06 GMT
ARG LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db
# Fri, 24 Jul 2020 17:37:06 GMT
ARG LIBERTY_BUILD_LABEL=cl200320200305-1433
# Fri, 24 Jul 2020 17:37:07 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip
# Fri, 24 Jul 2020 17:37:07 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:37:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.3
# Fri, 24 Jul 2020 17:37:07 GMT
COPY dir:db13e0b286891a0bd7aa45ab6285056101f78bde154aff1711d0e2933840a07f in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:37:07 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:37:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:37:22 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:37:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:37:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:37:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200320200305-1433 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.3/openliberty-runtime-20.0.0.3.zip LIBERTY_SHA=49180c2cd6ce23f863760d837a4b1663680084db LIBERTY_VERSION=20.0.0.3
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:37:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:37:35 GMT
USER 1001
# Fri, 24 Jul 2020 17:37:35 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:37:36 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:37:36 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdbfee9880c5e41794a1ca65edc0a01b942f32e927b4481f7fdb11bd7ab79ca`  
		Last Modified: Fri, 24 Jul 2020 17:38:46 GMT  
		Size: 6.5 KB (6546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74acede404ebf1a4b9981bed002766538fdaabbcc4c4d51de74bc153538c7ed`  
		Last Modified: Fri, 24 Jul 2020 17:38:44 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bd03a0059228291798592da0b97c71d2b91b2092db1a21364cb7beb961abab`  
		Last Modified: Fri, 24 Jul 2020 17:38:52 GMT  
		Size: 155.1 MB (155084786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9693f928dcee984456fc8517688c9b142be7175c7db08e1bfa66141ba7cef86`  
		Last Modified: Fri, 24 Jul 2020 17:38:44 GMT  
		Size: 996.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ffefb9990bc9c50a133ba9e64836214f713d56290373c56af50fe70c97a05a`  
		Last Modified: Fri, 24 Jul 2020 17:38:45 GMT  
		Size: 7.6 KB (7636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c519bf2dd207613215153e0b3d249eb5d6261535f7f6a2eb754eaab3d654ddb0`  
		Last Modified: Fri, 24 Jul 2020 17:38:45 GMT  
		Size: 8.2 MB (8224263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.6-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:a6833fea852b340b106d955cb5e824675e85b4393b97f562056fd5ee7aa403c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.6-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:6033e26e2e40d038cd1a7338117116c40a3782867a646ef60689f46b24cdda96
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272150362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54372ce342fb47987af81d848dd2f9caf0741bc6bed95f734e7bec888ee2aa4e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:54:39 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Fri, 17 Jul 2020 22:54:40 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Fri, 17 Jul 2020 22:54:40 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Fri, 17 Jul 2020 22:54:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Fri, 17 Jul 2020 22:54:40 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:54:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Fri, 17 Jul 2020 22:54:40 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:54:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:54:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:54:53 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:54:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:54:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:55:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:55:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:55:13 GMT
USER 1001
# Fri, 17 Jul 2020 22:55:13 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:55:13 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:55:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:55:20 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 17 Jul 2020 22:55:50 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00652744eb70f9cb75d725b60f802dec2024e1ecb27b0e814d6cf46e5c35a4eb`  
		Last Modified: Fri, 17 Jul 2020 22:57:21 GMT  
		Size: 8.4 KB (8354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83817042c52882957a822d44960b005acff774efc81fd585fc52b3840759a619`  
		Last Modified: Fri, 17 Jul 2020 22:57:20 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0d2f13a48a72e613a8dc7a8c17a3d32ec3f10f5209183530853c98aefe23a3`  
		Last Modified: Fri, 17 Jul 2020 22:57:30 GMT  
		Size: 157.8 MB (157758230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f540d776fa3dcffcc8e8cdde79f32af6d98c9f555b3dcc1fba720523f22e05`  
		Last Modified: Fri, 17 Jul 2020 22:57:20 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931db93ced61c9bfb9322ca1fa1a07653104a8bb005b751e07be037e788aa923`  
		Last Modified: Fri, 17 Jul 2020 22:57:20 GMT  
		Size: 9.4 KB (9410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87651c1e8db7a9eaaf51605532f7b2025350579e05e73153ffe162e020d46375`  
		Last Modified: Fri, 17 Jul 2020 22:57:21 GMT  
		Size: 8.3 MB (8264669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02be425045b8c01bc8eb00b02f693abc55524d7152a6b0f76f6f41fb0994d40`  
		Last Modified: Fri, 17 Jul 2020 22:57:34 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85de23076a40a043073a2fbb319b75afee25664d3682eb1941b7f2d372caf8a`  
		Last Modified: Fri, 17 Jul 2020 22:57:36 GMT  
		Size: 16.8 MB (16808571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:da22b47f34a12beb0fc6263182a0f05c31474377e4d55468c66907189324eb7b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.3 MB (273322588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdff7c51d91a9bbdc09553b135c709b130977acc9a1c0965d4ec64a75319630e`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:06:21 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Sat, 18 Jul 2020 02:06:26 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Sat, 18 Jul 2020 02:06:32 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Sat, 18 Jul 2020 02:06:42 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Sat, 18 Jul 2020 02:06:47 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:06:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Sat, 18 Jul 2020 02:06:56 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:07:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:09:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:09:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:09:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:09:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:10:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:10:17 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:10:33 GMT
USER 1001
# Sat, 18 Jul 2020 02:10:44 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:10:52 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:10:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:11:22 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 18 Jul 2020 02:12:23 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795bbc64b71223dbec958ea3e886a04f9a1ce0df69247bce5179842c3555b89b`  
		Last Modified: Sat, 18 Jul 2020 02:18:53 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448295d3deae9c98777bbea0c1f3e6516bc3aa40a63858209cb7ac17775e2a1d`  
		Last Modified: Sat, 18 Jul 2020 02:18:49 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426765a2b7ec8a9f8922b67f7f546f135c7f62b2d10b093c2bf6ce9b568bd48`  
		Last Modified: Sat, 18 Jul 2020 02:19:03 GMT  
		Size: 157.8 MB (157759300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb67ae6ebe99b5fc585556759313381e2b3b1c81c53667354976d405ba23cb1`  
		Last Modified: Sat, 18 Jul 2020 02:18:49 GMT  
		Size: 969.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f633f38a4e21564f960a488b77693b36d20b3fbec3cd2d4b4e65d5ef9ed93aff`  
		Last Modified: Sat, 18 Jul 2020 02:18:49 GMT  
		Size: 9.5 KB (9512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e65adf1a8f01bb2d22131ed2541b587f43f829d8fee688dbe518cf449c69b0`  
		Last Modified: Sat, 18 Jul 2020 02:18:51 GMT  
		Size: 6.9 MB (6853894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578bb044cdfc8d42c9f2c52a65cb7becfcfb271231ce019b512096f7ff381278`  
		Last Modified: Sat, 18 Jul 2020 02:19:12 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfac83512aa6da18ceef0f98e6d27ea10f0b529ee4bb0acd0a43007092f38a2a`  
		Last Modified: Sat, 18 Jul 2020 02:19:16 GMT  
		Size: 14.6 MB (14580514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:60dc606795b5d136307c11cf9354ebbda37a3ad39176e99830b1e6e59c2d8c9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268626857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10d9064383c4864de61a0d2e0be89d781a90c97a13f0f3d4742502a39553426f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:36:06 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Fri, 24 Jul 2020 17:36:06 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Fri, 24 Jul 2020 17:36:07 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Fri, 24 Jul 2020 17:36:07 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Fri, 24 Jul 2020 17:36:07 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:36:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Fri, 24 Jul 2020 17:36:07 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:36:08 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:36:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:36:22 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:36:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:36:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:36:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:36:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:36:34 GMT
USER 1001
# Fri, 24 Jul 2020 17:36:34 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:36:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:36:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:36:43 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 24 Jul 2020 17:37:00 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff11c7face9c0891727fd900ff0b7729597f501799e6817982bcdf416db029df`  
		Last Modified: Fri, 24 Jul 2020 17:38:22 GMT  
		Size: 8.4 KB (8379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b123248cb48749dc2e3f1ca4c45c55fbd3f11b78c471cebcf18031bc96b78470`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed88e303b9446e31d2905ee51eace4acdbf43872db0b194c3062f2aec450307`  
		Last Modified: Fri, 24 Jul 2020 17:38:28 GMT  
		Size: 157.8 MB (157758394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08f1fda8f80aaa8c65193f52ba91535890a15bae0a456d01c55b5b8f565527`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 968.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b4931c04889fd45a06eef4c69db92f27fbe88ac6f5034a3b25ed5db8b14b53`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 9.5 KB (9494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af40bc93a666a58e89ff40c24cb7ae845b9a1e9ba2fc55851747f32186177709`  
		Last Modified: Fri, 24 Jul 2020 17:38:22 GMT  
		Size: 7.4 MB (7354989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba41cf1173b1bf68f393004c6b8af1a5da5776b82392005a72cd86fb3dc6236c`  
		Last Modified: Fri, 24 Jul 2020 17:38:36 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44afccd8f57459fc0b1a10848a092fadf9eba1c0ae809dcf88e38e5451928fc`  
		Last Modified: Fri, 24 Jul 2020 17:38:40 GMT  
		Size: 16.1 MB (16103685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.6-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:224bcd4b78037e05a06a97994903577c859d1e5a694e8e0b355467830caf8849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.6-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:90cec38b827e96e8674dfdac403747981b5d17c4afc367b4b1458201074034c4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255340827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6d185350f5a6ff25cf224bf349c5a8900b15a6a165276fd759736f42f393ace`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:54:39 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Fri, 17 Jul 2020 22:54:40 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Fri, 17 Jul 2020 22:54:40 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Fri, 17 Jul 2020 22:54:40 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Fri, 17 Jul 2020 22:54:40 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:54:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Fri, 17 Jul 2020 22:54:40 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:54:41 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:54:52 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:54:53 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:54:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:54:54 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:55:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:55:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:55:13 GMT
USER 1001
# Fri, 17 Jul 2020 22:55:13 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:55:13 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:55:14 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00652744eb70f9cb75d725b60f802dec2024e1ecb27b0e814d6cf46e5c35a4eb`  
		Last Modified: Fri, 17 Jul 2020 22:57:21 GMT  
		Size: 8.4 KB (8354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83817042c52882957a822d44960b005acff774efc81fd585fc52b3840759a619`  
		Last Modified: Fri, 17 Jul 2020 22:57:20 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0d2f13a48a72e613a8dc7a8c17a3d32ec3f10f5209183530853c98aefe23a3`  
		Last Modified: Fri, 17 Jul 2020 22:57:30 GMT  
		Size: 157.8 MB (157758230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f540d776fa3dcffcc8e8cdde79f32af6d98c9f555b3dcc1fba720523f22e05`  
		Last Modified: Fri, 17 Jul 2020 22:57:20 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931db93ced61c9bfb9322ca1fa1a07653104a8bb005b751e07be037e788aa923`  
		Last Modified: Fri, 17 Jul 2020 22:57:20 GMT  
		Size: 9.4 KB (9410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87651c1e8db7a9eaaf51605532f7b2025350579e05e73153ffe162e020d46375`  
		Last Modified: Fri, 17 Jul 2020 22:57:21 GMT  
		Size: 8.3 MB (8264669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:2fbe37b39e9c03ede6c15552aed964f479e9b3c161fecc9e1e74a6a41797f4e2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.7 MB (258741108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6085e4db632129f1bdf304cbb89b9603f1f03548606e1d18ea15700c14d6a345`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:06:21 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Sat, 18 Jul 2020 02:06:26 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Sat, 18 Jul 2020 02:06:32 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Sat, 18 Jul 2020 02:06:42 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Sat, 18 Jul 2020 02:06:47 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:06:52 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Sat, 18 Jul 2020 02:06:56 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:07:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:09:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:09:18 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:09:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:09:40 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:10:09 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:10:17 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:10:33 GMT
USER 1001
# Sat, 18 Jul 2020 02:10:44 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:10:52 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:10:57 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795bbc64b71223dbec958ea3e886a04f9a1ce0df69247bce5179842c3555b89b`  
		Last Modified: Sat, 18 Jul 2020 02:18:53 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448295d3deae9c98777bbea0c1f3e6516bc3aa40a63858209cb7ac17775e2a1d`  
		Last Modified: Sat, 18 Jul 2020 02:18:49 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426765a2b7ec8a9f8922b67f7f546f135c7f62b2d10b093c2bf6ce9b568bd48`  
		Last Modified: Sat, 18 Jul 2020 02:19:03 GMT  
		Size: 157.8 MB (157759300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb67ae6ebe99b5fc585556759313381e2b3b1c81c53667354976d405ba23cb1`  
		Last Modified: Sat, 18 Jul 2020 02:18:49 GMT  
		Size: 969.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f633f38a4e21564f960a488b77693b36d20b3fbec3cd2d4b4e65d5ef9ed93aff`  
		Last Modified: Sat, 18 Jul 2020 02:18:49 GMT  
		Size: 9.5 KB (9512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e65adf1a8f01bb2d22131ed2541b587f43f829d8fee688dbe518cf449c69b0`  
		Last Modified: Sat, 18 Jul 2020 02:18:51 GMT  
		Size: 6.9 MB (6853894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.6-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:40e2ac90a9372401bd51e55ad020ebfe23af070e86c21d2ac0618992feb5a486
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.5 MB (252522210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ca931dcec78db08a91fba9063e2ee6232654cbfd7319dc3c3d9601855558b0`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:36:06 GMT
ARG LIBERTY_VERSION=20.0.0.6
# Fri, 24 Jul 2020 17:36:06 GMT
ARG LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3
# Fri, 24 Jul 2020 17:36:07 GMT
ARG LIBERTY_BUILD_LABEL=cl200620200528-0414
# Fri, 24 Jul 2020 17:36:07 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip
# Fri, 24 Jul 2020 17:36:07 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:36:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.6
# Fri, 24 Jul 2020 17:36:07 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:36:08 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:36:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:36:22 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:36:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:36:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:36:34 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200620200528-0414 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.6/openliberty-runtime-20.0.0.6.zip LIBERTY_SHA=083e89c2f96972df339a513582b338658e6562b3 LIBERTY_VERSION=20.0.0.6
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:36:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:36:34 GMT
USER 1001
# Fri, 24 Jul 2020 17:36:34 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:36:35 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:36:35 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff11c7face9c0891727fd900ff0b7729597f501799e6817982bcdf416db029df`  
		Last Modified: Fri, 24 Jul 2020 17:38:22 GMT  
		Size: 8.4 KB (8379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b123248cb48749dc2e3f1ca4c45c55fbd3f11b78c471cebcf18031bc96b78470`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed88e303b9446e31d2905ee51eace4acdbf43872db0b194c3062f2aec450307`  
		Last Modified: Fri, 24 Jul 2020 17:38:28 GMT  
		Size: 157.8 MB (157758394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba08f1fda8f80aaa8c65193f52ba91535890a15bae0a456d01c55b5b8f565527`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 968.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b4931c04889fd45a06eef4c69db92f27fbe88ac6f5034a3b25ed5db8b14b53`  
		Last Modified: Fri, 24 Jul 2020 17:38:21 GMT  
		Size: 9.5 KB (9494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af40bc93a666a58e89ff40c24cb7ae845b9a1e9ba2fc55851747f32186177709`  
		Last Modified: Fri, 24 Jul 2020 17:38:22 GMT  
		Size: 7.4 MB (7354989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.7-full-java8-openj9`

```console
$ docker pull open-liberty@sha256:68c1050e02d4bfbe28b8cf3b644a592815759c2fc71d31fc370ab1a65438c749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.7-full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:c2a27d0ea2a831437eb9aa7827ee8981f5c8a8dd7b0543ae0c531f532ee1761b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271833836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388a94564c394cd1198307ad44aa52575189e91fa2269f5b65430c4a487481a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:53:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 17 Jul 2020 22:54:26 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d87ae3bca31579ea606a2a26fda0d2764eed2c473dbd9463ac06b75fd7bd160`  
		Last Modified: Fri, 17 Jul 2020 22:57:11 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5043a1b4004b7c5e00d1325a216ffb151a0097b1772a5819aeddb8b53eab216`  
		Last Modified: Fri, 17 Jul 2020 22:57:14 GMT  
		Size: 16.6 MB (16607884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.7-full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:406e1fb5b9ecef8a18441c0e8f89bbec097e74f074000763c81ee68aadb90640
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.4 MB (273386132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533a1b42c71f538f3b60de5ea84664eacb0ba4a27ab3e5c652f9c60855043cec`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:04:40 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 18 Jul 2020 02:05:59 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3d863d3bbe2fba0007496e6d28cb1c228903d11def1649cd0740212c126e4`  
		Last Modified: Sat, 18 Jul 2020 02:18:20 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9473bd9c8be011b5c4fbaff984fdbbcdff651c5e34dbab19e442959b69d8658`  
		Last Modified: Sat, 18 Jul 2020 02:18:23 GMT  
		Size: 14.6 MB (14604611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.7-full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:d278466174c0b5b2e11bd4f5c312c9a52c3e99ba24eb4956a1458ce4b56ded9e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268806564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535780584bc43f463cc56e06ff859c24bffe1cbb8558188c357bd4ea58b4e68f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:35:35 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 24 Jul 2020 17:35:53 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4d14ed70732f9a814554bdc82298cb5007ee00e74145d9ec19670dbd1ce75`  
		Last Modified: Fri, 24 Jul 2020 17:38:10 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eba8540de396124137bf7c22f6a5f54817dac7c3f4a9163b068f7da134af6f`  
		Last Modified: Fri, 24 Jul 2020 17:38:12 GMT  
		Size: 16.2 MB (16223160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:20.0.0.7-kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:32a2ea1c3f7e8875a7a2a64386dafceddc1f387486782870b5f487473d50425b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:20.0.0.7-kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:9ec416148ff15897d3dba3fafe2e24f2b71526208eb5b5833bc349d906c68cec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255224988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b8699d351291d1d74a75f32f66d653aaee6c7765fd31b748c645a82398bd04`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.7-kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:d2cb84538ff7fcbe68ad226a2418a724415185d7613cffa1e27117295309d217
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258780554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5bf5002f95973df2e78c8fc6d50359a043e4a86fe9146c37c7c16ca67486123`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:20.0.0.7-kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:9cefbdfa6306cb7ea02459a48487a4615261ce979e5effe9c3811f253bcae4bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.6 MB (252582440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d36d55ef052dbab326c014b4681c441a98cae9fb12cd31fcb76a4b715d2ada36`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full`

```console
$ docker pull open-liberty@sha256:68c1050e02d4bfbe28b8cf3b644a592815759c2fc71d31fc370ab1a65438c749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full` - linux; amd64

```console
$ docker pull open-liberty@sha256:c2a27d0ea2a831437eb9aa7827ee8981f5c8a8dd7b0543ae0c531f532ee1761b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271833836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388a94564c394cd1198307ad44aa52575189e91fa2269f5b65430c4a487481a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:53:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 17 Jul 2020 22:54:26 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d87ae3bca31579ea606a2a26fda0d2764eed2c473dbd9463ac06b75fd7bd160`  
		Last Modified: Fri, 17 Jul 2020 22:57:11 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5043a1b4004b7c5e00d1325a216ffb151a0097b1772a5819aeddb8b53eab216`  
		Last Modified: Fri, 17 Jul 2020 22:57:14 GMT  
		Size: 16.6 MB (16607884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:406e1fb5b9ecef8a18441c0e8f89bbec097e74f074000763c81ee68aadb90640
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.4 MB (273386132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533a1b42c71f538f3b60de5ea84664eacb0ba4a27ab3e5c652f9c60855043cec`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:04:40 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 18 Jul 2020 02:05:59 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3d863d3bbe2fba0007496e6d28cb1c228903d11def1649cd0740212c126e4`  
		Last Modified: Sat, 18 Jul 2020 02:18:20 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9473bd9c8be011b5c4fbaff984fdbbcdff651c5e34dbab19e442959b69d8658`  
		Last Modified: Sat, 18 Jul 2020 02:18:23 GMT  
		Size: 14.6 MB (14604611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full` - linux; s390x

```console
$ docker pull open-liberty@sha256:d278466174c0b5b2e11bd4f5c312c9a52c3e99ba24eb4956a1458ce4b56ded9e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268806564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535780584bc43f463cc56e06ff859c24bffe1cbb8558188c357bd4ea58b4e68f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:35:35 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 24 Jul 2020 17:35:53 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4d14ed70732f9a814554bdc82298cb5007ee00e74145d9ec19670dbd1ce75`  
		Last Modified: Fri, 24 Jul 2020 17:38:10 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eba8540de396124137bf7c22f6a5f54817dac7c3f4a9163b068f7da134af6f`  
		Last Modified: Fri, 24 Jul 2020 17:38:12 GMT  
		Size: 16.2 MB (16223160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:full-java8-openj9`

```console
$ docker pull open-liberty@sha256:68c1050e02d4bfbe28b8cf3b644a592815759c2fc71d31fc370ab1a65438c749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:full-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:c2a27d0ea2a831437eb9aa7827ee8981f5c8a8dd7b0543ae0c531f532ee1761b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271833836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388a94564c394cd1198307ad44aa52575189e91fa2269f5b65430c4a487481a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:53:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 17 Jul 2020 22:54:26 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d87ae3bca31579ea606a2a26fda0d2764eed2c473dbd9463ac06b75fd7bd160`  
		Last Modified: Fri, 17 Jul 2020 22:57:11 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5043a1b4004b7c5e00d1325a216ffb151a0097b1772a5819aeddb8b53eab216`  
		Last Modified: Fri, 17 Jul 2020 22:57:14 GMT  
		Size: 16.6 MB (16607884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:406e1fb5b9ecef8a18441c0e8f89bbec097e74f074000763c81ee68aadb90640
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.4 MB (273386132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533a1b42c71f538f3b60de5ea84664eacb0ba4a27ab3e5c652f9c60855043cec`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:04:40 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 18 Jul 2020 02:05:59 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3d863d3bbe2fba0007496e6d28cb1c228903d11def1649cd0740212c126e4`  
		Last Modified: Sat, 18 Jul 2020 02:18:20 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9473bd9c8be011b5c4fbaff984fdbbcdff651c5e34dbab19e442959b69d8658`  
		Last Modified: Sat, 18 Jul 2020 02:18:23 GMT  
		Size: 14.6 MB (14604611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:full-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:d278466174c0b5b2e11bd4f5c312c9a52c3e99ba24eb4956a1458ce4b56ded9e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268806564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535780584bc43f463cc56e06ff859c24bffe1cbb8558188c357bd4ea58b4e68f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:35:35 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 24 Jul 2020 17:35:53 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4d14ed70732f9a814554bdc82298cb5007ee00e74145d9ec19670dbd1ce75`  
		Last Modified: Fri, 24 Jul 2020 17:38:10 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eba8540de396124137bf7c22f6a5f54817dac7c3f4a9163b068f7da134af6f`  
		Last Modified: Fri, 24 Jul 2020 17:38:12 GMT  
		Size: 16.2 MB (16223160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel`

```console
$ docker pull open-liberty@sha256:32a2ea1c3f7e8875a7a2a64386dafceddc1f387486782870b5f487473d50425b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel` - linux; amd64

```console
$ docker pull open-liberty@sha256:9ec416148ff15897d3dba3fafe2e24f2b71526208eb5b5833bc349d906c68cec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255224988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b8699d351291d1d74a75f32f66d653aaee6c7765fd31b748c645a82398bd04`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:d2cb84538ff7fcbe68ad226a2418a724415185d7613cffa1e27117295309d217
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258780554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5bf5002f95973df2e78c8fc6d50359a043e4a86fe9146c37c7c16ca67486123`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; s390x

```console
$ docker pull open-liberty@sha256:9cefbdfa6306cb7ea02459a48487a4615261ce979e5effe9c3811f253bcae4bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.6 MB (252582440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d36d55ef052dbab326c014b4681c441a98cae9fb12cd31fcb76a4b715d2ada36`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:kernel-java8-openj9`

```console
$ docker pull open-liberty@sha256:32a2ea1c3f7e8875a7a2a64386dafceddc1f387486782870b5f487473d50425b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel-java8-openj9` - linux; amd64

```console
$ docker pull open-liberty@sha256:9ec416148ff15897d3dba3fafe2e24f2b71526208eb5b5833bc349d906c68cec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.2 MB (255224988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b8699d351291d1d74a75f32f66d653aaee6c7765fd31b748c645a82398bd04`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-java8-openj9` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:d2cb84538ff7fcbe68ad226a2418a724415185d7613cffa1e27117295309d217
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.8 MB (258780554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5bf5002f95973df2e78c8fc6d50359a043e4a86fe9146c37c7c16ca67486123`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel-java8-openj9` - linux; s390x

```console
$ docker pull open-liberty@sha256:9cefbdfa6306cb7ea02459a48487a4615261ce979e5effe9c3811f253bcae4bc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.6 MB (252582440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d36d55ef052dbab326c014b4681c441a98cae9fb12cd31fcb76a4b715d2ada36`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:68c1050e02d4bfbe28b8cf3b644a592815759c2fc71d31fc370ab1a65438c749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:c2a27d0ea2a831437eb9aa7827ee8981f5c8a8dd7b0543ae0c531f532ee1761b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271833836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6388a94564c394cd1198307ad44aa52575189e91fa2269f5b65430c4a487481a`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 21:56:08 GMT
ADD file:0b40d881e3e00d68de1f1df0a565385bb838144b83814df891c994f466e9efa2 in / 
# Mon, 06 Jul 2020 21:56:09 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 21:56:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:56:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:56:11 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:03:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:52 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:21:18 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:21:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:21:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 17 Jul 2020 22:53:03 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 17 Jul 2020 22:53:04 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 17 Jul 2020 22:53:04 GMT
ARG OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:04 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 17 Jul 2020 22:53:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 17 Jul 2020 22:53:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 17 Jul 2020 22:53:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 17 Jul 2020 22:53:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 17 Jul 2020 22:53:19 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 17 Jul 2020 22:53:41 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 17 Jul 2020 22:53:41 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 17 Jul 2020 22:53:41 GMT
USER 1001
# Fri, 17 Jul 2020 22:53:41 GMT
EXPOSE 9080 9443
# Fri, 17 Jul 2020 22:53:42 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 17 Jul 2020 22:53:42 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 17 Jul 2020 22:53:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 17 Jul 2020 22:54:26 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:a1125296b23d78a3585a7910d649fbf0cc56284f9d2066e3243e8bc18f90b308`  
		Last Modified: Wed, 01 Jul 2020 12:21:40 GMT  
		Size: 26.7 MB (26696193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c742a4a0f38c95e690ad2dad8909c0cb232911418ac94a73da2a28becc7b734`  
		Last Modified: Mon, 06 Jul 2020 21:57:18 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ea3b329965bf7239f4e4f484915a444ec6d78b532ae12525934d4f6f7ac9a`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4be91ead68299f53759fd80c135e0dde0eb797e91eb8fbc5a708a506e0c433`  
		Last Modified: Mon, 06 Jul 2020 21:57:19 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262049cebf1b6f60b6dc78a926be5d3a689ba76a6c5c28edc9b195952b98c31f`  
		Last Modified: Fri, 17 Jul 2020 22:23:14 GMT  
		Size: 13.9 MB (13875144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7ae3562f54a1abcec2e390aa39c5d1bdd4d797018f8288100ac516ff45ec7e`  
		Last Modified: Fri, 17 Jul 2020 22:25:12 GMT  
		Size: 48.7 MB (48691295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cd1c7cabb21604488842a6b70ae3b2b1f4f3f4ab8f3166c7d886a938b470aa`  
		Last Modified: Fri, 17 Jul 2020 22:56:57 GMT  
		Size: 8.4 KB (8355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0a7e5386637638c3baa64552e90f97f3a78b8758988bede3c9aa9cd9ff23dd`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2164691c4714f263629a04436be551e7f183e34ae362c7cd328f004d6839e`  
		Last Modified: Fri, 17 Jul 2020 22:57:07 GMT  
		Size: 157.8 MB (157783993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9561ae263f5638923b206f0e2fe29e3b990a44216e271332e01860490479fd5`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0d9ee4b1303ecddcb8c9642dacd16d0ba6ca2667af936583b610dc1abdbd2`  
		Last Modified: Fri, 17 Jul 2020 22:56:56 GMT  
		Size: 9.4 KB (9404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78593c7e93c95a24d1067de28c5918f5b0934f1137c1b6ff284a4984214e12b`  
		Last Modified: Fri, 17 Jul 2020 22:56:58 GMT  
		Size: 8.1 MB (8123074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d87ae3bca31579ea606a2a26fda0d2764eed2c473dbd9463ac06b75fd7bd160`  
		Last Modified: Fri, 17 Jul 2020 22:57:11 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5043a1b4004b7c5e00d1325a216ffb151a0097b1772a5819aeddb8b53eab216`  
		Last Modified: Fri, 17 Jul 2020 22:57:14 GMT  
		Size: 16.6 MB (16607884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:406e1fb5b9ecef8a18441c0e8f89bbec097e74f074000763c81ee68aadb90640
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.4 MB (273386132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:533a1b42c71f538f3b60de5ea84664eacb0ba4a27ab3e5c652f9c60855043cec`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jul 2020 22:11:55 GMT
ADD file:02f6904c1e662a7dcf6c813b0b166d2a793532babdd26486ccdf54c62e496d74 in / 
# Mon, 06 Jul 2020 22:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Mon, 06 Jul 2020 22:12:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:12:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:12:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:37:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 17 Jul 2020 22:19:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 17 Jul 2020 22:23:30 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 17 Jul 2020 22:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 17 Jul 2020 22:24:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 17 Jul 2020 22:24:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 18 Jul 2020 02:01:05 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Sat, 18 Jul 2020 02:01:11 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Sat, 18 Jul 2020 02:01:18 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Sat, 18 Jul 2020 02:01:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Sat, 18 Jul 2020 02:01:26 GMT
ARG OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:01:30 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Sat, 18 Jul 2020 02:01:33 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Sat, 18 Jul 2020 02:01:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 18 Jul 2020 02:02:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 18 Jul 2020 02:02:36 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 18 Jul 2020 02:03:11 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 18 Jul 2020 02:03:29 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 18 Jul 2020 02:04:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 18 Jul 2020 02:04:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 18 Jul 2020 02:04:14 GMT
USER 1001
# Sat, 18 Jul 2020 02:04:19 GMT
EXPOSE 9080 9443
# Sat, 18 Jul 2020 02:04:21 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 18 Jul 2020 02:04:23 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Sat, 18 Jul 2020 02:04:40 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Sat, 18 Jul 2020 02:05:59 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:9bf98a17426d75ff2afb0ce90ba51b39da3fbd14db0cbd75941ca79a027edf5b`  
		Last Modified: Mon, 06 Jul 2020 15:46:29 GMT  
		Size: 30.4 MB (30403476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e6b7f1e0e442a73216c8f3a0be0d2541c137fd3387775bef4342bfb80c73d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 35.2 KB (35202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164204b75b39358091c51e041d91a70cee768036b72edaaa3c0a9d3b5f01bb4`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8349a86bc0c340cfe9292a4a0743f0d20683515f048ac5b7a38bad559ebd5d`  
		Last Modified: Mon, 06 Jul 2020 22:18:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa43882d8fd530416f9c313375005f26b3e32c8de56ef714a969cea393c840`  
		Last Modified: Fri, 17 Jul 2020 22:29:17 GMT  
		Size: 14.5 MB (14519008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5619f87564e3f3e7b4085ba86ac2983c16c46479b5a7e4f631e9f17b63528f7c`  
		Last Modified: Fri, 17 Jul 2020 22:32:27 GMT  
		Size: 49.2 MB (49150050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b16980667b6cf257f5dffb0289980883ce112dc23cb032c08489b48b3df88e`  
		Last Modified: Sat, 18 Jul 2020 02:17:54 GMT  
		Size: 8.4 KB (8382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a72a6ebb235b8952f22c24a95fa8543f80e8c58c15af372b95129e1e820a4`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3153ba5a4e1d3114b68ea85e4be3a97a70f5306da92bc0f21fd6715c8b2863ad`  
		Last Modified: Sat, 18 Jul 2020 02:18:05 GMT  
		Size: 157.8 MB (157785172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56717cde9ea5691083686031ff9d7c0081c78d19166876973b02393a08489ebe`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea378b21197e77bf2f0ef4aebdf4c637d53e68998641b9b4c270315e1fab7cf1`  
		Last Modified: Sat, 18 Jul 2020 02:17:51 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adeb21baf9321364d6aac56520d1c15a64bda2c48ad9d6de03495adf81daad0`  
		Last Modified: Sat, 18 Jul 2020 02:17:52 GMT  
		Size: 6.9 MB (6867452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a3d863d3bbe2fba0007496e6d28cb1c228903d11def1649cd0740212c126e4`  
		Last Modified: Sat, 18 Jul 2020 02:18:20 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9473bd9c8be011b5c4fbaff984fdbbcdff651c5e34dbab19e442959b69d8658`  
		Last Modified: Sat, 18 Jul 2020 02:18:23 GMT  
		Size: 14.6 MB (14604611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:d278466174c0b5b2e11bd4f5c312c9a52c3e99ba24eb4956a1458ce4b56ded9e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.8 MB (268806564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:535780584bc43f463cc56e06ff859c24bffe1cbb8558188c357bd4ea58b4e68f`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:07:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Jul 2020 15:08:06 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:13:31 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Fri, 24 Jul 2020 15:14:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Jul 2020 15:14:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:14:25 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_VERSION=20.0.0.7
# Fri, 24 Jul 2020 17:34:59 GMT
ARG LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_BUILD_LABEL=cl200720200625-0300
# Fri, 24 Jul 2020 17:35:00 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip
# Fri, 24 Jul 2020 17:35:00 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200720200625-0300 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.7
# Fri, 24 Jul 2020 17:35:00 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Fri, 24 Jul 2020 17:35:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Fri, 24 Jul 2020 17:35:12 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Fri, 24 Jul 2020 17:35:15 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:35:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:35:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Fri, 24 Jul 2020 17:35:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200720200625-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.7/openliberty-runtime-20.0.0.7.zip LIBERTY_SHA=226cd89250b2b831fd777042eff1ae69edb1cb1f LIBERTY_VERSION=20.0.0.7
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Fri, 24 Jul 2020 17:35:29 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Fri, 24 Jul 2020 17:35:29 GMT
USER 1001
# Fri, 24 Jul 2020 17:35:29 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:35:29 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:35:30 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:35:35 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Fri, 24 Jul 2020 17:35:53 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebf51d7ec44631141845860c73ae158d9eca8b087d075b3b5c3e7661e8ef437`  
		Last Modified: Fri, 24 Jul 2020 15:18:57 GMT  
		Size: 13.6 MB (13596135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93358898b91550d68b80b3d58ae875f654512e84efc3fb5b48b6267f6ee4cc9`  
		Last Modified: Fri, 24 Jul 2020 15:21:51 GMT  
		Size: 48.4 MB (48386852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7563bb2aec6b96c393862e4f2058765f70cb9e39fa7e4a86b41dae6fb41113`  
		Last Modified: Fri, 24 Jul 2020 17:37:58 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4c2cbac501e83a1b6a8bd010b0a26b26490a1201a07e124fb9ca836298bf46`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c60d1e1832b696d4583ef4104d0aefbbf3fdbcf3e912f910dacc9f74283e56`  
		Last Modified: Fri, 24 Jul 2020 17:38:04 GMT  
		Size: 157.8 MB (157784205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006a1e5ca0e1bf778c17b22cf959bd2b1a230b60f4a4f12b8478a865061684f`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 970.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173d1c10d8d509ac8d130380367391c45c3662fec3eb3b33aca47dfba66165e9`  
		Last Modified: Fri, 24 Jul 2020 17:37:56 GMT  
		Size: 9.5 KB (9490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91f40ddf6d30b4b0723b75694c949a73372b58bd95d27674ed6f411eace1666`  
		Last Modified: Fri, 24 Jul 2020 17:37:57 GMT  
		Size: 7.4 MB (7389409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd4d14ed70732f9a814554bdc82298cb5007ee00e74145d9ec19670dbd1ce75`  
		Last Modified: Fri, 24 Jul 2020 17:38:10 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23eba8540de396124137bf7c22f6a5f54817dac7c3f4a9163b068f7da134af6f`  
		Last Modified: Fri, 24 Jul 2020 17:38:12 GMT  
		Size: 16.2 MB (16223160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
