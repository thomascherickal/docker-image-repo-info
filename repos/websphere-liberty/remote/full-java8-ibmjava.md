## `websphere-liberty:full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:13054766e4cfca2e8a3344b05f66d7663810f8235461afac7c3eb0fc10b48c77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:fca6d33c7efcc2fb4d3442a7df891eaa3030c0bf39db96efb8227a03312cfe14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.8 MB (583837175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd24a3ad754a3fec4398bd9820380f0e7198fd5e459963713cf9281c9af8960`
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
# Mon, 21 Aug 2023 19:22:59 GMT
ENV JAVA_VERSION=8.0.8.10
# Mon, 21 Aug 2023 19:24:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='0ba3f228adc03c78d620a9d79a01d681a81dade244834b53d8f5456947b0e74b';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='8793ed949c728ebf5c28db8c6d43e17e0580ad95173a51624c9dc74d2b154680';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f4209abc6de52de6366ea771999eb0f420bb7132709455ca16438e0d4c3d4550';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='b84ce990439243beba14c3430a4072a8eab58bc9e41ca58f74efebdc64bc785c';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 21 Aug 2023 19:24:06 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 21 Aug 2023 22:34:49 GMT
USER root
# Mon, 21 Aug 2023 22:34:49 GMT
ARG VERBOSE=false
# Mon, 21 Aug 2023 22:34:49 GMT
ARG OPENJ9_SCC=true
# Mon, 21 Aug 2023 22:34:49 GMT
ARG LIBERTY_VERSION=23.0.0.7
# Mon, 21 Aug 2023 22:34:49 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Mon, 21 Aug 2023 22:34:50 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Thomas Watson, Wendy Raschke, Michal Broz org.opencontainers.image.vendor=IBM org.opencontainers.image.url=https://github.com/WASdev/ci.docker org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.7 org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Mon, 21 Aug 2023 22:34:50 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Mon, 21 Aug 2023 22:34:50 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.7 BuildLabel=cl230720230710-1201
# Mon, 21 Aug 2023 22:35:01 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     apt-get update;     apt-get install -y curl;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;     apt-get purge --auto-remove -y curl;     rm -rf /var/lib/apt/lists/*;
# Mon, 21 Aug 2023 22:35:01 GMT
ARG LIBERTY_URL
# Mon, 21 Aug 2023 22:35:01 GMT
ARG DOWNLOAD_OPTIONS=
# Mon, 21 Aug 2023 22:35:13 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml | grep -E "^\s*kernel:.*${LIBERTY_VERSION}\.zip" | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && cp -a /opt/ibm/wlp/lafiles/. /licenses/     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Mon, 21 Aug 2023 22:35:13 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Mon, 21 Aug 2023 22:35:14 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ibm/wlp/usr/servers/defaultServer/server.env
# Mon, 21 Aug 2023 22:35:14 GMT
COPY file:7278f8f20139aab77b5c9fa76ad85e8a92836053c3ecfb9f5925f1a19788ef47 in /opt/ibm/NOTICES 
# Mon, 21 Aug 2023 22:35:15 GMT
COPY dir:40844bf0b1e39d0b6229e70ffb53eeccd3a0946186d4b924025fd748df62f886 in /opt/ibm/helpers/ 
# Mon, 21 Aug 2023 22:35:15 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Mon, 21 Aug 2023 22:35:15 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm/wlp /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Mon, 21 Aug 2023 22:35:22 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Mon, 21 Aug 2023 22:35:22 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Mon, 21 Aug 2023 22:35:22 GMT
USER 1001
# Mon, 21 Aug 2023 22:35:22 GMT
EXPOSE 9080 9443
# Mon, 21 Aug 2023 22:35:22 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Mon, 21 Aug 2023 22:35:23 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Mon, 21 Aug 2023 22:35:35 GMT
ARG VERBOSE=false
# Mon, 21 Aug 2023 22:35:35 GMT
ARG REPOSITORIES_PROPERTIES=
# Mon, 21 Aug 2023 22:44:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN set -eux;   if [ ! -z "$REPOSITORIES_PROPERTIES" ]; then     mkdir /opt/ibm/wlp/etc/;     echo "$REPOSITORIES_PROPERTIES" > /opt/ibm/wlp/etc/repositories.properties;   fi;   installUtility install --acceptLicense baseBundle;   if [ ! -z "$REPOSITORIES_PROPERTIES" ]; then     rm /opt/ibm/wlp/etc/repositories.properties;   fi;   rm -rf /output/workarea /output/logs;   find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw;
# Mon, 21 Aug 2023 22:44:04 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Mon, 21 Aug 2023 22:44:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:c362fdbb5a459b13ed19a97e848dfdc64e14ce1c72ff7494e56ef8913411d293`  
		Last Modified: Mon, 21 Aug 2023 19:26:41 GMT  
		Size: 134.2 MB (134152601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19be6393107ef6115ae8e2ff28ce1f59f9bf16e8e958d118e49d8a9b160d893e`  
		Last Modified: Mon, 21 Aug 2023 22:47:12 GMT  
		Size: 266.0 KB (266014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c00bbd7b33e386442bf982273d1df4f9b9c1a138c6ce688407d8ec8962d2c77`  
		Last Modified: Mon, 21 Aug 2023 22:47:13 GMT  
		Size: 19.3 MB (19321793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64d1cb5eea6691a1da17e16f541d7e136b2321afa390f78a1551e0f2b0d94ca`  
		Last Modified: Mon, 21 Aug 2023 22:47:11 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e189ce41a2217507b7db9e99ef945086add0cdb6ac8f048490c034d336c1fda9`  
		Last Modified: Mon, 21 Aug 2023 22:47:09 GMT  
		Size: 1.5 KB (1522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e957df6ef3a092c301261dfdb8e99fdc131421ecbc60b87602289798b6348d88`  
		Last Modified: Mon, 21 Aug 2023 22:47:09 GMT  
		Size: 11.1 KB (11083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5138f195bc5163b9c7dfeb0242a181c88de9ae07aec9cb094368e7787d8e05`  
		Last Modified: Mon, 21 Aug 2023 22:47:10 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd319bd446e3d80ac326abf6bc35e8a24002e9d1d4e0525e92cad517e97ac7b6`  
		Last Modified: Mon, 21 Aug 2023 22:47:10 GMT  
		Size: 12.0 KB (12011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cedbf4ab84fe5ca2a75387c8dec07d9cb3821ca8671ba7b6b81e69d54a55773f`  
		Last Modified: Mon, 21 Aug 2023 22:47:10 GMT  
		Size: 5.5 MB (5517242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba79acf76dae8aeb154880c1b83930b4a0681e61a80674e3c48352ade1e49e5`  
		Last Modified: Mon, 21 Aug 2023 22:47:41 GMT  
		Size: 377.8 MB (377783378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5a2c438b1293f479a4c056b8b8a924ddf68923d8b2cd65f58bd97397cdb64b`  
		Last Modified: Mon, 21 Aug 2023 22:47:24 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baec278c7f0678f53c153374268ce2e0fe7dea8928571501c41d2b17b8008767`  
		Last Modified: Mon, 21 Aug 2023 22:47:26 GMT  
		Size: 14.9 MB (14862637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:c52b670b1809346d4a107290e68e4d9e1e9b6d18fcbd42cc6091b5a9b19c5c8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **586.6 MB (586627869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b12031d58b29dfbfd039c747236e3674677d0fd26ceb3fafe50c29615f7bfc2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 07:14:37 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 17 Aug 2023 07:15:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:15:05 GMT
ENV JAVA_VERSION=8.0.8.6
# Thu, 17 Aug 2023 07:16:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='2f173ec848303a99bcd38b0c13b1ddb2a70bb4ba9fa0e4ec5bd99268ff9987f8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cc637ac2d65386079932d06a303c244daa39282e514ba376cdb7fd0128cd05a5';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='e510a98c183248a9ebbec0093958c5fc2f1dc126c792878e0bc739b44eaad7cd';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='7bd82044da06a852d373c20bac462cc60bc85355ca57c850b9d5b513c7b93768';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 17 Aug 2023 07:16:27 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 17 Aug 2023 11:26:11 GMT
USER root
# Thu, 17 Aug 2023 11:26:11 GMT
ARG VERBOSE=false
# Thu, 17 Aug 2023 11:26:11 GMT
ARG OPENJ9_SCC=true
# Thu, 17 Aug 2023 11:26:12 GMT
ARG LIBERTY_VERSION=23.0.0.7
# Thu, 17 Aug 2023 11:26:12 GMT
ARG LIBERTY_BUILD_LABEL=cl230720230710-1201
# Thu, 17 Aug 2023 11:26:12 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Thomas Watson, Wendy Raschke, Michal Broz org.opencontainers.image.vendor=IBM org.opencontainers.image.url=https://github.com/WASdev/ci.docker org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.7 org.opencontainers.image.revision=cl230720230710-1201 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 17 Aug 2023 11:26:12 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Thu, 17 Aug 2023 11:26:13 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.7 BuildLabel=cl230720230710-1201
# Thu, 17 Aug 2023 11:26:30 GMT
# ARGS: LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN set -eux;     apt-get update;     apt-get install -y curl;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_aarch64';          DUMB_INIT_SHA256=b7d648f97154a99c539b63c55979cd29f005f88430fb383007fe3458340b795e;          ;;        amd64|x86_64)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_x86_64';          DUMB_INIT_SHA256=e874b55f3279ca41415d290c512a7ba9d08f98041b28ae7c2acb19a545f1c4df;          ;;        ppc64el|ppc64le)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_ppc64le';          DUMB_INIT_SHA256=3d15e80e29f0f4fa1fc686b00613a2220bc37e83a35283d4b4cca1fbd0a5609f;          ;;        s390x)          DUMB_INIT_URL='https://github.com/Yelp/dumb-init/releases/download/v1.2.5/dumb-init_1.2.5_s390x';          DUMB_INIT_SHA256=47e4601b152fc6dcb1891e66c30ecc62a2939fd7ffd1515a7c30f281cfec53b7;          ;;       *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /usr/bin/dumb-init ${DUMB_INIT_URL};     echo "${DUMB_INIT_SHA256} */usr/bin/dumb-init" | sha256sum -c -;     chmod +x /usr/bin/dumb-init;     apt-get purge --auto-remove -y curl;     rm -rf /var/lib/apt/lists/*;
# Thu, 17 Aug 2023 11:26:30 GMT
ARG LIBERTY_URL
# Thu, 17 Aug 2023 11:26:30 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 17 Aug 2023 11:26:48 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml | grep -E "^\s*kernel:.*${LIBERTY_VERSION}\.zip" | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && cp -a /opt/ibm/wlp/lafiles/. /licenses/     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 11:26:48 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 17 Aug 2023 11:26:51 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea     && rm -rf /opt/ibm/wlp/usr/servers/defaultServer/server.env
# Thu, 17 Aug 2023 11:26:51 GMT
COPY file:7278f8f20139aab77b5c9fa76ad85e8a92836053c3ecfb9f5925f1a19788ef47 in /opt/ibm/NOTICES 
# Thu, 17 Aug 2023 11:26:51 GMT
COPY dir:40844bf0b1e39d0b6229e70ffb53eeccd3a0946186d4b924025fd748df62f886 in /opt/ibm/helpers/ 
# Thu, 17 Aug 2023 11:26:52 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 17 Aug 2023 11:26:53 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm/wlp /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 17 Aug 2023 11:27:05 GMT
# ARGS: DOWNLOAD_OPTIONS= LIBERTY_BUILD_LABEL=cl230720230710-1201 LIBERTY_VERSION=23.0.0.7 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 17 Aug 2023 11:27:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 17 Aug 2023 11:27:06 GMT
USER 1001
# Thu, 17 Aug 2023 11:27:06 GMT
EXPOSE 9080 9443
# Thu, 17 Aug 2023 11:27:06 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 17 Aug 2023 11:27:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 17 Aug 2023 11:28:41 GMT
ARG VERBOSE=false
# Thu, 17 Aug 2023 11:28:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 17 Aug 2023 11:38:36 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN set -eux;   if [ ! -z "$REPOSITORIES_PROPERTIES" ]; then     mkdir /opt/ibm/wlp/etc/;     echo "$REPOSITORIES_PROPERTIES" > /opt/ibm/wlp/etc/repositories.properties;   fi;   installUtility install --acceptLicense baseBundle;   if [ ! -z "$REPOSITORIES_PROPERTIES" ]; then     rm /opt/ibm/wlp/etc/repositories.properties;   fi;   rm -rf /output/workarea /output/logs;   find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw;
# Thu, 17 Aug 2023 11:38:38 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 17 Aug 2023 11:39:32 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178c6af71882c03cbea1c4a79fb71458fc3e42c0589327d53c7ab2045de5bb83`  
		Last Modified: Thu, 17 Aug 2023 07:19:38 GMT  
		Size: 1.6 MB (1576539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e209ceabeba11764fc987f9e906485a5be674c5766e9d0e2bbf3fdba501699`  
		Last Modified: Thu, 17 Aug 2023 07:19:54 GMT  
		Size: 133.8 MB (133791919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7140b03f7f55d6afb254737ee5ffaca31396988edf8448765708b3f02fa3d`  
		Last Modified: Thu, 17 Aug 2023 12:26:18 GMT  
		Size: 270.4 KB (270388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83f531da811c0b900bfd5960853c7d94e2db9cbb0e99a90b21512a5be13a675`  
		Last Modified: Thu, 17 Aug 2023 12:26:20 GMT  
		Size: 19.3 MB (19322354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd70fdc1f0746e2cdad3664d36d71d4abb75d35cf12f9c99a3ae1ec3e5bda1b`  
		Last Modified: Thu, 17 Aug 2023 12:26:18 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0556d7d198844892c922cbf5b18becb1074589d703d36af7c9d47742bd88f8bb`  
		Last Modified: Thu, 17 Aug 2023 12:26:15 GMT  
		Size: 1.5 KB (1518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bbfed253fbcd5e795787098eb6d155d20527ff287c7af17435e649ef2bd95e`  
		Last Modified: Thu, 17 Aug 2023 12:26:15 GMT  
		Size: 11.1 KB (11075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21c0c1d3b2e7ce42f3adc9d58d7e8872332360c48cf3f3994c12dad347a6a53`  
		Last Modified: Thu, 17 Aug 2023 12:26:15 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef76ffe59bdf0da9dd0633fc6bf0a2b901ccc63953b9b9915ae802f10fb1ba74`  
		Last Modified: Thu, 17 Aug 2023 12:26:15 GMT  
		Size: 12.0 KB (12009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd10eb2f631ddeb319c291963de390797526862e028a7b371ea2b1e993f5f74`  
		Last Modified: Thu, 17 Aug 2023 12:26:17 GMT  
		Size: 5.2 MB (5222198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5bc72e9fae7f12b462f466c03462643ecbb281fede7f0b158267e986045966`  
		Last Modified: Thu, 17 Aug 2023 12:27:35 GMT  
		Size: 377.8 MB (377784042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423b6719e7ac1ca919d69f288800311bc5f92008ef1f09b3c8a5ff4f870dfc87`  
		Last Modified: Thu, 17 Aug 2023 12:27:02 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aded978eff6bbbc2a8945a25cd33ae9aca559045592bcb8390abe98fb8af72e`  
		Last Modified: Thu, 17 Aug 2023 12:27:06 GMT  
		Size: 12.9 MB (12921303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:4a9b99420141f44356a079127a1629f0634b0c3f51a3543d517eee61d64786f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **578.8 MB (578809702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f6da2f8b40fda71cc3396421b76c3a5f5187a3411edcc19a6f690c2cd7d7c4`
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
# Wed, 16 Aug 2023 17:58:45 GMT
ARG VERBOSE=false
# Wed, 16 Aug 2023 17:58:45 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 16 Aug 2023 18:07:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN set -eux;   if [ ! -z "$REPOSITORIES_PROPERTIES" ]; then     mkdir /opt/ibm/wlp/etc/;     echo "$REPOSITORIES_PROPERTIES" > /opt/ibm/wlp/etc/repositories.properties;   fi;   installUtility install --acceptLicense baseBundle;   if [ ! -z "$REPOSITORIES_PROPERTIES" ]; then     rm /opt/ibm/wlp/etc/repositories.properties;   fi;   rm -rf /output/workarea /output/logs;   find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw;
# Wed, 16 Aug 2023 18:07:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 16 Aug 2023 18:07:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:1a63e3ccf1966a6ab04de193374e43cffa302f7aacab04b47f22e930f5c754d6`  
		Last Modified: Wed, 16 Aug 2023 18:46:36 GMT  
		Size: 377.8 MB (377783727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb2e18949a370a19e3b1c7f8bc8f64a58fb19687cd90f37290a6b5d6ccb6ae2`  
		Last Modified: Wed, 16 Aug 2023 18:46:17 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965a6ec2db55ee5820b1481cefcd4df8951ffdac514320e7dfca12cf39107dcd`  
		Last Modified: Wed, 16 Aug 2023 18:46:19 GMT  
		Size: 15.1 MB (15091385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
