## `websphere-liberty:kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:daa7d12e98d36fe64bb8ffe1396d32403f6baf7d2afb008986291600742210e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:de07e964f4d2b99a273f1d5ffae3acf85287515598e656d22df7132c89a68d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114021899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec73fcb0a6302fa9128956667ba086785f3d521543009f68e3654a654aae3860`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:12:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 03:01:36 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 03:03:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 03:03:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 03:03:08 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 03:03:43 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 07:29:52 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 07:29:52 GMT
ARG OPENJ9_SCC=true
# Tue, 07 Jun 2022 07:29:52 GMT
ARG EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8
# Tue, 07 Jun 2022 07:29:52 GMT
ARG NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47
# Tue, 07 Jun 2022 07:29:52 GMT
ARG NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759
# Tue, 07 Jun 2022 07:29:52 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.5 org.opencontainers.image.revision=cl220520220425-0301 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 07 Jun 2022 07:29:53 GMT
ENV LIBERTY_VERSION=22.0.0_05
# Tue, 07 Jun 2022 07:29:53 GMT
ARG LIBERTY_URL
# Tue, 07 Jun 2022 07:29:53 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 07 Jun 2022 07:30:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 07:30:02 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 07:30:02 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.5 BuildLabel=cl220520220425-0301
# Tue, 07 Jun 2022 07:30:02 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 07 Jun 2022 07:30:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 07 Jun 2022 07:30:04 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Tue, 07 Jun 2022 07:30:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 07 Jun 2022 07:30:05 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 07 Jun 2022 07:30:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 07 Jun 2022 07:30:13 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 07 Jun 2022 07:30:13 GMT
USER 1001
# Tue, 07 Jun 2022 07:30:13 GMT
EXPOSE 9080 9443
# Tue, 07 Jun 2022 07:30:13 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 07 Jun 2022 07:30:13 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caca7a4a00fe7d5efa72ecdbb346c7a4ee0e8e43c3a263d2bb79893d52bd4678`  
		Last Modified: Tue, 07 Jun 2022 00:19:21 GMT  
		Size: 16.0 MB (16029798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d02b90d4d9f1e0720f417ce2564200cb30804d3044ff23e657beb90aaae16`  
		Last Modified: Tue, 07 Jun 2022 03:09:14 GMT  
		Size: 47.8 MB (47754415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf77fc31a9a48f84b642dbad87196fdc478bdeb7ab123e80f2aedf1f1e01a1a4`  
		Last Modified: Tue, 07 Jun 2022 03:09:07 GMT  
		Size: 4.8 MB (4778262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9b55ad552221143ecdeea2975b3de326ab6af800d4e152c7ba7ffc2ba0c0a7`  
		Last Modified: Tue, 07 Jun 2022 08:39:22 GMT  
		Size: 14.3 MB (14285640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27992e7d840ee4307bf884e766b8315f7cf13214f651755adb9a1e12e502717`  
		Last Modified: Tue, 07 Jun 2022 08:39:18 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bf8098676ced38c13893cd67e5e951a7ce4aa241d501421c0d3987edf5c288`  
		Last Modified: Tue, 07 Jun 2022 08:39:19 GMT  
		Size: 9.7 KB (9672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c08263b0d0d87d8df83bd5763bfe5274710a4f03e6d8eacc0d28df7414bc34`  
		Last Modified: Tue, 07 Jun 2022 08:39:19 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d95cd0a61e31c78107343188cfea10dc34d6bdbd9e4f64fefc836d5a47027`  
		Last Modified: Tue, 07 Jun 2022 08:39:18 GMT  
		Size: 10.7 KB (10659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1811011eea660165e8a54dbec124cfa29f04526ac1c28784d9e1931a6ba12b`  
		Last Modified: Tue, 07 Jun 2022 08:39:19 GMT  
		Size: 2.6 MB (2579861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:9ecfa7a76d7c69e27d7b1989c01c83d1c371d0f33e43d9225119568294665750
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119459230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafd60a5f3188c2ffd3f00ff6abc8f64a1b0aeb31951c6ec10b695cbb42f321b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:29:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:32:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:35:07 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Sat, 30 Apr 2022 01:37:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 01:37:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 01:37:29 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 30 Apr 2022 01:38:16 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 30 Apr 2022 05:22:00 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 05:22:02 GMT
ARG OPENJ9_SCC=true
# Wed, 18 May 2022 02:57:03 GMT
ARG EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8
# Wed, 18 May 2022 02:57:06 GMT
ARG NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47
# Wed, 18 May 2022 02:57:09 GMT
ARG NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759
# Wed, 18 May 2022 02:57:13 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.5 org.opencontainers.image.revision=cl220520220425-0301 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 18 May 2022 02:57:16 GMT
ENV LIBERTY_VERSION=22.0.0_05
# Wed, 18 May 2022 02:57:18 GMT
ARG LIBERTY_URL
# Wed, 18 May 2022 02:57:22 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 18 May 2022 02:57:54 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 02:57:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 May 2022 02:58:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.5 BuildLabel=cl220520220425-0301
# Wed, 18 May 2022 02:58:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 18 May 2022 02:58:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 18 May 2022 02:58:28 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Wed, 18 May 2022 02:58:31 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 18 May 2022 02:58:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 18 May 2022 02:59:15 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 18 May 2022 02:59:24 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 18 May 2022 02:59:32 GMT
USER 1001
# Wed, 18 May 2022 02:59:36 GMT
EXPOSE 9080 9443
# Wed, 18 May 2022 02:59:39 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 18 May 2022 02:59:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436aa11f9f1d03225e672ec1f60e82ddcff2d3b267d9904213f0f01ed5eeba5`  
		Last Modified: Sat, 30 Apr 2022 00:45:44 GMT  
		Size: 17.2 MB (17204116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8c792b34d18de9373beaaa4adec0b0068cab8ff321cde143f0eaa2a05cb7d0`  
		Last Modified: Sat, 30 Apr 2022 01:47:24 GMT  
		Size: 48.1 MB (48115300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281ec4a02de94b8b58ce1680b236f20f463b157fcfdda7c5e25eb129cbc6d297`  
		Last Modified: Sat, 30 Apr 2022 01:47:16 GMT  
		Size: 3.7 MB (3705717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c395b7ce1658d721753048e62d9f054a86f0e9c0d0e84515d24b6bf2bf9f36c`  
		Last Modified: Wed, 18 May 2022 03:33:44 GMT  
		Size: 14.6 MB (14617092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a82392815556b414d7e2cfed34a8e1bbe0a3967910f000b8db20d8c92462111`  
		Last Modified: Wed, 18 May 2022 03:33:39 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8584d77479615e1e11e3351d0ffd6ffeb7b2b318f379a9e613a6aacf98acc496`  
		Last Modified: Wed, 18 May 2022 03:33:39 GMT  
		Size: 9.7 KB (9677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed76f2c686e6b74282e92c00cf3db637d9351c3f6c58bdbddde5a6df33925aab`  
		Last Modified: Wed, 18 May 2022 03:33:39 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ef69f1846327fd6a3176026c8c572b279d1ab5e150e10120f518296b9c2a23`  
		Last Modified: Wed, 18 May 2022 03:33:39 GMT  
		Size: 10.7 KB (10665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671d4c2abb210a42063ecf17b233983181f15736ffdf9483e91049db9a2902b5`  
		Last Modified: Wed, 18 May 2022 03:33:40 GMT  
		Size: 2.5 MB (2505025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:1f5bf692478526634b88913654c2950375695e21e051bf57c6abcd0d0e1449f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110852942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d581e20a51a2a97de025954de3af12e0d109d6e10b8dbda03e78b3f2df5cfc`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:11:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 06:11:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:17:40 GMT
ENV JAVA_VERSION=jdk-17.0.3+7_openj9-0.32.0
# Tue, 07 Jun 2022 06:18:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f899948ea0c5dc80a66f801db585939a25a4ae7e1f21a9a8f3bf3749c3baa87f';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9c54166490ac55a6bd26249b57eae5df4531635f4871e6642e7979affc894875';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='dad35fec82047e3a82c6e2dda8b53ee763b55aaedaed13b7b130856f4a3ffd35';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='4e2f631ad18c288e419db5c35295829dd7e83f4cd1be95252db06eb622b23090';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.3%2B7_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_17.0.3_7_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:18:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:18:56 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 07 Jun 2022 06:19:29 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 07 Jun 2022 08:05:41 GMT
ARG VERBOSE=false
# Tue, 07 Jun 2022 08:05:42 GMT
ARG OPENJ9_SCC=true
# Tue, 07 Jun 2022 08:05:42 GMT
ARG EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8
# Tue, 07 Jun 2022 08:05:43 GMT
ARG NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47
# Tue, 07 Jun 2022 08:05:44 GMT
ARG NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759
# Tue, 07 Jun 2022 08:05:44 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.5 org.opencontainers.image.revision=cl220520220425-0301 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 07 Jun 2022 08:05:45 GMT
ENV LIBERTY_VERSION=22.0.0_05
# Tue, 07 Jun 2022 08:05:46 GMT
ARG LIBERTY_URL
# Tue, 07 Jun 2022 08:05:46 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 07 Jun 2022 08:06:04 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:06:06 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 08:06:07 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.5 BuildLabel=cl220520220425-0301
# Tue, 07 Jun 2022 08:06:08 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 07 Jun 2022 08:06:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 07 Jun 2022 08:06:11 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Tue, 07 Jun 2022 08:06:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 07 Jun 2022 08:06:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 07 Jun 2022 08:06:27 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=2c85b0e69fa3b281919e9db592846585762fc82a6cad058d53fa484013aaf4b8 NON_IBM_SHA=6e08202f7be09eb4e05a2e754285812724e169318596248763ff833e85a27b47 NOTICES_SHA=afc4329090afc2b5913c49afb9866137497bce169a2ca71e36c7e74ed6945759 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 07 Jun 2022 08:06:29 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 07 Jun 2022 08:06:29 GMT
USER 1001
# Tue, 07 Jun 2022 08:06:30 GMT
EXPOSE 9080 9443
# Tue, 07 Jun 2022 08:06:31 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 07 Jun 2022 08:06:31 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908ba35702b3545e3156e807426eb36d13103c223acf51195f236f759910d212`  
		Last Modified: Tue, 07 Jun 2022 06:23:28 GMT  
		Size: 15.7 MB (15730049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897655bd3c7dec4efa7a0e8f8ecf3ec7f54efab8f9b298a61832098ce76e6e79`  
		Last Modified: Tue, 07 Jun 2022 06:25:38 GMT  
		Size: 46.2 MB (46241852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c178a5f949ecd320fb5c874b177b6bd44cfe054338cc4cdb12476990dbc1a17`  
		Last Modified: Tue, 07 Jun 2022 06:25:32 GMT  
		Size: 4.9 MB (4868988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75d4d97aec6f5d474c35c5c127f3984fb890a927dedc0c4e63f9a9dbff7bb34`  
		Last Modified: Tue, 07 Jun 2022 09:27:52 GMT  
		Size: 14.3 MB (14285734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14afa2e857465a3bf36a8d29ce7953399808bfa7e977939f921c0dfb7bdd837a`  
		Last Modified: Tue, 07 Jun 2022 09:27:50 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56a08a4dd70ef18efb2345ab7e61f2216aa5702e0781f6c6be48dface7ab9d1`  
		Last Modified: Tue, 07 Jun 2022 09:27:50 GMT  
		Size: 9.7 KB (9675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0594fc1efbcde9c460abe48f7bc8797be65152ee44d2d62e316f1f1c3e8c6f88`  
		Last Modified: Tue, 07 Jun 2022 09:27:50 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab28d83826ab8117061e1bc918dd92f6ffa53fe3c80f8841e8549d7f7df6602`  
		Last Modified: Tue, 07 Jun 2022 09:27:50 GMT  
		Size: 10.7 KB (10658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f931b50f1a3903a7672f55f1dd40299709b6a55da2cec7500e7ee0586c25ca09`  
		Last Modified: Tue, 07 Jun 2022 09:27:51 GMT  
		Size: 2.6 MB (2649005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
