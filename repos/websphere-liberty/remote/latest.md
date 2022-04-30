## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:66a363171c734e9a28467158b345e6108678a6d95f8fe2c3094f94e81f201703
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:39ed29618ea9544340f9884293984e1af07d3ac667665cd03359b66b06b8dfa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.1 MB (460127021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8221788795cebf3551ab780b45ee8d46f59480986e0558b182e36a1e4650346`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:46:26 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 22 Apr 2022 02:46:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:46:34 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 22 Apr 2022 02:47:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='04b9e508ec9d206296b4972f1e122a168fc5f2524f7606ec3ade6600cef193a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d0fa8483f91717a478d3ae8cca82c8934966a7603287208da0ba6fd2261c544b';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2532804fa557187bb2b7a57d134b818b5cc9054cc3346d0b6ba93467e337fbdb';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='92323ebeb274e60f48f9301a8fe157382191927e50e97870cd9619461b527b5f';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='62e48b9b65d1266c017a890db6e5b3f24d28e543e04d1cf1ce553b280f9bf2c6';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 22 Apr 2022 02:47:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 22 Apr 2022 04:29:12 GMT
ARG VERBOSE=false
# Fri, 22 Apr 2022 04:29:12 GMT
ARG OPENJ9_SCC=true
# Fri, 22 Apr 2022 04:29:12 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Fri, 22 Apr 2022 04:29:13 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Fri, 22 Apr 2022 04:29:13 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Fri, 22 Apr 2022 04:29:13 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 22 Apr 2022 04:29:13 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Fri, 22 Apr 2022 04:29:13 GMT
ARG LIBERTY_URL
# Fri, 22 Apr 2022 04:29:13 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 22 Apr 2022 04:29:23 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:29:24 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 04:29:24 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Fri, 22 Apr 2022 04:29:24 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 22 Apr 2022 04:29:25 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 22 Apr 2022 04:29:25 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Fri, 22 Apr 2022 04:29:25 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 22 Apr 2022 04:29:26 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 22 Apr 2022 04:29:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 22 Apr 2022 04:29:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 22 Apr 2022 04:29:35 GMT
USER 1001
# Fri, 22 Apr 2022 04:29:35 GMT
EXPOSE 9080 9443
# Fri, 22 Apr 2022 04:29:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 22 Apr 2022 04:29:35 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 22 Apr 2022 04:30:27 GMT
ARG VERBOSE=false
# Fri, 22 Apr 2022 04:30:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 22 Apr 2022 04:34:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 22 Apr 2022 04:34:13 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 22 Apr 2022 04:34:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62da0fb33f1f956bb5cd7b0cd80748069becbe26b1ad9eada0d99f9f993c53a0`  
		Last Modified: Fri, 22 Apr 2022 02:48:52 GMT  
		Size: 3.0 MB (2960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce52da6e029d902a6851cb17baad356187b7cb727bd8fd2c51c48d1e13c60f20`  
		Last Modified: Fri, 22 Apr 2022 02:49:01 GMT  
		Size: 129.0 MB (129010215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db85f4d9e155401599941aca66c51a8924988c800b89ccbeff1244cec597091`  
		Last Modified: Fri, 22 Apr 2022 05:12:21 GMT  
		Size: 14.2 MB (14196097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8caee47663254be2ab0c000aeac86bd90e77ab45b4cc092d792f77b009650c8c`  
		Last Modified: Fri, 22 Apr 2022 05:12:17 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d2e5f9dea8b90fb929a7c1794d13712a339fb18439d42277095efd8a37c265`  
		Last Modified: Fri, 22 Apr 2022 05:12:17 GMT  
		Size: 9.7 KB (9676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7079155b663c5e006fd4964187da1b072dddaabbaa183f09b32f5b4cb9abcb33`  
		Last Modified: Fri, 22 Apr 2022 05:12:17 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f5fe67d71c53b0f19190d32992a87068b415c8f640d77abe9f250caea903a1`  
		Last Modified: Fri, 22 Apr 2022 05:12:17 GMT  
		Size: 10.7 KB (10663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434ba1d89b0e1246f288ee297057b7024345cf624430240d13d377c874d03add`  
		Last Modified: Fri, 22 Apr 2022 05:12:18 GMT  
		Size: 5.7 MB (5745286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d9856cc2f9abf48cfff908ebe04f1216c9445d16aace947584704b09cbe28`  
		Last Modified: Fri, 22 Apr 2022 05:13:03 GMT  
		Size: 265.2 MB (265214735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35f0dbe24df72d4645d475373e9d2bd9ecf88e09f2848c1a613fd73fd45825e`  
		Last Modified: Fri, 22 Apr 2022 05:12:49 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936f276c42232c2f4c558d95306869578ac7e9872a77ef89034de51f2ad0942c`  
		Last Modified: Fri, 22 Apr 2022 05:12:52 GMT  
		Size: 16.3 MB (16268505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:d33905280aa7e4be2346895da4392f39902c2c1741c340bac250da00f4fae6fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.0 MB (461041703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25626c050c44c08a02fbaa023d5696bf9a3293fbc39af071897093cb0414a93b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:03:42 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 22 Apr 2022 10:04:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:04:36 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 22 Apr 2022 10:05:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='04b9e508ec9d206296b4972f1e122a168fc5f2524f7606ec3ade6600cef193a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d0fa8483f91717a478d3ae8cca82c8934966a7603287208da0ba6fd2261c544b';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2532804fa557187bb2b7a57d134b818b5cc9054cc3346d0b6ba93467e337fbdb';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='92323ebeb274e60f48f9301a8fe157382191927e50e97870cd9619461b527b5f';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='62e48b9b65d1266c017a890db6e5b3f24d28e543e04d1cf1ce553b280f9bf2c6';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 22 Apr 2022 10:05:46 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 22 Apr 2022 11:29:14 GMT
ARG VERBOSE=false
# Fri, 22 Apr 2022 11:29:17 GMT
ARG OPENJ9_SCC=true
# Fri, 22 Apr 2022 11:29:20 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Fri, 22 Apr 2022 11:29:24 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Fri, 22 Apr 2022 11:29:26 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Fri, 22 Apr 2022 11:29:30 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 22 Apr 2022 11:29:35 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Fri, 22 Apr 2022 11:29:36 GMT
ARG LIBERTY_URL
# Fri, 22 Apr 2022 11:29:38 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 22 Apr 2022 11:30:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 11:30:23 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 11:30:27 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Fri, 22 Apr 2022 11:30:29 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 22 Apr 2022 11:30:47 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 22 Apr 2022 11:30:48 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Fri, 22 Apr 2022 11:30:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 22 Apr 2022 11:31:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 22 Apr 2022 11:31:21 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 22 Apr 2022 11:31:27 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 22 Apr 2022 11:31:30 GMT
USER 1001
# Fri, 22 Apr 2022 11:31:32 GMT
EXPOSE 9080 9443
# Fri, 22 Apr 2022 11:31:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 22 Apr 2022 11:31:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 22 Apr 2022 11:36:13 GMT
ARG VERBOSE=false
# Fri, 22 Apr 2022 11:36:15 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 22 Apr 2022 11:40:44 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 22 Apr 2022 11:40:55 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 22 Apr 2022 11:41:54 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6335837c025cb29531b7e6877b94805906b0badbb0e9a6b740b8f8790d328f8`  
		Last Modified: Fri, 22 Apr 2022 10:08:53 GMT  
		Size: 3.1 MB (3082171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0223ddd2905f573e2994ea5b8b008ce050316827c83f9585b4e86b487c147ace`  
		Last Modified: Fri, 22 Apr 2022 10:09:06 GMT  
		Size: 128.5 MB (128516363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2936e89a6e44075ca055819a1ccac18b956b74c216c9af396c03fdf774049b`  
		Last Modified: Fri, 22 Apr 2022 12:44:09 GMT  
		Size: 14.2 MB (14196604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b134f32652bcc7467bf683fe249e52192bfbc3451cded49083d1e50d11682a`  
		Last Modified: Fri, 22 Apr 2022 12:44:02 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75458e7a937f156c3914a040477c004e70fd8545f94a75843768228e849c88bf`  
		Last Modified: Fri, 22 Apr 2022 12:44:02 GMT  
		Size: 9.7 KB (9678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926fc24c3bd1eafaa1a9b757c4c8a17758021541885f68b3e2224a8be05358ad`  
		Last Modified: Fri, 22 Apr 2022 12:44:02 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f765cfe519143cacdb28d00d4e7fe06d517e0647e8ac113dd748513941efd20`  
		Last Modified: Fri, 22 Apr 2022 12:44:02 GMT  
		Size: 10.7 KB (10671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f25f10a55db308edd60a67ad965b7820df23ce76712c6a410407fc83d1ec5cb`  
		Last Modified: Fri, 22 Apr 2022 12:44:04 GMT  
		Size: 5.3 MB (5315783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6e6176c1089f3dafbbebb9353efb6c8dc382ca7d86c7616ab6fc8092a74058`  
		Last Modified: Fri, 22 Apr 2022 12:45:16 GMT  
		Size: 265.2 MB (265214955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6addf465143b9352ec294943a9f7fecf10bc5c78812daa8f198b556a442a905`  
		Last Modified: Fri, 22 Apr 2022 12:44:48 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adb8ac6b78cf603d70f2e6cfcb551373a11e62076597376cf1209b66a4db9e6`  
		Last Modified: Fri, 22 Apr 2022 12:44:51 GMT  
		Size: 14.3 MB (14251278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:da1648da9cd6b402387d63441828f661d1fe8a00632daf8582613efde13fa74d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **455.4 MB (455408408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f747386df299b6e924c0694a4af468b325d843209ee182f48740f5257a21ffd2`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:15 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 29 Apr 2022 23:27:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:27:22 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 29 Apr 2022 23:28:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='04b9e508ec9d206296b4972f1e122a168fc5f2524f7606ec3ade6600cef193a8';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d0fa8483f91717a478d3ae8cca82c8934966a7603287208da0ba6fd2261c544b';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='2532804fa557187bb2b7a57d134b818b5cc9054cc3346d0b6ba93467e337fbdb';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='92323ebeb274e60f48f9301a8fe157382191927e50e97870cd9619461b527b5f';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='62e48b9b65d1266c017a890db6e5b3f24d28e543e04d1cf1ce553b280f9bf2c6';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 29 Apr 2022 23:28:03 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Sat, 30 Apr 2022 01:14:41 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 01:14:41 GMT
ARG OPENJ9_SCC=true
# Sat, 30 Apr 2022 01:14:41 GMT
ARG EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851
# Sat, 30 Apr 2022 01:14:42 GMT
ARG NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e
# Sat, 30 Apr 2022 01:14:42 GMT
ARG NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024
# Sat, 30 Apr 2022 01:14:42 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.4 org.opencontainers.image.revision=cl220420220328-1303 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 30 Apr 2022 01:14:43 GMT
ENV LIBERTY_VERSION=22.0.0_04
# Sat, 30 Apr 2022 01:14:43 GMT
ARG LIBERTY_URL
# Sat, 30 Apr 2022 01:14:43 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 30 Apr 2022 01:14:57 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:14:58 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 01:14:58 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.4 BuildLabel=cl220420220328-1303
# Sat, 30 Apr 2022 01:14:59 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 30 Apr 2022 01:15:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 30 Apr 2022 01:15:01 GMT
COPY dir:b44499731da0f244ad2e27b60beff4f4cda216316903b60ecb41a7fba3784b48 in /opt/ibm/helpers/ 
# Sat, 30 Apr 2022 01:15:01 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 30 Apr 2022 01:15:03 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 30 Apr 2022 01:15:13 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1a343321d66ae6d10f502ae7198213b40ede1d1211bbc565cd02987b13e0b851 NON_IBM_SHA=47fb7794756b124cb5e2517c27444c7c772476121107bb5ecbfa87ceaf9bb91e NOTICES_SHA=eb3295e9c769d420c1472cf782a43ffdb82af42964492ca067ff7d44b6031024 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 30 Apr 2022 01:15:13 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Sat, 30 Apr 2022 01:15:14 GMT
USER 1001
# Sat, 30 Apr 2022 01:15:14 GMT
EXPOSE 9080 9443
# Sat, 30 Apr 2022 01:15:14 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 30 Apr 2022 01:15:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 30 Apr 2022 01:16:34 GMT
ARG VERBOSE=false
# Sat, 30 Apr 2022 01:16:35 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 30 Apr 2022 01:21:08 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Sat, 30 Apr 2022 01:21:13 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 30 Apr 2022 01:21:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:1347a7b069ceb0e131b6f229b7b96bae189f8e4c594c1933170e278d0ed928b2`  
		Last Modified: Fri, 29 Apr 2022 22:51:49 GMT  
		Size: 25.4 MB (25365828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f94c1c13b8b89cf54909fe9580987f60938a39e09f8c39697300c3a17a3ec1`  
		Last Modified: Fri, 29 Apr 2022 23:30:09 GMT  
		Size: 2.7 MB (2677016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06275ac2a17fcdc0af3d5fad5f5da24eb7ecf8a3004379b24dd0062489da9426`  
		Last Modified: Fri, 29 Apr 2022 23:30:17 GMT  
		Size: 126.0 MB (126023446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526431fa9dc5bd7d72595d46b6a45b3ffa7fa1487a9b1cbc98291113a2fe4f43`  
		Last Modified: Sat, 30 Apr 2022 02:07:13 GMT  
		Size: 14.2 MB (14196138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d56570d6faf829d691e509476a0a82fd2727f4c9fad51998666c386a64ba81`  
		Last Modified: Sat, 30 Apr 2022 02:07:11 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc6217d92d87c2e7f9645378f071e35d9baf752fbc5f267dbd679d5d7065dac`  
		Last Modified: Sat, 30 Apr 2022 02:07:11 GMT  
		Size: 9.7 KB (9681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6595126d065352c5e08b2db0e6ab23763266bc8f261c6097537f7abcbc5fefd`  
		Last Modified: Sat, 30 Apr 2022 02:07:11 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3123395afcb24dc24c8c88f0b8481a910de6035d254353c510adbb339e63244b`  
		Last Modified: Sat, 30 Apr 2022 02:07:12 GMT  
		Size: 10.7 KB (10664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a388ddf64e692cadd78fee704cda4b11738779305d329d56abf76a3ce58ac4fe`  
		Last Modified: Sat, 30 Apr 2022 02:07:12 GMT  
		Size: 5.9 MB (5901598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c5d187a773be752b6523f41f106f5faf6b26fe5601f525f14fa63378fd939a`  
		Last Modified: Sat, 30 Apr 2022 02:07:43 GMT  
		Size: 265.2 MB (265214801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7702d2096946bb1f97cc533de42665d3e179c6bc98da5e806c0043792f4cab89`  
		Last Modified: Sat, 30 Apr 2022 02:07:32 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7b61aee1dfbf667c522b80ef0b7f3fb4ef1ed2d62781e0d5f67b71033dc33d`  
		Last Modified: Sat, 30 Apr 2022 02:07:34 GMT  
		Size: 16.0 MB (16007314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
