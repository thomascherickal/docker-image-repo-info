## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:b713233174a42a1ff6810634c47c6ae9757fe7f98b80e2c5d8c1d546706a6771
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:4a2665dc2f90245d2dad79dd526564518834f164687b65d094b9362e66659097
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.1 MB (244087382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb53d731275e0fc8b250e9c53fe271cde657f0d49d332e2a19d7edcece5beb85`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:44:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Jan 2020 01:45:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:46:28 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Thu, 16 Jan 2020 01:46:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3d96339956017e486fda746c4d79799ec26b1750f06e835561bbe480cb1ea37e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        s390x)          ESUM='b99b2d532a3874ecb1189defe1b26c5749a6fbd144d93436620038cda7ca5b84';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_s390x_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        amd64|x86_64)          ESUM='30bdfdb38901d4807d96a72a33b83f7a4f40255e11a88853c1e8732acc4644a7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_x64_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Jan 2020 01:46:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jan 2020 01:46:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 22 Jan 2020 23:20:24 GMT
ARG LIBERTY_VERSION=20.0.0.1
# Wed, 22 Jan 2020 23:20:24 GMT
ARG LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5
# Wed, 22 Jan 2020 23:20:24 GMT
ARG LIBERTY_BUILD_LABEL=cl200120200108-0300
# Wed, 22 Jan 2020 23:20:24 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip
# Wed, 22 Jan 2020 23:20:24 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200120200108-0300
# Wed, 22 Jan 2020 23:20:24 GMT
COPY dir:9836239f58c155c5069977595ca2f57d1849061e5426a8d04e229a44d8bf789f in /opt/ol/helpers 
# Wed, 22 Jan 2020 23:20:37 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 22 Jan 2020 23:20:37 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Wed, 22 Jan 2020 23:20:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 22 Jan 2020 23:20:39 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 22 Jan 2020 23:20:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN populate_scc.sh 4m 3     && rm -rf /output/messaging /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 22 Jan 2020 23:20:55 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 22 Jan 2020 23:20:55 GMT
USER 1001
# Wed, 22 Jan 2020 23:20:56 GMT
EXPOSE 9080 9443
# Wed, 22 Jan 2020 23:20:56 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 22 Jan 2020 23:20:56 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 22 Jan 2020 23:21:03 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e1a6e1ff3c935882f4005a6063541af139f9244769187488ef236e2052ce19`  
		Last Modified: Thu, 16 Jan 2020 01:48:24 GMT  
		Size: 13.3 MB (13323265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebebda7f1652cc076704348044c4842909daceef9bf436640f289864ada8670`  
		Last Modified: Thu, 16 Jan 2020 01:51:25 GMT  
		Size: 48.0 MB (47954202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880eb5b3105726a8f797eb0d6621bab3988909e3bf30087f0f0dcbba993d2676`  
		Last Modified: Wed, 22 Jan 2020 23:23:40 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4053916fe836485b621b916d55c943233ed0bfa27aedc07d58f5b993cbda3d66`  
		Last Modified: Wed, 22 Jan 2020 23:24:04 GMT  
		Size: 155.0 MB (155005703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216c245d0fabaeef05d5f31f01b8cdd194ce0ddd185be5f4b596fec3219c8a5e`  
		Last Modified: Wed, 22 Jan 2020 23:23:40 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63d0ce1e622d6b3f417b4a2fe29b590d0a852cd864aa3820ca9633e8726e88c`  
		Last Modified: Wed, 22 Jan 2020 23:23:40 GMT  
		Size: 3.8 KB (3808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e24a11701612e76e0a7960c24f67c5a22cc2a4378aa89c02a8472f9f445012`  
		Last Modified: Wed, 22 Jan 2020 23:23:41 GMT  
		Size: 1.1 MB (1069029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6664efff25366546372bbbd25f05f76f465b0e012c3b36f97860df7fe5c910d3`  
		Last Modified: Wed, 22 Jan 2020 23:24:10 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:507e3acb3c8fd02f1adab1704bc0aab46b224d0a030af5e0225e661b5eacad82
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248896974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:446e8db23e3569670a3b5d7d154828c8bf3fd0eacb94b364883a4b6e16cfa637`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:43:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Jan 2020 01:44:08 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:46:38 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Thu, 16 Jan 2020 01:47:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3d96339956017e486fda746c4d79799ec26b1750f06e835561bbe480cb1ea37e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        s390x)          ESUM='b99b2d532a3874ecb1189defe1b26c5749a6fbd144d93436620038cda7ca5b84';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_s390x_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        amd64|x86_64)          ESUM='30bdfdb38901d4807d96a72a33b83f7a4f40255e11a88853c1e8732acc4644a7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_x64_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Jan 2020 01:47:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jan 2020 01:47:19 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 23 Jan 2020 00:25:27 GMT
ARG LIBERTY_VERSION=20.0.0.1
# Thu, 23 Jan 2020 00:25:30 GMT
ARG LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5
# Thu, 23 Jan 2020 00:25:34 GMT
ARG LIBERTY_BUILD_LABEL=cl200120200108-0300
# Thu, 23 Jan 2020 00:25:36 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip
# Thu, 23 Jan 2020 00:25:38 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200120200108-0300
# Thu, 23 Jan 2020 00:25:40 GMT
COPY dir:9836239f58c155c5069977595ca2f57d1849061e5426a8d04e229a44d8bf789f in /opt/ol/helpers 
# Thu, 23 Jan 2020 00:26:14 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 23 Jan 2020 00:26:17 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Thu, 23 Jan 2020 00:26:27 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 23 Jan 2020 00:26:32 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 23 Jan 2020 00:26:55 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN populate_scc.sh 4m 3     && rm -rf /output/messaging /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 23 Jan 2020 00:26:57 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 23 Jan 2020 00:27:00 GMT
USER 1001
# Thu, 23 Jan 2020 00:27:03 GMT
EXPOSE 9080 9443
# Thu, 23 Jan 2020 00:27:05 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 23 Jan 2020 00:27:07 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 23 Jan 2020 00:27:27 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5515694a6e8bfc9e87d0ae9d3b2046662f7a29cfbcb1eaa00c8c3d1a2ba211`  
		Last Modified: Thu, 16 Jan 2020 01:50:01 GMT  
		Size: 14.0 MB (13969109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ccf4b12a3d3e3b2b4191ee5f43db32f4f8f45e405c1e411535a14740891072`  
		Last Modified: Thu, 16 Jan 2020 01:53:35 GMT  
		Size: 48.4 MB (48403146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4c45191dd9e322814f829c25da362c4fe99aa795c8f739b17b35190ca595cc`  
		Last Modified: Thu, 23 Jan 2020 00:30:00 GMT  
		Size: 2.9 KB (2935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6873d212218b760829416f93f6600679dbfff192cc0d854a8795fa609ef67919`  
		Last Modified: Thu, 23 Jan 2020 00:30:15 GMT  
		Size: 155.0 MB (155005853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106c7ff825c3f9bfced05d7c54b02666bb98d360419a87363dd564c9cd2d58ce`  
		Last Modified: Thu, 23 Jan 2020 00:30:00 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e117f6f9a2d2020d62bf031582ec540efd9ca2413a79c25e9584f8765efc76`  
		Last Modified: Thu, 23 Jan 2020 00:30:00 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb0a8a7391a98d12194b7bf00f3f11fc8e57cc6ddc9010da78ebfb07378f0c0`  
		Last Modified: Thu, 23 Jan 2020 00:30:01 GMT  
		Size: 1.1 MB (1073202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ef2765180502c67439e20f35ca33441ac39f03007a88be119921d0064e9774`  
		Last Modified: Thu, 23 Jan 2020 00:30:26 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:8c6005f01f6c4d4a6731e911af102368a7a9eab62eff406b751e628b9c96138f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.0 MB (242978011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bf127d3239d41f8487125420fa9858b26359070bbd14a03b03b2daca706f620`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 31 Oct 2019 22:41:56 GMT
ADD file:6e6c5c69d7791dc0b62c8d03fc0c5051c6291e08dfc4e11abbdc333bc6f44359 in / 
# Thu, 31 Oct 2019 22:41:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:41:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:42:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:42:01 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:00:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 08 Nov 2019 02:41:48 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 08 Nov 2019 02:42:43 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Fri, 08 Nov 2019 02:43:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='3d96339956017e486fda746c4d79799ec26b1750f06e835561bbe480cb1ea37e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        s390x)          ESUM='b99b2d532a3874ecb1189defe1b26c5749a6fbd144d93436620038cda7ca5b84';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_s390x_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        amd64|x86_64)          ESUM='30bdfdb38901d4807d96a72a33b83f7a4f40255e11a88853c1e8732acc4644a7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jre_x64_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 08 Nov 2019 02:43:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Nov 2019 02:43:02 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 22 Jan 2020 23:49:32 GMT
ARG LIBERTY_VERSION=20.0.0.1
# Wed, 22 Jan 2020 23:49:32 GMT
ARG LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5
# Wed, 22 Jan 2020 23:49:32 GMT
ARG LIBERTY_BUILD_LABEL=cl200120200108-0300
# Wed, 22 Jan 2020 23:49:33 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip
# Wed, 22 Jan 2020 23:49:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200120200108-0300
# Wed, 22 Jan 2020 23:49:33 GMT
COPY dir:9836239f58c155c5069977595ca2f57d1849061e5426a8d04e229a44d8bf789f in /opt/ol/helpers 
# Wed, 22 Jan 2020 23:51:23 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 22 Jan 2020 23:51:23 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true
# Wed, 22 Jan 2020 23:51:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 22 Jan 2020 23:51:26 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 22 Jan 2020 23:51:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200120200108-0300 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.1/openliberty-runtime-20.0.0.1.zip LIBERTY_SHA=dfededade132ba37fabbcf07d5004773ee9f3be5 LIBERTY_VERSION=20.0.0.1
RUN populate_scc.sh 4m 3     && rm -rf /output/messaging /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 22 Jan 2020 23:51:36 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 22 Jan 2020 23:51:36 GMT
USER 1001
# Wed, 22 Jan 2020 23:51:37 GMT
EXPOSE 9080 9443
# Wed, 22 Jan 2020 23:51:37 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 22 Jan 2020 23:51:37 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 22 Jan 2020 23:51:52 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
```

-	Layers:
	-	`sha256:617b55fd1ba95b3ed68226101c9b2568ed00a9b7c50959230d2124648f3a47d2`  
		Last Modified: Thu, 31 Oct 2019 22:43:47 GMT  
		Size: 25.4 MB (25364650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee6ed80b799b3b7d7d66e31ba7e61be1f8d02732bccb1a22d1f14c65f9cea21`  
		Last Modified: Thu, 31 Oct 2019 22:43:42 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc71634b6bba51b68da661aedfd0876ba93b197653cc94323ca050369bef0bc`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e017bfda3869ce68902d01d6dfb0fe74964f8c598ea31bc77825772e58a122b`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b19c0383ed91f9b1804ed41cac85c7d675628ede6f1b32b27d54b75a6f40aa`  
		Last Modified: Fri, 08 Nov 2019 02:44:24 GMT  
		Size: 13.0 MB (13040836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b63420eb012512ef34ef7e38065d3f26446be94667985189c3af8ecf724d517`  
		Last Modified: Fri, 08 Nov 2019 02:45:58 GMT  
		Size: 48.1 MB (48137321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92df130d9abe09c5d48c86eea1b7851a135688f7f3824d1b830d564847c2e3cf`  
		Last Modified: Wed, 22 Jan 2020 23:55:37 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8b5cf043da8542a135d4a4d3fe65ac35be55e93a3a313ba0789760265c7d08`  
		Last Modified: Wed, 22 Jan 2020 23:55:48 GMT  
		Size: 155.3 MB (155316692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c5f92be82947b34aecf6823f5ea5a693863d487cc37298ca3cbb86717de34d`  
		Last Modified: Wed, 22 Jan 2020 23:55:37 GMT  
		Size: 937.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba1c6afeff955a2773c3f31609eec959644d99e14bdf1c4ed52e74910e40e68`  
		Last Modified: Wed, 22 Jan 2020 23:55:37 GMT  
		Size: 3.8 KB (3807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937f2b94f50a75f76c95823433f164ba0314d0bd41ac60d4fd59f36c43afce5f`  
		Last Modified: Wed, 22 Jan 2020 23:55:37 GMT  
		Size: 1.1 MB (1072722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571a45215242415cafef863fc56686c0c4f610b8bccfdc6dd7f6cb1c96d3a403`  
		Last Modified: Wed, 22 Jan 2020 23:55:54 GMT  
		Size: 967.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
