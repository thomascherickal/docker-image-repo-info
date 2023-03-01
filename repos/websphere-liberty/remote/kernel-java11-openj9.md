## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:0be7aa63ab389c9e3af9ebff9c577487629e347ebd39844a74f79b6873a75be7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:3a3957e06c14f246c2024ab18fece4dd7a46ed6d072e0efdf34fbcecc0611293
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114323917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ae7f8533447feaf005ff9cc72671bbad3517aa30fafe6f54ce76f6765e1a487`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:00:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Feb 2023 19:01:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 19:02:59 GMT
ENV JAVA_VERSION=jdk-11.0.17+8_openj9-0.35.0
# Wed, 01 Feb 2023 19:04:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ab7f01a961559b49ce9b0a76af20191b7c047c6c1b6e5258e38f6c38de8cdc3f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_aarch64_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fba1dd9c25b0cce7efe124151b006624eeb2d2b0764284ca892d0e50ee457a41';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_ppc64le_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        amd64|x86_64)          ESUM='b1d31a4165cabcad66771a05acf8ff750f40953558494ba8d88e97fac55af6a9';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_x64_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        s390x)          ESUM='5f52184c9f4fff9ed628c12da4567162c8be77f4bcbc5939b6fe6e9d250b3798';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_s390x_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 01 Feb 2023 19:04:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Feb 2023 19:04:18 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 01 Feb 2023 19:04:54 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 02 Feb 2023 00:00:08 GMT
ARG VERBOSE=false
# Thu, 02 Feb 2023 00:00:08 GMT
ARG OPENJ9_SCC=true
# Fri, 10 Feb 2023 19:24:13 GMT
ARG EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e
# Fri, 10 Feb 2023 19:24:13 GMT
ARG NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5
# Fri, 10 Feb 2023 19:24:14 GMT
ARG NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1
# Fri, 10 Feb 2023 19:24:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.1 org.opencontainers.image.revision=cl230120230123-2118 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 10 Feb 2023 19:24:14 GMT
ENV LIBERTY_VERSION=23.0.0_1
# Fri, 10 Feb 2023 19:24:14 GMT
ARG LIBERTY_URL
# Fri, 10 Feb 2023 19:24:14 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 10 Feb 2023 19:24:29 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 19:24:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Fri, 10 Feb 2023 19:24:29 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.1 BuildLabel=cl230120230123-2118
# Fri, 10 Feb 2023 19:24:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 10 Feb 2023 19:24:30 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 10 Feb 2023 19:24:30 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Fri, 10 Feb 2023 19:24:30 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 10 Feb 2023 19:24:31 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 10 Feb 2023 19:24:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 10 Feb 2023 19:24:36 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 10 Feb 2023 19:24:37 GMT
USER 1001
# Fri, 10 Feb 2023 19:24:37 GMT
EXPOSE 9080 9443
# Fri, 10 Feb 2023 19:24:37 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 10 Feb 2023 19:24:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd590f15e5f87e6290f884ad85262183d7adecbfd0a298d1a443f8a177d71add`  
		Last Modified: Wed, 01 Feb 2023 19:10:30 GMT  
		Size: 16.0 MB (15995942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ee4255ee577b1c64299ffcee7ed33aea9a1fc0740db251a4054bc5ceac92be`  
		Last Modified: Wed, 01 Feb 2023 19:11:38 GMT  
		Size: 48.2 MB (48172744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2223646a84b35b53eeee1f522b66a7d98b2ae354fde67ad414d05bb146a45a26`  
		Last Modified: Wed, 01 Feb 2023 19:11:32 GMT  
		Size: 4.2 MB (4218659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8c1569b87d4094ba8cecdc24287921b9c8c1672befd25dac57611dd55508e`  
		Last Modified: Fri, 10 Feb 2023 20:46:01 GMT  
		Size: 14.8 MB (14753653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92439a070aa4a9d7b9fa0ba3c4c4afbb3df0ca2e015013dd1fb5947dfb67c1ee`  
		Last Modified: Fri, 10 Feb 2023 20:45:58 GMT  
		Size: 676.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cad63fe67b65fa09457a0e9ab1a42ecd934e512d161b48f3f6efd7c6ad7680`  
		Last Modified: Fri, 10 Feb 2023 20:45:58 GMT  
		Size: 9.8 KB (9751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c48f3467ab9e2340d0ff9cb582a3108f028d752149b64ae4f2f019ae83211a`  
		Last Modified: Fri, 10 Feb 2023 20:45:58 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1154c7dd10ad3516a2ed8cb8ec1786a3c45d8df8b172831091281d36ecbcaa`  
		Last Modified: Fri, 10 Feb 2023 20:45:58 GMT  
		Size: 10.7 KB (10730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539d82d83799b2e77aacb16ed2392ac4d1a80e2bc40d3c2db784f9c5b6167ac5`  
		Last Modified: Fri, 10 Feb 2023 20:45:59 GMT  
		Size: 2.6 MB (2583608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:2bdf0dd05410953cd66263dfccf8b2a0b67721c9c7d82b00e40715b52ad8b38f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120199733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac890637ce1bd72cf6631701d7ede145fb33d99323b4dbe4db5b8fda95d488b5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:30 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:31 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:34 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Wed, 01 Feb 2023 11:27:34 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:40:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Feb 2023 18:40:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:43:04 GMT
ENV JAVA_VERSION=jdk-11.0.17+8_openj9-0.35.0
# Wed, 01 Feb 2023 18:44:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ab7f01a961559b49ce9b0a76af20191b7c047c6c1b6e5258e38f6c38de8cdc3f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_aarch64_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fba1dd9c25b0cce7efe124151b006624eeb2d2b0764284ca892d0e50ee457a41';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_ppc64le_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        amd64|x86_64)          ESUM='b1d31a4165cabcad66771a05acf8ff750f40953558494ba8d88e97fac55af6a9';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_x64_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        s390x)          ESUM='5f52184c9f4fff9ed628c12da4567162c8be77f4bcbc5939b6fe6e9d250b3798';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.17%2B8_openj9-0.35.0/ibm-semeru-open-jre_s390x_linux_11.0.17_8_openj9-0.35.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 01 Feb 2023 18:44:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Feb 2023 18:44:29 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 01 Feb 2023 18:45:06 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 01 Feb 2023 21:52:19 GMT
ARG VERBOSE=false
# Wed, 01 Feb 2023 21:52:19 GMT
ARG OPENJ9_SCC=true
# Fri, 10 Feb 2023 04:15:53 GMT
ARG EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e
# Fri, 10 Feb 2023 04:15:54 GMT
ARG NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5
# Fri, 10 Feb 2023 04:15:54 GMT
ARG NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1
# Fri, 10 Feb 2023 04:15:55 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.1 org.opencontainers.image.revision=cl230120230123-2118 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 10 Feb 2023 04:15:55 GMT
ENV LIBERTY_VERSION=23.0.0_1
# Fri, 10 Feb 2023 04:15:56 GMT
ARG LIBERTY_URL
# Fri, 10 Feb 2023 04:15:56 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 10 Feb 2023 04:16:48 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 10 Feb 2023 04:16:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Fri, 10 Feb 2023 04:16:50 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.1 BuildLabel=cl230120230123-2118
# Fri, 10 Feb 2023 04:16:51 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 10 Feb 2023 04:16:53 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 10 Feb 2023 04:16:53 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Fri, 10 Feb 2023 04:16:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 10 Feb 2023 04:16:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 10 Feb 2023 04:17:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 10 Feb 2023 04:17:08 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Fri, 10 Feb 2023 04:17:08 GMT
USER 1001
# Fri, 10 Feb 2023 04:17:10 GMT
EXPOSE 9080 9443
# Fri, 10 Feb 2023 04:17:10 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 10 Feb 2023 04:17:11 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481cbd38c2d3559c559e39aaee6d3e9e7787b7af1d9a7ce35a8a392b075fb453`  
		Last Modified: Wed, 01 Feb 2023 18:51:57 GMT  
		Size: 17.2 MB (17168703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5767fd55acd577a01fec9e1c711043fad9db8934974e33a074e5c0a2186e5958`  
		Last Modified: Wed, 01 Feb 2023 18:53:37 GMT  
		Size: 48.9 MB (48936213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7306f15e60bf2ec91a63cbc7cf5d6ec8ed242981c1e683a475f1eda868044d03`  
		Last Modified: Wed, 01 Feb 2023 18:53:26 GMT  
		Size: 3.4 MB (3442688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dd1207c172c736d6ec29119297a1b4a5483dc0d6eb9142b17b0344eb0b29c9`  
		Last Modified: Fri, 10 Feb 2023 07:01:50 GMT  
		Size: 14.8 MB (14774779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd9fe3355ab20c67ed70d3dad9f7ded88f8f3ff8e9089e07a1fcbf3cf0625de`  
		Last Modified: Fri, 10 Feb 2023 07:01:46 GMT  
		Size: 679.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5399c2fdaf8141b005ddfce51cceaf068833965c9e1c5ed32950c3c85711e081`  
		Last Modified: Fri, 10 Feb 2023 07:01:46 GMT  
		Size: 9.8 KB (9753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52f32acabc9558ce7a62cdccf89628e81bdd934cfb158c55c85124e98da9913`  
		Last Modified: Fri, 10 Feb 2023 07:01:46 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9ae39ccd8fdd2f293bf03a35b1f10c60a5c5f7f7170a407cb079286b8f522b`  
		Last Modified: Fri, 10 Feb 2023 07:01:46 GMT  
		Size: 10.7 KB (10741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7acf3ab42269492a08af6adf939267c8220bcb46a2ef9e77b71fc263ad750fd5`  
		Last Modified: Fri, 10 Feb 2023 07:01:46 GMT  
		Size: 2.6 MB (2555562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d945d492e68e5664424f001b7b2cb23cc7e094339eafd6d0b8749ee79651a48d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.2 MB (112206881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf3366c6d19b5f3817de6dee6afb1dc8d60ca88b6d444578ab4cf23a9a07ae7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 01 Feb 2023 12:00:21 GMT
ARG RELEASE
# Wed, 01 Feb 2023 12:00:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 12:00:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 12:00:23 GMT
ADD file:4d5fa9b68af51e9c8cd7b25fb55ddd47256efb0b2eda9432507b72b7c1a17053 in / 
# Wed, 01 Feb 2023 12:00:24 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:23:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Feb 2023 18:23:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 00:21:46 GMT
ENV JAVA_VERSION=jdk-11.0.18+10_openj9-0.36.0
# Wed, 01 Mar 2023 00:23:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b7dae99808061eb1774e3af436453c48c30c01213a1613ca53df698276844f65';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_aarch64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f4eb9f501596a722a4be708361c1bfaa6b760cc7c885519d176cabba7a84d6e8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_ppc64le_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        amd64|x86_64)          ESUM='509a8c1e533c41896fddab187a8f6712ce1121d19eff71f4f023b58969147c9f';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_x64_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        s390x)          ESUM='ed6bbd482d9db361beb27510c5e88d882ba7232fc80409e35e33c08a5af7c7c0';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.18%2B10_openj9-0.36.1/ibm-semeru-open-jre_s390x_linux_11.0.18_10_openj9-0.36.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 01 Mar 2023 00:23:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 00:23:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 01 Mar 2023 00:24:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 01 Mar 2023 01:19:04 GMT
ARG VERBOSE=false
# Wed, 01 Mar 2023 01:19:04 GMT
ARG OPENJ9_SCC=true
# Wed, 01 Mar 2023 01:19:04 GMT
ARG EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e
# Wed, 01 Mar 2023 01:19:04 GMT
ARG NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5
# Wed, 01 Mar 2023 01:19:05 GMT
ARG NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1
# Wed, 01 Mar 2023 01:19:05 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.1 org.opencontainers.image.revision=cl230120230123-2118 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 01 Mar 2023 01:19:05 GMT
ENV LIBERTY_VERSION=23.0.0_1
# Wed, 01 Mar 2023 01:19:05 GMT
ARG LIBERTY_URL
# Wed, 01 Mar 2023 01:19:05 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 01 Mar 2023 01:19:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 01:19:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Wed, 01 Mar 2023 01:19:17 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.1 BuildLabel=cl230120230123-2118
# Wed, 01 Mar 2023 01:19:17 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 01 Mar 2023 01:19:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 01 Mar 2023 01:19:18 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 01 Mar 2023 01:19:18 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 01 Mar 2023 01:19:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 01 Mar 2023 01:19:22 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=dd3e1f52b274ac7551192d7ff07a2858396132ece9a26e8d3e8e28830e84183e NON_IBM_SHA=0a41a7fa840ccd132d68f0fc6138f573fe110dafaa36f2bcdeab9f2b495876a5 NOTICES_SHA=d4e03fe4b7d7492aba18a7ed449c0a5666258e4318c1a929042f53ed87abafa1 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 01 Mar 2023 01:19:22 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 01 Mar 2023 01:19:22 GMT
USER 1001
# Wed, 01 Mar 2023 01:19:22 GMT
EXPOSE 9080 9443
# Wed, 01 Mar 2023 01:19:22 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 01 Mar 2023 01:19:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:cbc0e1117f61ba365a9a02263b82c04f704d5d162aa31b25a9326797dd1c7084`  
		Last Modified: Tue, 31 Jan 2023 17:54:46 GMT  
		Size: 27.0 MB (27016130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32329c78fa891c29ef5b9df096b2cffaba8738e3e5a77aa5d7cb00958cf46491`  
		Last Modified: Wed, 01 Feb 2023 18:33:24 GMT  
		Size: 15.7 MB (15686940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8935a7e34d27cc150ec16df07fdf78aec18ac029b8b1b0134d5301b3e49c4abd`  
		Last Modified: Wed, 01 Mar 2023 00:32:41 GMT  
		Size: 47.7 MB (47746549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86271d0de72e52b072dc31c9af2ed315b5758bb764508a020c054fd91e0f45dd`  
		Last Modified: Wed, 01 Mar 2023 00:32:35 GMT  
		Size: 4.4 MB (4368581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5842abfb98f6f4cb09bbf007323bf7eddddf0ff59762f670011c678115334455`  
		Last Modified: Wed, 01 Mar 2023 02:10:15 GMT  
		Size: 14.8 MB (14755522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6950b2f09e972f0ca5d91a54e421ca8e1d7af5b9244e8e4b5c20ecbcce299628`  
		Last Modified: Wed, 01 Mar 2023 02:10:18 GMT  
		Size: 673.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b840d996fbe18cd3ce20896355e9a4df2995781c7b5fcc560810784edc517449`  
		Last Modified: Wed, 01 Mar 2023 02:10:12 GMT  
		Size: 9.8 KB (9752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4af5e1d0c5a9ac9904c950034a4f6b4ebf92d7029e17fa9d0c00cab860bc4b7`  
		Last Modified: Wed, 01 Mar 2023 02:10:12 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c732334d2cc022a990d1f5802f5f8b0a54b5815393446f06493b80af8ee6b8`  
		Last Modified: Wed, 01 Mar 2023 02:10:12 GMT  
		Size: 10.7 KB (10727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9693f65d7bbb9aa6d8fa543c23a26915eabc602daaaaf451de7b6296942957`  
		Last Modified: Wed, 01 Mar 2023 02:10:12 GMT  
		Size: 2.6 MB (2611737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
