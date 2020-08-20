## `open-liberty:latest`

```console
$ docker pull open-liberty@sha256:653bc5b94658baf23fad2f69e91477a95ec86c0db9f738763a825107882c413d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `open-liberty:latest` - linux; amd64

```console
$ docker pull open-liberty@sha256:7cbe0cfd4556d2484c1f7054179541681d9b31a76f72086b9fe77869990082ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.2 MB (272154665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02d04f1ae31520d1f366a0ed0fa838952d13c24556a0460f8cd411523e83344d`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:58:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:58:49 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:00:38 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:00:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:00:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 02:16:31 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 02:16:32 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:32 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 02:16:32 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 02:16:44 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 02:16:44 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 02:16:45 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 02:16:46 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 02:17:07 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 02:17:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 02:17:08 GMT
USER 1001
# Thu, 20 Aug 2020 02:17:08 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 02:17:08 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 02:17:08 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 02:17:21 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 02:17:55 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7f96c83b992275744136bd8deb3404fb357ee0e75620f46f7db8aed8481d6`  
		Last Modified: Wed, 19 Aug 2020 22:02:55 GMT  
		Size: 13.9 MB (13875193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a8737f865890826d26efd4c158416bd1188e715c783fd41548e040ef975dbe`  
		Last Modified: Wed, 19 Aug 2020 22:05:50 GMT  
		Size: 48.7 MB (48691306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597d5c2fcc114d8288a0802f34d16d564cb007ed2d59d38188aa091be14b25d`  
		Last Modified: Thu, 20 Aug 2020 02:20:24 GMT  
		Size: 8.4 KB (8352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888430f050ceadc370b33895dc685299bfd5a255de3160addf3e8887d57ad3c1`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34bb89999af5eea4a3a2270b33aab65b156ded317b60b50da02b17e14762d37`  
		Last Modified: Thu, 20 Aug 2020 02:20:34 GMT  
		Size: 157.8 MB (157847581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea7686ef22dccde6374800a0a8af564aab1d2ce37971d5491effba12f260f83`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd604c0109bce96a7f35816d7a30c902b84f8cafc5121ae095a6e3bb00b07fc4`  
		Last Modified: Thu, 20 Aug 2020 02:20:23 GMT  
		Size: 9.4 KB (9400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6cc4e7ae36550db2126f74e99c81b6d5eb44b5f5b38112ff7272b531c91db`  
		Last Modified: Thu, 20 Aug 2020 02:20:25 GMT  
		Size: 8.1 MB (8057281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a7ba33d6ba87063fb63dd6b87d739a5c0ebae06b7ac2867d34a17af16c0a3`  
		Last Modified: Thu, 20 Aug 2020 02:20:38 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3fd1c9f3fd3f9472a9dddda0b74f0edf7b5ae82f7d7bf7fb104c3e63bd634d`  
		Last Modified: Thu, 20 Aug 2020 02:20:41 GMT  
		Size: 16.9 MB (16926973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; ppc64le

```console
$ docker pull open-liberty@sha256:cfc22d235e304fb21276e202255d52b979ce40e105a1ab420fd1f17418abcca4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.6 MB (273578130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7be0bb5cbe3179d1a1d907492325e9237827a8a8f805ab37c1b5788f12975fe8`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:04 GMT
ADD file:4954b2b03fa4bd48fabecbc1facd6d05808f55a143012aca45648ab2f767042a in / 
# Wed, 19 Aug 2020 21:14:14 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:22 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:32 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:22:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 22:25:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:33 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 22:33:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 22:33:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 22:33:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 20 Aug 2020 03:13:43 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Thu, 20 Aug 2020 03:13:46 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Thu, 20 Aug 2020 03:13:49 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Thu, 20 Aug 2020 03:13:52 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Thu, 20 Aug 2020 03:13:53 GMT
ARG OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:14:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Thu, 20 Aug 2020 03:14:02 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Thu, 20 Aug 2020 03:14:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Thu, 20 Aug 2020 03:14:56 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Thu, 20 Aug 2020 03:15:06 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Thu, 20 Aug 2020 03:15:25 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 20 Aug 2020 03:15:36 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Thu, 20 Aug 2020 03:16:06 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Thu, 20 Aug 2020 03:16:09 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Thu, 20 Aug 2020 03:16:12 GMT
USER 1001
# Thu, 20 Aug 2020 03:16:18 GMT
EXPOSE 9080 9443
# Thu, 20 Aug 2020 03:16:23 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Thu, 20 Aug 2020 03:16:29 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Thu, 20 Aug 2020 03:16:49 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Thu, 20 Aug 2020 03:17:48 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:23e4ce51557a90638716607f36b99292ea21b3e246ef66f83934e1eadb095632`  
		Last Modified: Mon, 10 Aug 2020 15:49:13 GMT  
		Size: 30.4 MB (30408877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b20479dd2a1972abd69e09a781025590f55fcbe8bef98a35b1067dceff85d60`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 35.2 KB (35223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3107678818d326669afdd9fcce37d6b61613c2103e889ff7e019515b97ade1d`  
		Last Modified: Wed, 19 Aug 2020 21:18:51 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a571510b31b5805e20c811dcbb2413f66118e4be6a44a54c430826d8be670e7`  
		Last Modified: Wed, 19 Aug 2020 21:18:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a656bb9c393e26fb309b29304e7708385080d6380485fd32eca79e8dc60234`  
		Last Modified: Wed, 19 Aug 2020 22:41:31 GMT  
		Size: 14.5 MB (14518782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f59a1586230e65d6fbe8aebe774b944895c099ea81decb8818ba03aa8180880`  
		Last Modified: Wed, 19 Aug 2020 22:46:13 GMT  
		Size: 49.2 MB (49150099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ec4d988366d9ca7186bc54ce46603179ccf0681f888dc0d42e8cb0c3e7d01d`  
		Last Modified: Thu, 20 Aug 2020 03:26:08 GMT  
		Size: 8.4 KB (8383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1de4b8fd3a1677f86db2f581b69d6b8ec280d723044406d5873ef487e619738`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a445138c34d32647f9b4d494a0fa8d79332a812060b2c8ff31ef187339c1e9e`  
		Last Modified: Thu, 20 Aug 2020 03:26:17 GMT  
		Size: 157.8 MB (157848062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f6f8ed2c43944590fd32a48b0d2074618a6245b71a2ed18462d5c96e676b6c`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 981.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa47e1e197708807cfe4e1f6eae85c6097ceb9ff78de264cd77ff350acb85f`  
		Last Modified: Thu, 20 Aug 2020 03:26:03 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d2059ad7e51f9f633a992795b9d65cee7c9666fc49ff54680de2ce3ea9383`  
		Last Modified: Thu, 20 Aug 2020 03:26:05 GMT  
		Size: 6.9 MB (6918933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99121a436a07f2e84c54768e407a35724fb9a63574e29822e45ddcbde16aeb44`  
		Last Modified: Thu, 20 Aug 2020 03:26:29 GMT  
		Size: 966.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4d071db851d85c4d43f702c7b21e45077482c290f5d9fdb4f0be564a861dda`  
		Last Modified: Thu, 20 Aug 2020 03:26:33 GMT  
		Size: 14.7 MB (14676987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `open-liberty:latest` - linux; s390x

```console
$ docker pull open-liberty@sha256:842c5646b1c1e6d9b3a2aabd4883f4bcbf1c92690eb23cb7e874c6bf02bc1df2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.0 MB (269026630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c069ce61a624fb5ddfc3281f89c87b994492debae51d4aed6fa84b1c88d34f77`
-	Entrypoint: `["\/opt\/ol\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ol\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 21:55:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 19 Aug 2020 21:56:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:59:22 GMT
ENV JAVA_VERSION=jdk8u262-b10_openj9-0.21.0
# Wed, 19 Aug 2020 21:59:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='722517d9565bd9602580609114eb0de9b40b01050d52ff7bae24c438d363e186';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_ppc64le_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        s390x)          ESUM='c14aeedf4e989a6b31e00d6e18b8377957b07b000cac316aee9d973ef6d65b6f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_s390x_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        amd64|x86_64)          ESUM='aef8750b492ff6371318cf5138e38827d8895815b2ac079dcfcb02007a45c7f6';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u262-b10_openj9-0.21.0/OpenJDK8U-jre_x64_linux_openj9_8u262b10_openj9-0.21.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 19 Aug 2020 21:59:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_VERSION=20.0.0.8
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63
# Wed, 19 Aug 2020 22:46:11 GMT
ARG LIBERTY_BUILD_LABEL=cl200820200721-1900
# Wed, 19 Aug 2020 22:46:12 GMT
ARG LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip
# Wed, 19 Aug 2020 22:46:12 GMT
ARG OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:12 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=Open Liberty org.opencontainers.image.url=https://openliberty.io/ org.opencontainers.image.source=https://github.com/OpenLiberty/ci.docker org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the Open Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/OpenLiberty/ci.docker#building-an-application-image org.opencontainers.image.title=Open Liberty org.opencontainers.image.version=20.0.0.8
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:e8bb2487ca41e6b847cd1240bcb920ccb8c6de3c77aaaaf5ed7f0d39a3789c4a in /opt/ol/helpers 
# Wed, 19 Aug 2020 22:46:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ol/fixes/ 
# Wed, 19 Aug 2020 22:46:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8 OPENJ9_SCC=true
RUN apt-get update     && apt-get install -y --no-install-recommends unzip openssl wget     && rm -rf /var/lib/apt/lists/*     && wget -q $LIBERTY_DOWNLOAD_URL -U UA-Open-Liberty-Docker -O /tmp/wlp.zip     && echo "$LIBERTY_SHA  /tmp/wlp.zip" > /tmp/wlp.zip.sha1     && sha1sum -c /tmp/wlp.zip.sha1     && unzip -q /tmp/wlp.zip -d /opt/ol     && rm /tmp/wlp.zip     && rm /tmp/wlp.zip.sha1     && apt-get remove -y unzip     && apt-get remove -y wget     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && chown -R 1001:0 /opt/ol/wlp     && chmod -R g+rw /opt/ol/wlp
# Wed, 19 Aug 2020 22:46:27 GMT
ENV PATH=/opt/ol/wlp/bin:/opt/ol/docker/:/opt/ol/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ol/wlp/output WLP_SKIP_MAXPERMSIZE=true OPENJ9_SCC=true
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN /opt/ol/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 19 Aug 2020 22:46:28 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN mkdir /logs     && mkdir -p /opt/ol/wlp/usr/shared/resources/lib.index.cache     && ln -s /opt/ol/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p $WLP_OUTPUT_DIR/defaultServer     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ol/wlp/usr/servers/defaultServer /config     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && ln -s /opt/ol/wlp /liberty     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /opt/ol/wlp/usr     && chmod -R g+rw /opt/ol/wlp/usr     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rw /opt/ol/wlp/output     && chown -R 1001:0 /opt/ol/helpers     && chmod -R g+rw /opt/ol/helpers     && chown -R 1001:0 /opt/ol/fixes     && chmod -R g+rwx /opt/ol/fixes     && mkdir /etc/wlp     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && echo "<server description=\"Default Server\"><httpEndpoint id=\"defaultHttpEndpoint\" host=\"*\" /></server>" > /config/configDropins/defaults/open-default-port.xml
# Wed, 19 Aug 2020 22:46:43 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl200820200721-1900 LIBERTY_DOWNLOAD_URL=https://repo1.maven.org/maven2/io/openliberty/openliberty-runtime/20.0.0.8/openliberty-runtime-20.0.0.8.zip LIBERTY_SHA=24a590fc6e92273d6e35608d6bf23d4c45f91a63 LIBERTY_VERSION=20.0.0.8
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
# Wed, 19 Aug 2020 22:46:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ 
# Wed, 19 Aug 2020 22:46:44 GMT
USER 1001
# Wed, 19 Aug 2020 22:46:44 GMT
EXPOSE 9080 9443
# Wed, 19 Aug 2020 22:46:44 GMT
ENTRYPOINT ["/opt/ol/helpers/runtime/docker-server.sh"]
# Wed, 19 Aug 2020 22:46:45 GMT
CMD ["/opt/ol/wlp/bin/server" "run" "defaultServer"]
# Wed, 19 Aug 2020 22:46:53 GMT
RUN cp /opt/ol/wlp/templates/servers/javaee8/server.xml /config/server.xml
# Wed, 19 Aug 2020 22:47:16 GMT
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ol/wlp/output     && chmod -R g+rwx /opt/ol/wlp/output
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201a00e3942c21b28b0a9c8923d0cc0469da5d7cb95cd09f08b52650c8a559a2`  
		Last Modified: Wed, 19 Aug 2020 22:03:03 GMT  
		Size: 13.6 MB (13595628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a172b17642c4976ab19fd089c118bc5daf377f3a385fee3563d8af19598f2050`  
		Last Modified: Wed, 19 Aug 2020 22:05:35 GMT  
		Size: 48.4 MB (48386872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b611fd8ca23c160b4762d74a71c9cd634b4be59334c057b753ef115bae4fa3`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 8.4 KB (8380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6082ead0ee7fd5c965e9518845d895223681b0c395081b672e61f8609caae`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779a45a76e45c81bb2bd668adcc03deb55d44c66a727d5a5d873453a026b0b50`  
		Last Modified: Wed, 19 Aug 2020 22:49:45 GMT  
		Size: 157.8 MB (157847156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccc2d7faf8eb3abf7b4ce036697fd93cd747f4a743925d3bb2e15ac5f87983b`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 972.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadd59fcc56ef3a1cf58e38625ca4ea1cb83c64dfb48bed436b55ad040c19ce8`  
		Last Modified: Wed, 19 Aug 2020 22:49:38 GMT  
		Size: 9.5 KB (9495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5f8433ef858963b930e4ebb8360bf2fdb8d5eb829dac045a68b0ca29230d38`  
		Last Modified: Wed, 19 Aug 2020 22:49:39 GMT  
		Size: 7.5 MB (7491626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6810ce5a1c4bc7a1c60c6f4d422dbcf2fe75f9ec78f516ee244c874f98b56836`  
		Last Modified: Wed, 19 Aug 2020 22:49:51 GMT  
		Size: 965.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e59c06f29d6550fa79ae98c6540ed99bf540e00af155ff14140df006a62e3f`  
		Last Modified: Wed, 19 Aug 2020 22:49:53 GMT  
		Size: 16.3 MB (16276917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
