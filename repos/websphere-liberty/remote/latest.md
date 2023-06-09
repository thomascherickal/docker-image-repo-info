## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:5e2e07036920fca6c24cdd5e1a77dc1106054cc716ddf49de6b9530c6993aed8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:04d76b1727866a4204dcf9b3394a83eb1d5f14e75f3750b1aa74c987a8727e43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.3 MB (566307319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2544f1017320ec2b17f354b5a662a2e9a8d6435dab2e643525e1332e68a780a9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:03:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 02 Jun 2023 01:03:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Jun 2023 22:19:43 GMT
ENV JAVA_VERSION=8.0.8.5
# Tue, 06 Jun 2023 22:20:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6e2520c98e5fdca4a62f867b4dba1c5ade37fb32a60416de624ac7f7293bb52c';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c6400df29efd094dab907331b9954b4e75e8bd587df17be6226882e77dd48436';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f4a7dffcda42adbd0e98c2e37072e6dc00aff0ebb0344f59e1545896f14a9065';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='91ed937391e37feb42c70ce45d2ef6138e411cfd4162b8b8b9483349764044e9';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 06 Jun 2023 22:20:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 06 Jun 2023 22:42:28 GMT
ARG VERBOSE=false
# Tue, 06 Jun 2023 22:42:28 GMT
ARG OPENJ9_SCC=true
# Fri, 09 Jun 2023 06:52:16 GMT
ARG EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3
# Fri, 09 Jun 2023 06:52:17 GMT
ARG NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11
# Fri, 09 Jun 2023 06:52:17 GMT
ARG NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997
# Fri, 09 Jun 2023 06:52:17 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.5 org.opencontainers.image.revision=cl230520230514-1901 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 09 Jun 2023 06:52:17 GMT
ENV LIBERTY_VERSION=23.0.0_05
# Fri, 09 Jun 2023 06:52:17 GMT
ARG LIBERTY_URL
# Fri, 09 Jun 2023 06:52:17 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 09 Jun 2023 06:52:32 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Jun 2023 06:52:32 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Fri, 09 Jun 2023 06:52:32 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.5 BuildLabel=cl230520230514-1901
# Fri, 09 Jun 2023 06:52:33 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 09 Jun 2023 06:52:34 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 09 Jun 2023 06:52:34 GMT
COPY dir:914bfb97242d950c6caece0b64a51887f4841dba2f2ab4120f6cb39eedace555 in /opt/ibm/helpers/ 
# Fri, 09 Jun 2023 06:52:34 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 09 Jun 2023 06:52:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 09 Jun 2023 06:52:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 09 Jun 2023 06:52:42 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 09 Jun 2023 06:52:42 GMT
USER 1001
# Fri, 09 Jun 2023 06:52:42 GMT
EXPOSE 9080 9443
# Fri, 09 Jun 2023 06:52:42 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 09 Jun 2023 06:52:42 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 09 Jun 2023 06:53:43 GMT
ARG VERBOSE=false
# Fri, 09 Jun 2023 06:53:43 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 09 Jun 2023 07:02:49 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 09 Jun 2023 07:02:50 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 09 Jun 2023 07:03:18 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db07816b3aab4d393ea40ce80939a39026f25e04db32332ddbf7503eb707995`  
		Last Modified: Fri, 02 Jun 2023 01:07:16 GMT  
		Size: 1.5 MB (1468716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de71424202e6f4b89cb501a2262080e0b7c75655bb452706fd12793892298bf`  
		Last Modified: Tue, 06 Jun 2023 22:23:21 GMT  
		Size: 134.0 MB (134046792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b77ba303fc9128652d5d836f1d27f92936102b3d6e51dfba4ba63ceff42e372`  
		Last Modified: Fri, 09 Jun 2023 08:22:59 GMT  
		Size: 18.9 MB (18938666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5beee20f83cf39c5da69f264bf4ce3f0e3154ff713bd1cd4049efc374fac0c7c`  
		Last Modified: Fri, 09 Jun 2023 08:22:55 GMT  
		Size: 681.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2611de69506065c3eec0f21ce13bd7fbb940e09155169c8509408aa7ebe6b913`  
		Last Modified: Fri, 09 Jun 2023 08:22:55 GMT  
		Size: 10.5 KB (10538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063e37f3afe9097f5a3fd516f987d8530b639b4a4dc27a886ab2c172a48447e8`  
		Last Modified: Fri, 09 Jun 2023 08:22:55 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:856996156604eec0621fb26d7032682f0275c3173a284dac2046814dd2a4fcae`  
		Last Modified: Fri, 09 Jun 2023 08:22:56 GMT  
		Size: 11.5 KB (11524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd15d7546a411578b6d8b039da498afcab39b9cbf0f4e59f3cd739d15fc6d3e6`  
		Last Modified: Fri, 09 Jun 2023 08:22:57 GMT  
		Size: 6.0 MB (5979517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82449716dddd345357f1907c88b82fe43ca1db9952b64194d985aa63b47c5d32`  
		Last Modified: Fri, 09 Jun 2023 08:24:01 GMT  
		Size: 359.2 MB (359248908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f22249cff8e8f832b176d04fc7df99f770e20cb0d70f7d56629defb52ed966e`  
		Last Modified: Fri, 09 Jun 2023 08:23:23 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2858c541f6ba424426d1add209bbe7504fd2782074c9c7f36ba146a8687b61`  
		Last Modified: Fri, 09 Jun 2023 08:23:26 GMT  
		Size: 16.2 MB (16170479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:b7516b9f63c31319868b8e53e466ac89e1459908edff9cc2d8d2e5fbb281c1f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **563.7 MB (563688506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d2f7e5bd0abf6b44479c5cc14037a6fdb9751c84567c924d99406712736bd5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:17 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:18 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:21 GMT
ADD file:e75f08a67f0576b5441bb2fe454cad4b5b31a9d4efea23be791af62e1e0c712f in / 
# Tue, 25 Apr 2023 17:30:21 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 14:09:46 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 04 May 2023 14:09:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 14:09:58 GMT
ENV JAVA_VERSION=8.0.8.0
# Thu, 04 May 2023 14:12:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='39cf0ebeda2461c0ee81636d745643713a37863d729784c46a48b4eded4717fb';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='bef3e93e4b1025e8350492fed0f6a5a743a2d35fbacdb7820cc539d24c891a4e';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='87d22ee3d2e20faa9854044aa46bf6be5d39f8ceb9ccf91574c7518f2535dfcb';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='227ada7516542c170a920bc78a416c1dc492cba4321a23f42bd7e640ddc890e5';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 04 May 2023 14:12:40 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 04 May 2023 20:36:44 GMT
ARG VERBOSE=false
# Thu, 04 May 2023 20:36:44 GMT
ARG OPENJ9_SCC=true
# Thu, 04 May 2023 20:36:45 GMT
ARG EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093
# Thu, 04 May 2023 20:36:45 GMT
ARG NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0
# Thu, 04 May 2023 20:36:46 GMT
ARG NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925
# Thu, 04 May 2023 20:36:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.4 org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 04 May 2023 20:36:46 GMT
ENV LIBERTY_VERSION=23.0.0_04
# Thu, 04 May 2023 20:36:47 GMT
ARG LIBERTY_URL
# Thu, 04 May 2023 20:36:47 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 04 May 2023 20:37:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 20:37:47 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Thu, 04 May 2023 20:37:48 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.4 BuildLabel=cl230420230418-0035
# Thu, 04 May 2023 20:37:49 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 04 May 2023 20:37:52 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 04 May 2023 20:37:53 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Thu, 04 May 2023 20:37:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 04 May 2023 20:37:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 04 May 2023 20:38:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 04 May 2023 20:38:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Thu, 04 May 2023 20:38:12 GMT
USER 1001
# Thu, 04 May 2023 20:38:13 GMT
EXPOSE 9080 9443
# Thu, 04 May 2023 20:38:13 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 04 May 2023 20:38:14 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 04 May 2023 20:40:59 GMT
ARG VERBOSE=false
# Thu, 04 May 2023 20:40:59 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 04 May 2023 20:58:27 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Thu, 04 May 2023 20:58:34 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 04 May 2023 20:59:33 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f6a63d8cd043e76933823b18cbb7057a55bb4d66d64639c81e15a4700c101582`  
		Last Modified: Wed, 03 May 2023 17:09:07 GMT  
		Size: 35.7 MB (35712706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8e1caab24446aefe2b3b975cf39a80aad52df873c970c64a0a65cc82be5c0`  
		Last Modified: Thu, 04 May 2023 14:18:24 GMT  
		Size: 1.6 MB (1552398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908bd1b1e780377c2830ba296a4cfccc03d4b7967bc41aa767ee6ceaff2f3c81`  
		Last Modified: Thu, 04 May 2023 14:18:40 GMT  
		Size: 133.6 MB (133556002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9a74370575a86e9f95e058cc76d142c181ec03c33549d91aa8cfddd3cf2684`  
		Last Modified: Thu, 04 May 2023 22:18:19 GMT  
		Size: 14.3 MB (14347328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2b0d60d8cb06c021333c2471482bf3b5563e5adb6e1b6e9533b825f599fb5`  
		Last Modified: Thu, 04 May 2023 22:18:15 GMT  
		Size: 686.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a1645074458f91da133ecfb817d5383f696deb45e621ee37eb6fd97f3c435d`  
		Last Modified: Thu, 04 May 2023 22:18:15 GMT  
		Size: 9.8 KB (9820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60f8ac5608ae99431256430cb2be8d76f089d357e5d7d02ed4d4114973cadcc`  
		Last Modified: Thu, 04 May 2023 22:18:15 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c0b4d609715fb8d5995fb12809143fc9b60063cf0dd006a989ec1d798368e6`  
		Last Modified: Thu, 04 May 2023 22:18:15 GMT  
		Size: 10.8 KB (10815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f1527abf00b71338e5918e32e507ebca56d3ab76451eda62b5ed0f9e1397e9`  
		Last Modified: Thu, 04 May 2023 22:18:16 GMT  
		Size: 5.5 MB (5497161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c26992b9bcceb8a0eaa0a0cd4d85734756089956abdca3b89586ad202075fa7`  
		Last Modified: Thu, 04 May 2023 22:19:17 GMT  
		Size: 359.1 MB (359072976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a9df0ecd43754edf5ef7ce8031c46f7d1c3130aec4c5edf852cf9108f658919`  
		Last Modified: Thu, 04 May 2023 22:18:47 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58c9ec8fc0af5fd039ba632cc2d99d228350c7e1e2e56f6a63749b735f6332a`  
		Last Modified: Thu, 04 May 2023 22:18:51 GMT  
		Size: 13.9 MB (13927389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:49d7cf04cf4a465e5444492acc67924ddc890258191e158e7cdfe563f1cd424c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **560.8 MB (560795480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0a384ce7b70ebe4d41089922cd109b9b12c2736c1b4706b2601bae6c04e402b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 22 May 2023 17:46:45 GMT
ARG RELEASE
# Mon, 22 May 2023 17:46:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:46:45 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:46:47 GMT
ADD file:7bf1b7a1484e37f289d40f5c1c1cbe321ef337f898dd3d5809193c848a9a3dc2 in / 
# Mon, 22 May 2023 17:46:47 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 14:39:20 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 02 Jun 2023 14:39:28 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 06 Jun 2023 22:44:26 GMT
ENV JAVA_VERSION=8.0.8.5
# Tue, 06 Jun 2023 22:45:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6e2520c98e5fdca4a62f867b4dba1c5ade37fb32a60416de624ac7f7293bb52c';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c6400df29efd094dab907331b9954b4e75e8bd587df17be6226882e77dd48436';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='f4a7dffcda42adbd0e98c2e37072e6dc00aff0ebb0344f59e1545896f14a9065';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='91ed937391e37feb42c70ce45d2ef6138e411cfd4162b8b8b9483349764044e9';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 06 Jun 2023 22:45:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Tue, 06 Jun 2023 23:26:24 GMT
ARG VERBOSE=false
# Tue, 06 Jun 2023 23:26:24 GMT
ARG OPENJ9_SCC=true
# Fri, 09 Jun 2023 04:24:16 GMT
ARG EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3
# Fri, 09 Jun 2023 04:24:16 GMT
ARG NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11
# Fri, 09 Jun 2023 04:24:16 GMT
ARG NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997
# Fri, 09 Jun 2023 04:24:17 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.5 org.opencontainers.image.revision=cl230520230514-1901 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://ibm.biz/wl-app-image-template org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 09 Jun 2023 04:24:17 GMT
ENV LIBERTY_VERSION=23.0.0_05
# Fri, 09 Jun 2023 04:24:17 GMT
ARG LIBERTY_URL
# Fri, 09 Jun 2023 04:24:17 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 09 Jun 2023 04:24:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Jun 2023 04:24:35 GMT
ENV PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Fri, 09 Jun 2023 04:24:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.5 BuildLabel=cl230520230514-1901
# Fri, 09 Jun 2023 04:24:36 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 09 Jun 2023 04:24:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 09 Jun 2023 04:24:37 GMT
COPY dir:914bfb97242d950c6caece0b64a51887f4841dba2f2ab4120f6cb39eedace555 in /opt/ibm/helpers/ 
# Fri, 09 Jun 2023 04:24:37 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 09 Jun 2023 04:24:38 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/fixes /fixes     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 09 Jun 2023 04:24:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=16669604ed86a6ad4bd60b99ca85fad2a819ae3ff3e68d5585a64f3d51504ee3 NON_IBM_SHA=89faf793b9e068a80bda72d6c1cbf9b4e1362c699525710ae3247a6c135a0b11 NOTICES_SHA=f02cefd8eb429cd471b9f494c2ac7f3df10ef042f1b7e8271895afd2a46ae997 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 09 Jun 2023 04:24:44 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Fri, 09 Jun 2023 04:24:45 GMT
USER 1001
# Fri, 09 Jun 2023 04:24:45 GMT
EXPOSE 9080 9443
# Fri, 09 Jun 2023 04:24:45 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 09 Jun 2023 04:24:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 09 Jun 2023 04:25:46 GMT
ARG VERBOSE=false
# Fri, 09 Jun 2023 04:25:46 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 09 Jun 2023 04:35:28 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Fri, 09 Jun 2023 04:35:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 09 Jun 2023 04:36:16 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:f2957179c3a13374d05630725d1d996f8083efadf7d2da999c9b4ca53ab7c98f`  
		Last Modified: Thu, 01 Jun 2023 23:19:06 GMT  
		Size: 28.6 MB (28648005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc2efbbc357d3180a9037577b3e9ef5404409073cff3477f88ad10630fec864`  
		Last Modified: Fri, 02 Jun 2023 14:46:59 GMT  
		Size: 1.5 MB (1476762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a8319cfb6e84fa1452a3d30c3a0857c034c1c3ceaab59767bd04191ccf0a13`  
		Last Modified: Tue, 06 Jun 2023 22:52:48 GMT  
		Size: 130.6 MB (130609729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488d0d7fc5ee4b0df940b92c193dedf98892a67c6b762d96c0a2bfb133bc7de5`  
		Last Modified: Fri, 09 Jun 2023 06:01:36 GMT  
		Size: 18.9 MB (18938986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8252a871dfd45862ab5427e436d80c8cbab1851cf128f3596620ac46c20618b1`  
		Last Modified: Fri, 09 Jun 2023 06:01:34 GMT  
		Size: 684.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c6588f21160edcaa1bf560aaf71edb6c8d9f61b7b590a47f493c4f9696816b`  
		Last Modified: Fri, 09 Jun 2023 06:01:34 GMT  
		Size: 10.5 KB (10537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be89a5dd2c560828f55c57ee38e1770a5449353d6c45d31cb87a41a7f2f1c18`  
		Last Modified: Fri, 09 Jun 2023 06:01:34 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0497787f8f9d2da86c2534b0945f120d4e6762a15015d15aaf36c06787a9a81`  
		Last Modified: Fri, 09 Jun 2023 06:01:34 GMT  
		Size: 11.5 KB (11529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a900e903a8b247f173172b45c99cda7214febe8de66609706ada744a30fe999`  
		Last Modified: Fri, 09 Jun 2023 06:01:35 GMT  
		Size: 6.2 MB (6200794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2561790ede254631abd78cc80d97bde961c6f8f90fd8e1d66a129ce14c0c9833`  
		Last Modified: Fri, 09 Jun 2023 06:02:06 GMT  
		Size: 359.2 MB (359248086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34e588e2b63e5f07c4ba6fa8f40c824b9b746ec0af21a5cd57458c476423531`  
		Last Modified: Fri, 09 Jun 2023 06:01:51 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb937e754324fcabf01e8968474a2e37e67319a6130058c1cfe70aa87cb0fb3`  
		Last Modified: Fri, 09 Jun 2023 06:01:53 GMT  
		Size: 15.6 MB (15649149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
