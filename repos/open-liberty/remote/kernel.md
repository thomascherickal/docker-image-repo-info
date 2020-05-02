## `open-liberty:kernel`

```console
$ docker pull open-liberty@sha256:f27c5d294c36db0cfe50033f4426711a892f8222f8723b673d503db149f84400
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:kernel` - linux; amd64

```console
$ docker pull open-liberty@sha256:c747300d58d695ed0fa0823769bfb3e54beab0d295e4e2153e3e5f4eeda50d46
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.2 MB (252157783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24447081dd17b756a82636ebf642ab2c02768a06205384ad6f4e41c1c65f6dbe`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Apr 2020 01:07:00 GMT
ADD file:c3e6bb316dfa6b81dd4478aaa310df532883b1c0a14edeec3f63d641980c1789 in / 
# Fri, 24 Apr 2020 01:07:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Apr 2020 01:07:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Apr 2020 01:07:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Apr 2020 01:07:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 19:27:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Apr 2020 19:28:13 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 19:29:59 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Fri, 24 Apr 2020 19:30:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Apr 2020 19:30:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 19:30:18 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Sat, 25 Apr 2020 00:57:16 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Sat, 25 Apr 2020 00:57:16 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Sat, 25 Apr 2020 00:57:16 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Sat, 25 Apr 2020 00:57:17 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Sat, 25 Apr 2020 00:57:17 GMT
ARG OPENJ9_SCC=true
# Sat, 02 May 2020 00:20:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.4
# Sat, 02 May 2020 00:20:03 GMT
COPY dir:507dac3c6bcde6740cd7ed24cbc9211d8f9af223d8c63028a3be9fe6830a0d50 in /opt/ol/helpers 
# Sat, 02 May 2020 00:20:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 02 May 2020 00:20:16 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 02 May 2020 00:20:16 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 02 May 2020 00:20:17 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 02 May 2020 00:20:18 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 02 May 2020 00:20:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 02 May 2020 00:20:37 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 02 May 2020 00:20:38 GMT
USER 1001
# Sat, 02 May 2020 00:20:38 GMT
EXPOSE 9080 9443
# Sat, 02 May 2020 00:20:38 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 02 May 2020 00:20:38 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:23884877105a7ff84a910895cd044061a4561385ff6c36480ee080b76ec0e771`  
		Last Modified: Sat, 04 Apr 2020 12:21:10 GMT  
		Size: 26.7 MB (26689802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc38caa0f5b94141276220daaf428892096e4afd24b05668cd188311e00a635f`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 35.4 KB (35367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2910811b6c4227c2f42aaea9a3dd5f53b1d469f67e2cf7e601f631b119b61ff7`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36505266dcc64eeb1010bd2112e6f73981e1a8246e4f6d4e287763b57f101b0b`  
		Last Modified: Fri, 24 Apr 2020 01:09:01 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3058952867bac0b1deeecce925b304f4e354c7b8781d75fbfc6d36373ead53af`  
		Last Modified: Fri, 24 Apr 2020 19:32:11 GMT  
		Size: 13.3 MB (13324407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ca17f7600d2906e0183fa0288c8a744578c210727ae22c06d4b22c180b0e6`  
		Last Modified: Fri, 24 Apr 2020 19:34:47 GMT  
		Size: 48.5 MB (48502686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b5f575dfb2df027b791b1b61124a5499612f68db61a96008c390fae207f9cb`  
		Last Modified: Sat, 02 May 2020 00:23:21 GMT  
		Size: 8.0 KB (7975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3677f82c8c2d967a35acbe8c626de536b0082fae982081deefdb76880e439a3d`  
		Last Modified: Sat, 02 May 2020 00:23:20 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c873ee878087db84716bb946644e1909f97258c7a9d7c740bc6a4e469b4a41`  
		Last Modified: Sat, 02 May 2020 00:23:29 GMT  
		Size: 155.4 MB (155443591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67576cc58669d9fe7e25647692107efc34f3def6540c5e0c415e9f6e09c1a404`  
		Last Modified: Sat, 02 May 2020 00:23:20 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a30d8daac07917fcaadc9491b51b482ca4cb4aff66b32d8468d12beae87756`  
		Last Modified: Sat, 02 May 2020 00:23:20 GMT  
		Size: 9.0 KB (9019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59916918d5d2848725183530f0e622e8d5b12c41362e00951c348e74a0e67f25`  
		Last Modified: Sat, 02 May 2020 00:23:21 GMT  
		Size: 8.1 MB (8142776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:2b405e48eb65857d0cdd375e437b1acbe22dc86c3f437cc32c796e67c067410a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.8 MB (255752607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09ec5f2f1deded0474246f7ed74eae878ed0bc1e424452635d56289a216878ae`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 23 Apr 2020 20:42:30 GMT
ADD file:726a32203fbcaae787c10740754e38dcb186778893e6d078db3cba0f49ee6b3c in / 
# Thu, 23 Apr 2020 20:42:37 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 20:42:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 20:42:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 20:42:50 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 11:22:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Apr 2020 11:23:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 11:28:55 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Fri, 24 Apr 2020 11:29:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Apr 2020 11:29:59 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 11:30:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Apr 2020 17:12:14 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Fri, 24 Apr 2020 17:12:16 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Fri, 24 Apr 2020 17:12:19 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Fri, 24 Apr 2020 17:12:22 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Fri, 24 Apr 2020 17:12:24 GMT
ARG OPENJ9_SCC=true
# Sat, 02 May 2020 00:17:25 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.4
# Sat, 02 May 2020 00:17:26 GMT
COPY dir:507dac3c6bcde6740cd7ed24cbc9211d8f9af223d8c63028a3be9fe6830a0d50 in /opt/ol/helpers 
# Sat, 02 May 2020 00:17:26 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 02 May 2020 00:18:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 02 May 2020 00:18:10 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 02 May 2020 00:18:21 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 02 May 2020 00:18:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 02 May 2020 00:18:51 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 02 May 2020 00:18:53 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 02 May 2020 00:18:55 GMT
USER 1001
# Sat, 02 May 2020 00:18:56 GMT
EXPOSE 9080 9443
# Sat, 02 May 2020 00:18:59 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 02 May 2020 00:19:00 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:beed3bd0a281cacead564771f079ed9ee8b272a2ed0e28f533e188f3d21fee6e`  
		Last Modified: Mon, 06 Apr 2020 15:40:20 GMT  
		Size: 30.4 MB (30400298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae14d2411b83450b8afe92058b998540c56ec42f1ddd7581e8e9fe629c442f89`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82678240be3a5c783512ff7336f2b10837ae126958bc6bd1b476a8d039c08771`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7307ad4f24078fd763b41ec7c1772f2fd5238fed1bae36c5d42d28ec9adbffb9`  
		Last Modified: Thu, 23 Apr 2020 20:48:44 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841fc1003510ef9b0e7994850d1dd2608238f020eb8892ebb14f71b9b02c1170`  
		Last Modified: Fri, 24 Apr 2020 11:36:20 GMT  
		Size: 14.0 MB (13970642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45e0c4fcddd15c749661cc0058c2dd7920e760df9db2dffdc965e2ef971479`  
		Last Modified: Fri, 24 Apr 2020 11:42:31 GMT  
		Size: 49.0 MB (48992426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d573918de07ace95262b809258b3db7adc6b6102604d81600295efbf79e6f5`  
		Last Modified: Sat, 02 May 2020 00:25:44 GMT  
		Size: 8.0 KB (8009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce60e105919d46fa6b959a7a15698674638b242e1eec60c1d96c0dad0c798683`  
		Last Modified: Sat, 02 May 2020 00:25:41 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2cc9f1fb1ac955a4b5b3a249f7766cf7c6a1d04f2ee55bc839216b0bd5e9ad`  
		Last Modified: Sat, 02 May 2020 00:26:28 GMT  
		Size: 155.4 MB (155444564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d5045f7635d1dc2085c1c979f0c13d5bd22ca819215a2d7a126e0a745af56`  
		Last Modified: Sat, 02 May 2020 00:25:41 GMT  
		Size: 979.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0cfb645641b5bc3b8b819784d103d488d5e8a7cc250b70ce64d7b6121bc1e4`  
		Last Modified: Sat, 02 May 2020 00:25:41 GMT  
		Size: 9.1 KB (9140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a91fa109e9c9c8b887bca92ab9b2a36c458c16aed35f2b67d99637ddb0daed`  
		Last Modified: Sat, 02 May 2020 00:25:45 GMT  
		Size: 6.9 MB (6890046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:kernel` - linux; s390x

```console
$ docker pull open-liberty@sha256:0ae217f5b08bde99fd3703c75229aab75af238d712aa3aaee1942a4df577cc2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.4 MB (250441374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:345e0fb1e9ea7b2c961c3f67d8d6655aff55a803d91343553cf1558969f5eea2`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 23 Apr 2020 17:52:20 GMT
ADD file:ea66ef2a01c547f771866bfa221969f8a30489c28d2a81be8dde7f40e73da33b in / 
# Thu, 23 Apr 2020 17:52:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 23 Apr 2020 17:52:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 23 Apr 2020 17:52:30 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 23 Apr 2020 17:52:31 GMT
CMD ["/bin/bash"]
# Fri, 24 Apr 2020 07:36:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 24 Apr 2020 07:37:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Apr 2020 07:39:14 GMT
ENV JAVA_VERSION=jdk8u252-b09_openj9-0.20.0
# Fri, 24 Apr 2020 07:39:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='00095854b2219c71a142135ef2b63ae48869f4366c82524353991a36204cf7e9';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        s390x)          ESUM='7cb7d392fb7240c30b0993a6ec332060b406641589b4c0207b7f9cbbaad81fc8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_s390x_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5c0ab4691ff5f8e69bb14462f2afb8d73d751b01048eacf4b426ed6d6646dc63';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u252-b09_openj9-0.20.0/OpenJDK8U-jre_x64_linux_openj9_8u252b09_openj9-0.20.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 24 Apr 2020 07:39:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Apr 2020 07:39:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Fri, 24 Apr 2020 11:06:19 GMT
ARG LIBERTY_VERSION=20.0.0.4
# Fri, 24 Apr 2020 11:06:20 GMT
ARG LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10
# Fri, 24 Apr 2020 11:06:20 GMT
ARG LIBERTY_BUILD_LABEL=cl200420200401-1714
# Fri, 24 Apr 2020 11:06:20 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip
# Fri, 24 Apr 2020 11:06:20 GMT
ARG OPENJ9_SCC=true
# Sat, 02 May 2020 00:46:18 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200420200401-1714 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.4
# Sat, 02 May 2020 00:46:19 GMT
COPY dir:507dac3c6bcde6740cd7ed24cbc9211d8f9af223d8c63028a3be9fe6830a0d50 in /opt/ol/helpers 
# Sat, 02 May 2020 00:46:19 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Sat, 02 May 2020 00:46:31 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Sat, 02 May 2020 00:46:33 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Sat, 02 May 2020 00:46:35 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 02 May 2020 00:46:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Sat, 02 May 2020 00:46:48 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200420200401-1714 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.4/openliberty-runtime-20.0.0.4.zip LIBERTY_SHA=bddb444a461e22d1e69b970916993fe3046a0f10 LIBERTY_VERSION=20.0.0.4
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Sat, 02 May 2020 00:46:48 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Sat, 02 May 2020 00:46:48 GMT
USER 1001
# Sat, 02 May 2020 00:46:49 GMT
EXPOSE 9080 9443
# Sat, 02 May 2020 00:46:49 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Sat, 02 May 2020 00:46:49 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:13b4c2e4bb97a2a80bb0e557eeba41e4adea0f5e18352e359bca3f847193899c`  
		Last Modified: Mon, 06 Apr 2020 15:41:16 GMT  
		Size: 25.4 MB (25365338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a80e39fb485b86610de915eaaad3d867cc97e460b6da3bb656e03520e8a63`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 36.2 KB (36171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb0c128ddabc6a980ec71426ade04fc9bba2e1afcdc243e2d09c316b635f814`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678052ac148ee123df2f0773eb3a0f5f90490ada8b9a5705363b18a2f45fbe88`  
		Last Modified: Thu, 23 Apr 2020 17:54:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda817e3f7c865b0840c4d8029ccd310418aaf7af7a0aeda3eaa4cb945fca4b`  
		Last Modified: Fri, 24 Apr 2020 07:41:58 GMT  
		Size: 13.0 MB (13043886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fffe5699c9d3c03456957c9977d42c3622c4b7180850d773a72dbc3a7e9c06`  
		Last Modified: Fri, 24 Apr 2020 07:44:28 GMT  
		Size: 48.3 MB (48289486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43283e58300c7cfeb317c8dda8302733d68fb1ddb85d65f545d1b662cf6dd0e`  
		Last Modified: Sat, 02 May 2020 00:49:23 GMT  
		Size: 8.0 KB (8004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0743962d48228cada53a4b13353076a442cee69da05a30f2e6a4e2a6737567`  
		Last Modified: Sat, 02 May 2020 00:49:22 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683572ff7bae0f782e21af036b09932475e13c9898454779bee4e8eef44faf7`  
		Last Modified: Sat, 02 May 2020 00:49:35 GMT  
		Size: 155.4 MB (155443603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828a2367d7bf2ec8fae90121d42d2a3f079511d3cb76fb1f61cd0481d5d11981`  
		Last Modified: Sat, 02 May 2020 00:49:37 GMT  
		Size: 969.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc668b10988e40901411d302afe3c8e83cdc7ad986c15e6fc892c36321a64a6`  
		Last Modified: Sat, 02 May 2020 00:49:22 GMT  
		Size: 9.1 KB (9121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7798ce4b66d9f4af4a62400e62ccfb192385ef36887e0fb373ae77854f06ab33`  
		Last Modified: Sat, 02 May 2020 00:49:23 GMT  
		Size: 8.2 MB (8243493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
