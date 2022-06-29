## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:6ec97f5e50290c5295f5e99686b971a66d31742b6e49e70f5e5d4a0d6dcc7ec5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:00f78cd6f8d89d1c19cbbb92c7765f1065fd6afa8a6239b8f0f107a99e771aa0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **462.4 MB (462375580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9edbcd8cb10189c8fc1871fb635cf10b8ddcaa4a67fc259d68e7ec1cefc8401`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:52:33 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 02:52:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:19:40 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:20:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:20:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 18:46:44 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 18:46:44 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 18:46:44 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 18:46:44 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 18:46:44 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 18:46:44 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 18:46:45 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 18:46:45 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 18:46:45 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 18:47:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:47:00 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 18:47:00 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 18:47:00 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 18:47:01 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 18:47:01 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 18:47:02 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 18:47:02 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 18:47:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 18:47:11 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 18:47:11 GMT
USER 1001
# Wed, 29 Jun 2022 18:47:11 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 18:47:11 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 18:47:11 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 18:47:21 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 18:47:21 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 18:56:45 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 18:56:45 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 18:57:15 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc337ae35500f1356b4927d94eff4c5c2013592d9465313f05b0e829b69baf`  
		Last Modified: Tue, 07 Jun 2022 02:54:56 GMT  
		Size: 3.0 MB (2960220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b86a8569f165a4bde6ae9037437d65134d1609022f0eb5276abaa3606005f37`  
		Last Modified: Wed, 29 Jun 2022 18:23:31 GMT  
		Size: 129.1 MB (129092292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221fc979a5bb2e9f301839f86771026088560f2317fb4ad818f697772218c528`  
		Last Modified: Wed, 29 Jun 2022 19:08:53 GMT  
		Size: 14.4 MB (14394423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3272c57680288a2aed15f9c13f81a640d0afe4c07558878eeefa79f4a0947951`  
		Last Modified: Wed, 29 Jun 2022 19:08:49 GMT  
		Size: 680.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b2d95d73b6086211daad021b7282cc53b7d7149d8935c86c1aac1ff0408105`  
		Last Modified: Wed, 29 Jun 2022 19:08:49 GMT  
		Size: 9.8 KB (9754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbcbd4bf6439f94ebe818e09f3ed1b521d86ec1cc997ee39da973adf5d45ca5`  
		Last Modified: Wed, 29 Jun 2022 19:08:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006bf1ec74834c0986a945ed67e689bf1e86b765230ae7ebe517c7b44c5599bd`  
		Last Modified: Wed, 29 Jun 2022 19:08:48 GMT  
		Size: 10.7 KB (10742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c4a87240145b6d38d28daf5fd4644fe9e9376b67b96fd9c6ccb9c6ad6d2630`  
		Last Modified: Wed, 29 Jun 2022 19:08:49 GMT  
		Size: 5.7 MB (5738466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6543599ea7a49fd3c891c670eec9727a433ed5a0f01eed7e97b604647e070a`  
		Last Modified: Wed, 29 Jun 2022 19:09:15 GMT  
		Size: 267.1 MB (267145934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c3cbf39c511ec2dbfbdeaf5845cd5530f5171ed670a1f0d23176e9f53caf47`  
		Last Modified: Wed, 29 Jun 2022 19:09:01 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bdd98af8ee3e491ce2552b3ddc76ee225d0bf73e6fe45ac28d67fbe7788585`  
		Last Modified: Wed, 29 Jun 2022 19:09:03 GMT  
		Size: 16.3 MB (16310225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:20b8c8568ac1ace5302e32de4580705070ad867b1267fc10eddecc0342efb233
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.1 MB (463103256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24bec26d5b6e33bfa1465f31c5486fb46d341b64a8a89ebecee746a78fd2086b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:49:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 08:50:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:31:53 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:33:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:33:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:03:57 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:04:05 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:04:16 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:04:32 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:04:39 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:04:46 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:04:53 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:04:57 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:05:02 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:06:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:06:54 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:06:59 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:22 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:27 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:08:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:08:16 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:08:20 GMT
USER 1001
# Wed, 29 Jun 2022 19:08:28 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:08:35 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:08:44 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 19:09:19 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:09:27 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 19:18:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 19:18:47 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 19:19:57 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4a22aedc3b9f2593635b0a3f6fe64e6dd424850b9782f66e88c8c162926d6a`  
		Last Modified: Tue, 07 Jun 2022 08:54:16 GMT  
		Size: 3.1 MB (3082521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448aed354e59dc01b7da997655c86778001067ef107a5c1fb36a7c38fcf5fdda`  
		Last Modified: Wed, 29 Jun 2022 18:38:02 GMT  
		Size: 128.6 MB (128629743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ee64dfa956bec7a3911c4fbcec85677da5eb3557fdd1fad0cd05371b418ed3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 14.4 MB (14414087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f44198605bccf1a3fd327e2929165c362826698ef117c8ed5e5f61cf8471cce`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 685.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008efd74eeabae4093e325cb3ee9f17c49e27f7dbb19564636c92acb9051471`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 9.8 KB (9757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8e4e4d330f9771962db9ea9c4da8f370e92f1745f117e9db5baae643dfff3`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa888647a678f768a7a68d44ee29bc98b5834e1d4b43481f1d79fb22ae798d8`  
		Last Modified: Wed, 29 Jun 2022 19:36:14 GMT  
		Size: 10.7 KB (10748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24233765490b95aea52162ad51e9982a4c6bd67895d93467ca629ea8bfb5a68`  
		Last Modified: Wed, 29 Jun 2022 19:36:15 GMT  
		Size: 5.3 MB (5337804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a597fe1c695442d024092e9ba428ea88ffa886c912a199fbe492b776a53a7595`  
		Last Modified: Wed, 29 Jun 2022 19:36:52 GMT  
		Size: 267.1 MB (267144840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165a7c33a3339f487205b064950b8fb81222d47d74c6fdfef158d7464150dbbb`  
		Last Modified: Wed, 29 Jun 2022 19:36:29 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ede9c741b2ef54fc67a38aab455cdc0ef8bea790cfdf300b7e1d01aa4486ec`  
		Last Modified: Wed, 29 Jun 2022 19:36:35 GMT  
		Size: 14.0 MB (14028991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:29cfaefd6f6668d8f1ede678091d161629c5105a07999d5bc90dd4a08d5bcc7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.8 MB (457825061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c51a43207569fdcb0a847a5979cd7d2e021fade8db5ad67e7823e741436c7269`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Tue, 07 Jun 2022 04:04:44 GMT
ADD file:e2caa30d22701eeadebe1abd66923745f75d170d7baa51a62119576c31b7f89c in / 
# Tue, 07 Jun 2022 04:04:47 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:27:04 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 07 Jun 2022 06:27:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 18:41:46 GMT
ENV JAVA_VERSION=8.0.7.11
# Wed, 29 Jun 2022 18:42:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='6feb6681dfa18f98f4a9ad4eedfd1c9129d82221c0e244adbc0e23664dc22bcf';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='0b66a9069eb31f478a43e59ade2924694cff48320f921cd890df935ca55388ad';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='7fa23fe025fc41f0ea074628125d314a816f563452ab29e8adb7f8074729a70d';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='01dcdafbd8646768c226f76eb5dd57598de04b9ab6c95d35d5f9306fb27acb2a';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='5f4dd3046ee81f968dd3cf448e2977408c2128910417ad057f71baa52564b255';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 29 Jun 2022 18:42:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:07:18 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:07:19 GMT
ARG OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:19 GMT
ARG EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf
# Wed, 29 Jun 2022 19:07:20 GMT
ARG NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1
# Wed, 29 Jun 2022 19:07:20 GMT
ARG NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09
# Wed, 29 Jun 2022 19:07:21 GMT
LABEL org.opencontainers.image.authors=Leo Christy Jesuraj, Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=22.0.0.6 org.opencontainers.image.revision=cl220620220523-1607 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Wed, 29 Jun 2022 19:07:22 GMT
ENV LIBERTY_VERSION=22.0.0_06
# Wed, 29 Jun 2022 19:07:22 GMT
ARG LIBERTY_URL
# Wed, 29 Jun 2022 19:07:23 GMT
ARG DOWNLOAD_OPTIONS=
# Wed, 29 Jun 2022 19:07:39 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Wed, 29 Jun 2022 19:07:40 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Jun 2022 19:07:41 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=22.0.0.6 BuildLabel=cl220620220523-1607
# Wed, 29 Jun 2022 19:07:41 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Wed, 29 Jun 2022 19:07:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Wed, 29 Jun 2022 19:07:44 GMT
COPY dir:8bf844c49178cf63745af9ec643f57d70bd92c28166fabfad188dfc250d88353 in /opt/ibm/helpers/ 
# Wed, 29 Jun 2022 19:07:44 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Wed, 29 Jun 2022 19:07:46 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Wed, 29 Jun 2022 19:07:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=6d76dc1906ca448927abb8238487de96089a1b1591286c7339cba94976261abf NON_IBM_SHA=412ee94517773939d86d1ac9aa013c8bdff481de4d8ef58c84c997b4d612fef1 NOTICES_SHA=ca3ea01852554c9f84c907754677a18b6d9e39707469f7af93808fd1c1d42a09 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Wed, 29 Jun 2022 19:07:57 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,readonly,nonfatal,cacheDir=/output/.classCache/ -Dosgi.checkConfiguration=false -XX:+UseContainerSupport
# Wed, 29 Jun 2022 19:07:57 GMT
USER 1001
# Wed, 29 Jun 2022 19:07:58 GMT
EXPOSE 9080 9443
# Wed, 29 Jun 2022 19:07:58 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Wed, 29 Jun 2022 19:07:58 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Wed, 29 Jun 2022 19:08:19 GMT
ARG VERBOSE=false
# Wed, 29 Jun 2022 19:08:19 GMT
ARG REPOSITORIES_PROPERTIES=
# Wed, 29 Jun 2022 19:16:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Wed, 29 Jun 2022 19:16:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Wed, 29 Jun 2022 19:17:30 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -path "*.classCache*" ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:048a87c6fcb9ea8de843bbbe647d14716098af0741f7f59e30c60f39b96b4397`  
		Last Modified: Tue, 07 Jun 2022 04:07:30 GMT  
		Size: 25.4 MB (25370236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c178b02e888a022df784ee042a75ea8e48f1db295aec033725e7e6edc51cc1ca`  
		Last Modified: Tue, 07 Jun 2022 06:31:44 GMT  
		Size: 2.7 MB (2677363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec29645333a3d4f83d94dc17629a536bcc634567aa450d92ef4f53e9db47e2`  
		Last Modified: Wed, 29 Jun 2022 18:46:46 GMT  
		Size: 126.1 MB (126144122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b240ddfe692cd72e771eadc1881cb6f8756d8d32ee04fecade4acbb05b2f2c6b`  
		Last Modified: Wed, 29 Jun 2022 19:35:58 GMT  
		Size: 14.4 MB (14398484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d6e9e5f5717235e2e9ebf81aaf65f6d958a9ff7f0a5b1fbd5a0142f9a41624`  
		Last Modified: Wed, 29 Jun 2022 19:35:56 GMT  
		Size: 691.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043c4e5d54c8cd07131dc3d7d69767310b9888439360657a8d83d9da3421197`  
		Last Modified: Wed, 29 Jun 2022 19:35:56 GMT  
		Size: 9.8 KB (9758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b0be08e9b1658b8a1c86ff8070c1dd905f70b5982f36749e53438b0b9ee556`  
		Last Modified: Wed, 29 Jun 2022 19:35:56 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1838c85e3280c2c945a5fea0ae94a8b8ff30f92198b832b460001cfb6f038dbe`  
		Last Modified: Wed, 29 Jun 2022 19:35:56 GMT  
		Size: 10.8 KB (10753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec76384cf6cfd0dfa1bb2e33c8799ccb8d8cc1e54482302780d4961cb825b59`  
		Last Modified: Wed, 29 Jun 2022 19:35:57 GMT  
		Size: 6.0 MB (5972801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047f8d7ab9e6c9e56d38f2b372d6d86016d94a1eb6cd140fdbbe68a02bdb9fc3`  
		Last Modified: Wed, 29 Jun 2022 19:36:18 GMT  
		Size: 267.1 MB (267144991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9db18035026fe8361071f9230cb2ccc3c171afac1591bd812488498d3e6f9d9`  
		Last Modified: Wed, 29 Jun 2022 19:36:06 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6111e615ed5e274b282fd2099c5a0ecaa948d92ab4cabed9ad779aea793ff37f`  
		Last Modified: Wed, 29 Jun 2022 19:36:08 GMT  
		Size: 16.1 MB (16094642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
