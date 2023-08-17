## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:507b9f50bafafb7f9f2eb761027f87ea1540c3129b216231498341f12c7f0239
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:8eda9b98fdd942107bdb7f71ba3bd71f78f87c815a4b7d8f9b8dfe2efd7dca51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191175246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac23e467a00728974e166ab645db29b15c3b41b586087259cf699aba60bdc9f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 06:43:31 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 17 Aug 2023 06:43:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 06:43:41 GMT
ENV JAVA_VERSION=8.0.8.6
# Thu, 17 Aug 2023 06:44:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2f173ec848303a99bcd38b0c13b1ddb2a70bb4ba9fa0e4ec5bd99268ff9987f8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cc637ac2d65386079932d06a303c244daa39282e514ba376cdb7fd0128cd05a5';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e510a98c183248a9ebbec0093958c5fc2f1dc126c792878e0bc739b44eaad7cd';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='7bd82044da06a852d373c20bac462cc60bc85355ca57c850b9d5b513c7b93768';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 17 Aug 2023 06:44:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 17 Aug 2023 08:11:04 GMT
USER root
# Thu, 17 Aug 2023 08:11:04 GMT
ARG VERBOSE=false
# Thu, 17 Aug 2023 08:11:04 GMT
ARG OPENJ9_SCC=true
# Thu, 17 Aug 2023 08:11:05 GMT
ARG LIBERTY_VERSION=23.0.0.7
# Thu, 17 Aug 2023 08:11:05 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Thu, 17 Aug 2023 08:11:05 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Thomas Watson, Wendy Raschke, Michal Broz org.opencontainers.image.vendor=IBM org.opencontainers.image.url=https://github.com/WASdev/ci.docker org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.7 org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 17 Aug 2023 08:11:05 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Thu, 17 Aug 2023 08:11:05 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.7 BuildLabel=cl230720230710-1201
# Thu, 17 Aug 2023 08:11:13 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     apt-get update;     apt-get install -y curl;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;     apt-get purge --auto-remove -y curl;     rm -rf /var/lib/apt/lists/*;
# Thu, 17 Aug 2023 08:11:13 GMT
ARG LIBERTY_URL
# Thu, 17 Aug 2023 08:11:13 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 17 Aug 2023 08:11:25 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml | grep -E "^\s*kernel:.*${LIBERTY_VERSION}\.zip" | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && cp -a /opt/ibm/wlp/lafiles/. /licenses/     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 08:11:25 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 17 Aug 2023 08:11:27 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ibm/wlp/usr/servers/defaultServer/server.env
# Thu, 17 Aug 2023 08:11:27 GMT
COPY file:7278f8f20139aab77b5c9fa76ad85e8a92836053c3ecfb9f5925f1a19788ef47 in /opt/ibm/NOTICES 
# Thu, 17 Aug 2023 08:11:27 GMT
COPY dir:40844bf0b1e39d0b6229e70ffb53eeccd3a0946186d4b924025fd748df62f886 in /opt/ibm/helpers/ 
# Thu, 17 Aug 2023 08:11:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 17 Aug 2023 08:11:27 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm/wlp /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 17 Aug 2023 08:11:34 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 17 Aug 2023 08:11:34 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 17 Aug 2023 08:11:34 GMT
USER 1001
# Thu, 17 Aug 2023 08:11:35 GMT
EXPOSE 9080 9443
# Thu, 17 Aug 2023 08:11:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 17 Aug 2023 08:11:35 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d80cb2eef8352f8d51cee0579d0d7e53c9b3089f0aedb190b60897ae6b2e9c9`  
		Last Modified: Thu, 17 Aug 2023 06:47:15 GMT  
		Size: 1.5 MB (1469099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c72a893cd7ea6dc738f115907dd0cfda6c30070e74450e33e477cc8f5bf2f8`  
		Last Modified: Thu, 17 Aug 2023 06:47:25 GMT  
		Size: 134.1 MB (134095787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbb44f3aacde54e0cf255b482da6c33cc43d88954fe45c736d23fbb19cc3c7b`  
		Last Modified: Thu, 17 Aug 2023 08:59:04 GMT  
		Size: 266.0 KB (265954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e9070a614f3a5467e1edefe838abee3ce01e33dff15a77292202b6dd05d55a`  
		Last Modified: Thu, 17 Aug 2023 08:59:05 GMT  
		Size: 19.3 MB (19321766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0e3b61ceade0164e094b7e342d10b0001936af73fe2a49f8965ee0e04ae4e9`  
		Last Modified: Thu, 17 Aug 2023 08:59:03 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1806ad5c82b2360ba32862dc49b7cdd5e12bc2328b783fd3d9b4b7b1e4c83c36`  
		Last Modified: Thu, 17 Aug 2023 08:59:01 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3f157d1ec71dcb2cac70f72a2546ef286d8da193ffed986d1bbd6d81bd202e`  
		Last Modified: Thu, 17 Aug 2023 08:59:01 GMT  
		Size: 11.1 KB (11078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb70f95563c4e936a0927cbb0479ba8fedd90daa44fc16315c2431e0c0372646`  
		Last Modified: Thu, 17 Aug 2023 08:59:01 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f371fd6b97894863e4b577e1a4f18b0e66d8e127f06b895e5db697bebe504f`  
		Last Modified: Thu, 17 Aug 2023 08:59:01 GMT  
		Size: 12.0 KB (12005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad347c29c16c1a8e21fdeebe707d2c40a4661f8c7da179ba1af81d28910726d`  
		Last Modified: Thu, 17 Aug 2023 08:59:01 GMT  
		Size: 5.6 MB (5559195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:2daea68b7f6c8389f98a01dfe8570e7d386d0f1e154fbb169b0a35d34679d2c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195900095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26749a38e2b9c39bcb12241dec45d06603604a7b4cf80823c3cee4ee969b1fde`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 00:34:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Jul 2023 00:34:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:34:51 GMT
ENV JAVA_VERSION=8.0.8.6
# Wed, 05 Jul 2023 00:39:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2f173ec848303a99bcd38b0c13b1ddb2a70bb4ba9fa0e4ec5bd99268ff9987f8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cc637ac2d65386079932d06a303c244daa39282e514ba376cdb7fd0128cd05a5';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e510a98c183248a9ebbec0093958c5fc2f1dc126c792878e0bc739b44eaad7cd';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='7bd82044da06a852d373c20bac462cc60bc85355ca57c850b9d5b513c7b93768';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Jul 2023 00:39:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 27 Jul 2023 19:44:21 GMT
USER root
# Thu, 27 Jul 2023 19:44:21 GMT
ARG VERBOSE=false
# Thu, 27 Jul 2023 19:44:22 GMT
ARG OPENJ9_SCC=true
# Sat, 29 Jul 2023 09:50:21 GMT
ARG LIBERTY_VERSION=23.0.0.7
# Sat, 29 Jul 2023 09:50:22 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Sat, 29 Jul 2023 09:50:22 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Thomas Watson, Wendy Raschke, Michal Broz org.opencontainers.image.vendor=IBM org.opencontainers.image.url=https://github.com/WASdev/ci.docker org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.7 org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 29 Jul 2023 09:50:22 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Sat, 29 Jul 2023 09:50:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.7 BuildLabel=cl230720230710-1201
# Sat, 29 Jul 2023 09:50:49 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     apt-get update;     apt-get install -y curl;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;     apt-get purge --auto-remove -y curl;     rm -rf /var/lib/apt/lists/*;
# Sat, 29 Jul 2023 09:50:50 GMT
ARG LIBERTY_URL
# Sat, 29 Jul 2023 09:50:51 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 29 Jul 2023 09:51:33 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml | grep -E "^\s*kernel:.*${LIBERTY_VERSION}\.zip" | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && cp -a /opt/ibm/wlp/lafiles/. /licenses/     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 09:51:33 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 29 Jul 2023 09:51:37 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ibm/wlp/usr/servers/defaultServer/server.env
# Sat, 29 Jul 2023 09:51:37 GMT
COPY file:7278f8f20139aab77b5c9fa76ad85e8a92836053c3ecfb9f5925f1a19788ef47 in /opt/ibm/NOTICES 
# Sat, 29 Jul 2023 09:51:38 GMT
COPY dir:40844bf0b1e39d0b6229e70ffb53eeccd3a0946186d4b924025fd748df62f886 in /opt/ibm/helpers/ 
# Sat, 29 Jul 2023 09:51:38 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 29 Jul 2023 09:51:39 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm/wlp /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 29 Jul 2023 09:51:52 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 29 Jul 2023 09:51:53 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Sat, 29 Jul 2023 09:51:53 GMT
USER 1001
# Sat, 29 Jul 2023 09:51:53 GMT
EXPOSE 9080 9443
# Sat, 29 Jul 2023 09:51:54 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 29 Jul 2023 09:51:54 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d286660db27a2dfe5334aaf1b48fcb9672ab1c6c043ae843eb0b98fa0524d`  
		Last Modified: Wed, 05 Jul 2023 00:44:32 GMT  
		Size: 1.6 MB (1576543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d31cd2ed994f1426e9333a8af6a1080a2e959f741da051ea9d4e1e15a9a2d13`  
		Last Modified: Wed, 05 Jul 2023 00:44:49 GMT  
		Size: 133.8 MB (133792026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec157088c7369f0b3986f7f507f877dfb0aaf9e1742935154e4b22aad91cbb9e`  
		Last Modified: Sat, 29 Jul 2023 10:49:59 GMT  
		Size: 270.4 KB (270357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38622a8a665c854212f9a9b8feaa19eac505f00337c86c3de834537a56d3c463`  
		Last Modified: Sat, 29 Jul 2023 10:50:01 GMT  
		Size: 19.3 MB (19322377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b39afd29abc57b2499dd62053baab003b00c519a522001d0390b51cb3a50a8`  
		Last Modified: Sat, 29 Jul 2023 10:49:59 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeaaf132362dd52ae4e80579d245d9b9436aa2efc4489966073eb0bfe5f961e9`  
		Last Modified: Sat, 29 Jul 2023 10:49:56 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f795006878d4f508352c85c595ecd2b3cdad2e6709481dea7a66ee86e0710354`  
		Last Modified: Sat, 29 Jul 2023 10:49:56 GMT  
		Size: 11.1 KB (11084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e807f08d851f006e34c21727ca0312ca1aa23bd721896f79adca7a1402491f`  
		Last Modified: Sat, 29 Jul 2023 10:49:56 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dbab7836691bf6e98b452e2330672d3c916e7b745b7cead4fabc66967d746e`  
		Last Modified: Sat, 29 Jul 2023 10:49:56 GMT  
		Size: 12.0 KB (12016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f888c5cb50785065ffae1a42a450b5cc222ba6e25d8df2c82b3f982221577931`  
		Last Modified: Sat, 29 Jul 2023 10:49:58 GMT  
		Size: 5.2 MB (5201806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:880fb56d8c7f37f7d7f12e701c6183409e3f5491f4c867d3adc07e38c6633e7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.9 MB (185933643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c001915591c4cbbe4757ec6cc951e1db6a3fe64bd58a53fb0d78480c6a009ad`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 09:47:06 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 16 Aug 2023 09:47:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:47:12 GMT
ENV JAVA_VERSION=8.0.8.6
# Wed, 16 Aug 2023 09:48:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2f173ec848303a99bcd38b0c13b1ddb2a70bb4ba9fa0e4ec5bd99268ff9987f8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cc637ac2d65386079932d06a303c244daa39282e514ba376cdb7fd0128cd05a5';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e510a98c183248a9ebbec0093958c5fc2f1dc126c792878e0bc739b44eaad7cd';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='7bd82044da06a852d373c20bac462cc60bc85355ca57c850b9d5b513c7b93768';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 16 Aug 2023 09:48:16 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 16 Aug 2023 17:57:15 GMT
USER root
# Wed, 16 Aug 2023 17:57:15 GMT
ARG VERBOSE=false
# Wed, 16 Aug 2023 17:57:16 GMT
ARG OPENJ9_SCC=true
# Wed, 16 Aug 2023 17:57:16 GMT
ARG LIBERTY_VERSION=23.0.0.7
# Wed, 16 Aug 2023 17:57:16 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Wed, 16 Aug 2023 17:57:16 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Thomas Watson, Wendy Raschke, Michal Broz org.opencontainers.image.vendor=IBM org.opencontainers.image.url=https://github.com/WASdev/ci.docker org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.7 org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 16 Aug 2023 17:57:16 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Wed, 16 Aug 2023 17:57:16 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.7 BuildLabel=cl230720230710-1201
# Wed, 16 Aug 2023 17:57:24 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     apt-get update;     apt-get install -y curl;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;     apt-get purge --auto-remove -y curl;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 17:57:24 GMT
ARG LIBERTY_URL
# Wed, 16 Aug 2023 17:57:24 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 16 Aug 2023 17:57:34 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml | grep -E "^\s*kernel:.*${LIBERTY_VERSION}\.zip" | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && cp -a /opt/ibm/wlp/lafiles/. /licenses/     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 17:57:36 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 16 Aug 2023 17:57:37 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ibm/wlp/usr/servers/defaultServer/server.env
# Wed, 16 Aug 2023 17:57:37 GMT
COPY file:7278f8f20139aab77b5c9fa76ad85e8a92836053c3ecfb9f5925f1a19788ef47 in /opt/ibm/NOTICES 
# Wed, 16 Aug 2023 17:57:37 GMT
COPY dir:40844bf0b1e39d0b6229e70ffb53eeccd3a0946186d4b924025fd748df62f886 in /opt/ibm/helpers/ 
# Wed, 16 Aug 2023 17:57:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 16 Aug 2023 17:57:38 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm/wlp /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 16 Aug 2023 17:57:43 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 16 Aug 2023 17:57:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 16 Aug 2023 17:57:44 GMT
USER 1001
# Wed, 16 Aug 2023 17:57:44 GMT
EXPOSE 9080 9443
# Wed, 16 Aug 2023 17:57:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 16 Aug 2023 17:57:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481198287db5a00cd86f00bf03a07297476d96af9492766f7515b515bd7486fa`  
		Last Modified: Wed, 16 Aug 2023 09:51:24 GMT  
		Size: 1.5 MB (1477116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2faaac9b3a57ee65dcc19fcbfa77a4b8fbc211b0b7936b9a8ceda769c9f6a91`  
		Last Modified: Wed, 16 Aug 2023 09:51:33 GMT  
		Size: 130.7 MB (130652775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ae75edd988d45ab0a19c0fab202c3f7966606e4bb945e95514951c960a4726`  
		Last Modified: Wed, 16 Aug 2023 18:45:56 GMT  
		Size: 267.4 KB (267416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c63452e1ce285da4fa398d4ea775fb11ee7bf80574968d14c8d096cef06f4f`  
		Last Modified: Wed, 16 Aug 2023 18:45:59 GMT  
		Size: 19.3 MB (19322099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee98c078484e33afdcd83b172d95442fc2733483d27e4c837e159840ecb8790`  
		Last Modified: Wed, 16 Aug 2023 18:45:56 GMT  
		Size: 611.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f12c204a5fe0f5bf1534d5395e97e1c40c3359bd6ad33ec57b30c800030f34`  
		Last Modified: Wed, 16 Aug 2023 18:45:55 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a01c598ddaa18a184b3000c8dc79fefaa9439276253a421dc72524104b17092`  
		Last Modified: Wed, 16 Aug 2023 18:45:55 GMT  
		Size: 11.1 KB (11083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5046a1e87b25c025df702887e543924dbf5125824a412d8ea71c5a8cc9caa6ea`  
		Last Modified: Wed, 16 Aug 2023 18:45:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5ddaf5c116048ff3db20871e4a98b253659023645f5e95815a320ddfb7094`  
		Last Modified: Wed, 16 Aug 2023 18:45:55 GMT  
		Size: 12.0 KB (12010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35246b2e8bf2d97f4e7d624f47a9ddc899c0051c23ec96260d7528471a9d4a7f`  
		Last Modified: Wed, 16 Aug 2023 18:45:56 GMT  
		Size: 5.5 MB (5544362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
