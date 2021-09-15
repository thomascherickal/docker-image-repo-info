## `websphere-liberty:kernel-java11-openj9`

```console
$ docker pull websphere-liberty@sha256:fba6e1649bde8a5b5c4061f45234750c176fd0bd87bfeb90dc332e673b2e50a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java11-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:a3fdb7ed46d6b4bd06206c9e834d54a7ca7c8ac84ecbf2bc07d535dcb5a189de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109759872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0175b6c1c866656bf7bbba2f1492d94c3cb4c8df26e8068d3c64a6cad3e35a94`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:26:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:26:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:30:09 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Tue, 31 Aug 2021 02:31:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='f11ae15da7f2809caeeca70a7cf3b9e7f943848869f498f1b73efc10ef7170f0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='2d746296f743bdca55e3c391ddd5529c819e3b5193782085441c0078e1471406';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='152bf992d965ed018e9e1c3c2eb2c1771f92e0b6485b9a1f2c6d84d282117715';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:31:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:31:06 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 Aug 2021 02:31:42 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 Aug 2021 08:27:00 GMT
ARG VERBOSE=false
# Tue, 31 Aug 2021 08:27:00 GMT
ARG OPENJ9_SCC=true
# Tue, 31 Aug 2021 08:27:00 GMT
ARG EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5
# Tue, 31 Aug 2021 08:27:00 GMT
ARG NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a
# Tue, 31 Aug 2021 08:27:00 GMT
ARG NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e
# Tue, 31 Aug 2021 08:27:00 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.8 org.opencontainers.image.revision=cl210820210727-1323 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 31 Aug 2021 08:27:01 GMT
ENV LIBERTY_VERSION=21.0.0_08
# Tue, 31 Aug 2021 08:27:01 GMT
ARG LIBERTY_URL
# Tue, 31 Aug 2021 08:27:01 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 31 Aug 2021 08:27:09 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 08:27:09 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 08:27:09 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.8 BuildLabel=cl210820210727-1323
# Tue, 31 Aug 2021 08:27:09 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 31 Aug 2021 08:27:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 31 Aug 2021 08:27:11 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 31 Aug 2021 08:27:11 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 31 Aug 2021 08:27:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 31 Aug 2021 08:27:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 31 Aug 2021 08:27:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 31 Aug 2021 08:27:20 GMT
USER 1001
# Tue, 31 Aug 2021 08:27:20 GMT
EXPOSE 9080 9443
# Tue, 31 Aug 2021 08:27:21 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 31 Aug 2021 08:27:21 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d71b8f96bb4f1c00b7375be1090b56f03343a56b15fdcdf40d5ac4a207e217`  
		Last Modified: Tue, 31 Aug 2021 02:37:06 GMT  
		Size: 16.0 MB (16033698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331f7a510bc26accfdca19d6b781cac745d52177a44f2d00a25e22c62a6b0944`  
		Last Modified: Tue, 31 Aug 2021 02:41:27 GMT  
		Size: 44.4 MB (44382140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6374d9a272e0fd400a0dcaed489411c0bebbf287780709a62721d044c439e405`  
		Last Modified: Tue, 31 Aug 2021 02:41:21 GMT  
		Size: 4.1 MB (4075113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89cfdd53462293140b80067c051899db35b4ebc4577e8ff8fe72d0fd462aaf8`  
		Last Modified: Tue, 31 Aug 2021 08:52:59 GMT  
		Size: 14.2 MB (14160351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b0c99b9dc0a0338c8ec22dd1e00a698fe3461738a5b0ca5bcd9742f3e586ee`  
		Last Modified: Tue, 31 Aug 2021 08:52:55 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cd3ecac4fda4f840c5a759618f2b18cf7a5de9002c690e309274b09d824484`  
		Last Modified: Tue, 31 Aug 2021 08:52:54 GMT  
		Size: 9.7 KB (9670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ace3b8941cec33d2cb7c3476e842368656670c1c5a8c9b39d17806375791e3a`  
		Last Modified: Tue, 31 Aug 2021 08:52:55 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d031851cf071e25c8e5494049b3217e74cde8a17c113a4ca16ebe4c721ea2660`  
		Last Modified: Tue, 31 Aug 2021 08:52:55 GMT  
		Size: 10.7 KB (10654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49931af1adfa21ddee114a82e4c2e15a872b33dc6d25880289efcd6f2815ad6d`  
		Last Modified: Tue, 31 Aug 2021 08:52:55 GMT  
		Size: 2.5 MB (2517207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:fdc6dd76bc1418615bf34d2e5f16da4c281f25c1debcb8665d46c88636c80e0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115499633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c521132d604b08aa3fddd8e92fca9a7ff7bae02add6af1ef2730b08adda4f26b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:31:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:33:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:42:21 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Tue, 31 Aug 2021 02:44:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='f11ae15da7f2809caeeca70a7cf3b9e7f943848869f498f1b73efc10ef7170f0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='2d746296f743bdca55e3c391ddd5529c819e3b5193782085441c0078e1471406';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='152bf992d965ed018e9e1c3c2eb2c1771f92e0b6485b9a1f2c6d84d282117715';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:44:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:44:44 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 Aug 2021 02:45:27 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 Aug 2021 13:01:22 GMT
ARG VERBOSE=false
# Tue, 31 Aug 2021 13:01:24 GMT
ARG OPENJ9_SCC=true
# Tue, 31 Aug 2021 13:01:27 GMT
ARG EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5
# Tue, 31 Aug 2021 13:01:29 GMT
ARG NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a
# Tue, 31 Aug 2021 13:01:30 GMT
ARG NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e
# Tue, 31 Aug 2021 13:01:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.8 org.opencontainers.image.revision=cl210820210727-1323 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 31 Aug 2021 13:01:36 GMT
ENV LIBERTY_VERSION=21.0.0_08
# Tue, 31 Aug 2021 13:01:39 GMT
ARG LIBERTY_URL
# Tue, 31 Aug 2021 13:01:41 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 31 Aug 2021 13:02:18 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 13:02:20 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 13:02:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.8 BuildLabel=cl210820210727-1323
# Tue, 31 Aug 2021 13:02:25 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 31 Aug 2021 13:02:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 31 Aug 2021 13:02:42 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Tue, 31 Aug 2021 13:02:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 31 Aug 2021 13:02:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 31 Aug 2021 13:03:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=32d5a6d5092973394881e89884cca843222184438f329468a852d6fd3bc137c5 NON_IBM_SHA=57c70d10d8d72869c7e852a8f6521850d6a1c148875fae8b8099a4d3fad4832a NOTICES_SHA=ef2ab8d75bc030c0108825981a7a5e43972f2101d53e329fa0e211d5c5cbd64e VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 31 Aug 2021 13:03:20 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 31 Aug 2021 13:03:29 GMT
USER 1001
# Tue, 31 Aug 2021 13:03:33 GMT
EXPOSE 9080 9443
# Tue, 31 Aug 2021 13:03:38 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 31 Aug 2021 13:03:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6df1a3e21a26bf9e0775ad823e1762b00bf8c2a0650a891b7860b7fe18741a`  
		Last Modified: Tue, 31 Aug 2021 02:54:54 GMT  
		Size: 17.2 MB (17208636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bedb78bb4cd8318d7a6a8ebe3f7d69d8290741389f3f35077a25fdfd8c7f7c`  
		Last Modified: Tue, 31 Aug 2021 03:00:04 GMT  
		Size: 45.1 MB (45104809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac1b2ae26108e3759278e8d60be0ac46ef0ae3dcf52dbbaa7de94b551874c26`  
		Last Modified: Tue, 31 Aug 2021 02:59:58 GMT  
		Size: 3.3 MB (3257707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c9b27dc009bfc32117f7d9be7a9b9e4a02c77b456842b85c257d89e19e7dea`  
		Last Modified: Tue, 31 Aug 2021 13:26:15 GMT  
		Size: 14.2 MB (14160815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd49809138336c97d568b8a17eaddab6a5c2e3ab3ab5c9420f14c67eaf8331f`  
		Last Modified: Tue, 31 Aug 2021 13:26:10 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c13660b7324b101cc48f9408a9bf3754fd2099bb9d5ebeafc09f1773d0eeee`  
		Last Modified: Tue, 31 Aug 2021 13:26:11 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5b3c058554d21c971bb8350029f15ff9eb48f52a2c111dbf1a84b75e17f57a`  
		Last Modified: Tue, 31 Aug 2021 13:26:10 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d4cfedf29bdf152956d8dd8283adc12a24cfe8f7e1eab2db47779e320f63f7`  
		Last Modified: Tue, 31 Aug 2021 13:26:10 GMT  
		Size: 10.7 KB (10650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0225b2cb732ecb0ca26de7222f9b812150b9779aed863cadaaf5ce67b78ff118`  
		Last Modified: Tue, 31 Aug 2021 13:26:11 GMT  
		Size: 2.5 MB (2454590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java11-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:7ef9fa7f8906375b59ad0f6617207793bc87d7e560557e5e160b732bcbbb9bb2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107208422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a3d8b3bb0e0ab2b75e6e529dc56da17ac12a0789cbb46dcefc7ddb7c3c3ba9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:07:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:08:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:44 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Tue, 31 Aug 2021 02:15:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='f11ae15da7f2809caeeca70a7cf3b9e7f943848869f498f1b73efc10ef7170f0';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_ppc64le_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='2d746296f743bdca55e3c391ddd5529c819e3b5193782085441c0078e1471406';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_s390x_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='152bf992d965ed018e9e1c3c2eb2c1771f92e0b6485b9a1f2c6d84d282117715';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jre_x64_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:15:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:15:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 Aug 2021 02:15:41 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 Aug 2021 03:11:07 GMT
ARG VERBOSE=false
# Tue, 31 Aug 2021 03:11:07 GMT
ARG OPENJ9_SCC=true
# Wed, 15 Sep 2021 00:06:24 GMT
ARG EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a
# Wed, 15 Sep 2021 00:06:24 GMT
ARG NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0
# Wed, 15 Sep 2021 00:06:24 GMT
ARG NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755
# Wed, 15 Sep 2021 00:06:24 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter, Christy Jesuraj org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.9 org.opencontainers.image.revision=cl210920210824-2341 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with AdoptOpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 15 Sep 2021 00:06:24 GMT
ENV LIBERTY_VERSION=21.0.0_09
# Wed, 15 Sep 2021 00:06:24 GMT
ARG LIBERTY_URL
# Wed, 15 Sep 2021 00:06:25 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 15 Sep 2021 00:06:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 15 Sep 2021 00:06:33 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Sep 2021 00:06:33 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.9 BuildLabel=cl210920210824-2341
# Wed, 15 Sep 2021 00:06:33 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 15 Sep 2021 00:06:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 15 Sep 2021 00:06:34 GMT
COPY dir:489212918c9117d43d99cf93a14feddea56ce0482c252c77c33827f9d0160cb8 in /opt/ibm/helpers/ 
# Wed, 15 Sep 2021 00:06:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 15 Sep 2021 00:06:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 15 Sep 2021 00:06:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=5531853803b16c250b8c785873c9b095a9f5c295b62106ef026e2546d596a11a NON_IBM_SHA=1ebddca70b6f828f3c02b1bead777847da022dd2168c2f2448df0142321065a0 NOTICES_SHA=160afa9b79e037e552fb7901c30f9261b068d1be23ec7933b93206be02b3a755 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 15 Sep 2021 00:06:40 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Wed, 15 Sep 2021 00:06:40 GMT
USER 1001
# Wed, 15 Sep 2021 00:06:40 GMT
EXPOSE 9080 9443
# Wed, 15 Sep 2021 00:06:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 15 Sep 2021 00:06:41 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f47f4732fca5d50031ca6edf4776dd30d7e8eda1569ec50c3463d649acfc210`  
		Last Modified: Tue, 31 Aug 2021 02:23:22 GMT  
		Size: 15.7 MB (15741639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4506f4976a47d100e462ae4cca60d9201c251087630163685ae003e2488351d5`  
		Last Modified: Tue, 31 Aug 2021 02:26:46 GMT  
		Size: 43.8 MB (43840950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2a18ec44fd3128af9046bdf40def5a5736ad1a163083dbdfb3f7afbf7fb5d5`  
		Last Modified: Tue, 31 Aug 2021 02:26:41 GMT  
		Size: 3.9 MB (3865503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861802d95208c1997c46c6d0ed58198bba8bb1befb6dc2801873125a99ee78c3`  
		Last Modified: Wed, 15 Sep 2021 00:20:23 GMT  
		Size: 14.2 MB (14155043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16b56be074c021f2d4b2a7c4fb7b6fc797e1e9a747cba4585b635bb45c32226`  
		Last Modified: Wed, 15 Sep 2021 00:20:20 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5224607d2532ee24a1b917f1f0f571691f970265a066c94ea9caf56a11d5394`  
		Last Modified: Wed, 15 Sep 2021 00:20:20 GMT  
		Size: 9.7 KB (9673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d8b161c383447809e05cb38f2eb8dec42061a79cdc065cd858bb91036d2033`  
		Last Modified: Wed, 15 Sep 2021 00:20:20 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c465de7e9e9c2aa15ec1d43b91b3cf6969a8b278d2a1f157e632e6320663691c`  
		Last Modified: Wed, 15 Sep 2021 00:20:20 GMT  
		Size: 10.7 KB (10657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f1abc077e30217fbc7af338b9aceab0c477efe0045f5e5abb5071cdbd19f8d`  
		Last Modified: Wed, 15 Sep 2021 00:20:20 GMT  
		Size: 2.5 MB (2456520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
