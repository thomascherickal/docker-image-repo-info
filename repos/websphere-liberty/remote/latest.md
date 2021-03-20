## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:c541ba03441fd94d5de2a777c94996533b43290294226a3df023ab9a9cd8725c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:cfb49579a8e5f3b8445da872504d48cdc99db4572d557b7c26e85bac963bc069
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.3 MB (414258908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72166d3997241134bec436266fb8e72785a5fe70499c73b695732fe6de5028fa`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Thu, 11 Mar 2021 20:19:55 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 11 Mar 2021 20:20:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Mar 2021 20:20:18 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Thu, 11 Mar 2021 20:20:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 11 Mar 2021 20:20:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 11 Mar 2021 20:42:27 GMT
ARG VERBOSE=false
# Thu, 11 Mar 2021 20:42:27 GMT
ARG OPENJ9_SCC=true
# Sat, 20 Mar 2021 02:18:40 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Sat, 20 Mar 2021 02:18:40 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Sat, 20 Mar 2021 02:18:40 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Sat, 20 Mar 2021 02:18:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 20 Mar 2021 02:18:41 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Sat, 20 Mar 2021 02:18:41 GMT
ARG LIBERTY_URL
# Sat, 20 Mar 2021 02:18:41 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 20 Mar 2021 02:18:56 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 20 Mar 2021 02:18:56 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 20 Mar 2021 02:18:56 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Sat, 20 Mar 2021 02:18:57 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 20 Mar 2021 02:18:58 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 20 Mar 2021 02:18:58 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Sat, 20 Mar 2021 02:18:59 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 20 Mar 2021 02:19:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 20 Mar 2021 02:19:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 20 Mar 2021 02:19:10 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 20 Mar 2021 02:19:10 GMT
USER 1001
# Sat, 20 Mar 2021 02:19:10 GMT
EXPOSE 9080 9443
# Sat, 20 Mar 2021 02:19:10 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 20 Mar 2021 02:19:10 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 20 Mar 2021 02:19:41 GMT
ARG VERBOSE=false
# Sat, 20 Mar 2021 02:19:41 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 20 Mar 2021 02:22:23 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 20 Mar 2021 02:22:24 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 20 Mar 2021 02:23:00 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1ee32594389ea9f21979e9e4266c142c3379e6431fd40105ea37334fc9cb4d`  
		Last Modified: Thu, 11 Mar 2021 20:24:53 GMT  
		Size: 3.0 MB (2959314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304e3a3f32eb36308fe702533564d3de56222f8c13e89abfbe2f7e57ca85d144`  
		Last Modified: Thu, 11 Mar 2021 20:25:03 GMT  
		Size: 130.8 MB (130805806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f852182c7a020ef0039633e779be9572c089b2f6a3e9b28c634b46cbb2e0887`  
		Last Modified: Sat, 20 Mar 2021 02:27:15 GMT  
		Size: 14.0 MB (13989599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab787d43e9f0e4f526bb8c0a47f2b1030761ad42d1405b3b570447722dbe9db`  
		Last Modified: Sat, 20 Mar 2021 02:27:11 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a650e5016dc7f3e349b9e759af1a95527bcef6a4044ff8fdf73ba51856662032`  
		Last Modified: Sat, 20 Mar 2021 02:27:11 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c287d6adb0dd12fb8ae199bebeaf9003fd360b3d5d6f3444569691b035d71bbb`  
		Last Modified: Sat, 20 Mar 2021 02:27:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953614991855b84ee6eb99f8b771f2799713f123debacb68ba83445f99ab3d0`  
		Last Modified: Sat, 20 Mar 2021 02:27:11 GMT  
		Size: 10.5 KB (10537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d830f4ccfde55323ccb746993b8c92ad61638696d034365e11fab764980f375`  
		Last Modified: Sat, 20 Mar 2021 02:27:12 GMT  
		Size: 5.6 MB (5629901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eaf351438fe60ac6f409dd1e129550a8176fe36ef20e8dfc90df5cb92a3036`  
		Last Modified: Sat, 20 Mar 2021 02:27:50 GMT  
		Size: 212.8 MB (212786126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3308ba450c6579dd66e191e1ab8a5de69e63f7d2e1039b1bd6489d07f0cda0b`  
		Last Modified: Sat, 20 Mar 2021 02:27:37 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfd60855ebd948d2a5ddf39746deb07ce9750054376bfdef513c79952f25f30`  
		Last Modified: Sat, 20 Mar 2021 02:27:41 GMT  
		Size: 21.4 MB (21355000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; 386

```console
$ docker pull websphere-liberty@sha256:c847143995aec30ca5d4526544d7c41ca7a42a8baf8195848864d0128e96ecf3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.2 MB (349209019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d2c9374be56a63d6e35820fec8676f2d4ed2b9bdaf09a49c8545b039479bb7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 20 Mar 2020 18:38:55 GMT
ADD file:d859d389e38b7ac70fd56f97e38d52a77b58e72b96237a4302d1984cdd912a55 in / 
# Fri, 20 Mar 2020 18:38:56 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 20 Mar 2020 18:38:57 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 20 Mar 2020 18:38:58 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 20 Mar 2020 18:38:58 GMT
CMD ["/bin/bash"]
# Fri, 20 Mar 2020 19:06:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 20 Mar 2020 19:06:41 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:06:42 GMT
ENV JAVA_VERSION=1.8.0_sr6fp6
# Fri, 20 Mar 2020 19:07:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='87f9d45b7e1fa65ec018479f3ca7da69a03b52b0da10b8d1555142eec8ab0093';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='b5f825047c9bb5d360fb83694f12e17b1a5a15abf94ac82cd0a3aea32c9a361c';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f3c04cd07ef269c24373840eae6f59c7db7a16d2e206d393ba93efa6dbb8d74f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='2bbefda96f7d1a5f1694893961e92ccc59dfa50375ae5450675d7a4213d5812e';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='d5b0508d53d1c7382c06f5bc1daf3d57c19c70d851e86e6b1162bcd93f616f7e';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 20 Mar 2020 19:07:26 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:31:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433
# Fri, 20 Mar 2020 19:31:53 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 20 Mar 2020 19:31:53 GMT
ARG LIBERTY_URL
# Fri, 20 Mar 2020 19:31:53 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 20 Mar 2020 19:32:02 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 19:32:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Mar 2020 19:32:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 20 Mar 2020 19:32:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 20 Mar 2020 19:32:04 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 20 Mar 2020 19:32:04 GMT
COPY dir:0d0cedab2fbb7208b9d81afa78e9f15b12b71232224a2fe9753c00b7b72bd72e in /opt/ibm/helpers/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 20 Mar 2020 19:32:05 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 20 Mar 2020 19:32:06 GMT
# ARGS: DOWNLOAD_OPTIONS=
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 20 Mar 2020 19:32:06 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 20 Mar 2020 19:32:06 GMT
USER 1001
# Fri, 20 Mar 2020 19:32:06 GMT
EXPOSE 9080 9443
# Fri, 20 Mar 2020 19:32:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 20 Mar 2020 19:32:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 20 Mar 2020 19:32:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 20 Mar 2020 19:35:01 GMT
# ARGS: REPOSITORIES_PROPERTIES=
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 20 Mar 2020 19:35:01 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
```

-	Layers:
	-	`sha256:765ce743592771b94ad8ff27e281e66c13f6039962c7dde4dbe47123081e015b`  
		Last Modified: Mon, 16 Mar 2020 15:38:41 GMT  
		Size: 27.1 MB (27122453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dc9c4739090a3d2f7265f1f8184b1cbd8ae133b863f8aa93ec5cf1761ee7a5`  
		Last Modified: Fri, 20 Mar 2020 18:39:35 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a5b698281c077f48fc598e698f0619e4d00a2fedc1832fc95e9cf281408f63`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaebe599891b1e1befc10d752a117cc5615ec2dd3913d399fd66e26e0cace3e5`  
		Last Modified: Fri, 20 Mar 2020 18:39:34 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f829150bc8a53a37ac17eb34838fa33c990881a4031bc650a9dae26b3f7880e`  
		Last Modified: Fri, 20 Mar 2020 19:09:23 GMT  
		Size: 3.0 MB (2992132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17b9ccc4baf3a1ffa517a03c7c3d01900136b128b36a83558c67c42e6c1cbaa`  
		Last Modified: Fri, 20 Mar 2020 19:09:35 GMT  
		Size: 118.8 MB (118756706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5011972f1876d464fb62206211a5b5e162ba2603bf20fc4cd0f2b4ffd311cd9`  
		Last Modified: Fri, 20 Mar 2020 19:39:16 GMT  
		Size: 13.6 MB (13600436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5395b713d5baa0917182ca82077b6fa2a0c51789907f96cbb12455586d9fa9b`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 672.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389324a3d9489b2fbcd5946f9d24285c0171c3218470e4a5e2d45c731cefc522`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 3.5 KB (3515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38ea596499e1f23ce426826250984869e92da50aec5845a6233a76d7764bfd1`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea3197b55235384f836e31a605c460f6cb7196f68dc29c65640738d8aa50188`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f76bf565cdb9e59c325f24357eb6b164555ed8629a4b8383448239608966d`  
		Last Modified: Fri, 20 Mar 2020 19:39:13 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd2560c76831311d13d197b4784e0826f6ffae62e3b9a22d2fa5675b9b71a2`  
		Last Modified: Fri, 20 Mar 2020 19:39:42 GMT  
		Size: 186.6 MB (186634496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891aa2b3e904f8f514677372187983ac12c98c209c433ab5bf0862e09d6f4ef`  
		Last Modified: Fri, 20 Mar 2020 19:39:20 GMT  
		Size: 943.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:7e6964ab270c0f0892652e9a8d9221faa5f961b2e459effa0e3ce584c6fac59b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.6 MB (414591212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28b6bbcecd856e130addeffbae41c88e7c365b103cb7f53bb9180189fb39a56`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 04 Mar 2021 02:56:30 GMT
ADD file:4a2d847969faa9da1f1336ff0c2871a418cb7f7668abecb0d6914821ce7acd02 in / 
# Thu, 04 Mar 2021 02:56:48 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:57:06 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:57:19 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:57:22 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 06:05:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 04 Mar 2021 06:06:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Mar 2021 21:37:28 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Thu, 11 Mar 2021 21:38:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 11 Mar 2021 21:39:01 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 11 Mar 2021 23:30:51 GMT
ARG VERBOSE=false
# Thu, 11 Mar 2021 23:30:57 GMT
ARG OPENJ9_SCC=true
# Sat, 20 Mar 2021 03:45:07 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Sat, 20 Mar 2021 03:45:15 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Sat, 20 Mar 2021 03:45:22 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Sat, 20 Mar 2021 03:45:33 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 20 Mar 2021 03:45:39 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Sat, 20 Mar 2021 03:45:46 GMT
ARG LIBERTY_URL
# Sat, 20 Mar 2021 03:45:52 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 20 Mar 2021 03:47:00 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 20 Mar 2021 03:47:07 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 20 Mar 2021 03:47:15 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Sat, 20 Mar 2021 03:47:20 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 20 Mar 2021 03:47:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 20 Mar 2021 03:47:55 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Sat, 20 Mar 2021 03:48:03 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 20 Mar 2021 03:48:33 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 20 Mar 2021 03:49:07 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 20 Mar 2021 03:49:15 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 20 Mar 2021 03:49:20 GMT
USER 1001
# Sat, 20 Mar 2021 03:49:29 GMT
EXPOSE 9080 9443
# Sat, 20 Mar 2021 03:49:34 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 20 Mar 2021 03:49:40 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 20 Mar 2021 03:54:03 GMT
ARG VERBOSE=false
# Sat, 20 Mar 2021 03:54:08 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 20 Mar 2021 03:58:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 20 Mar 2021 03:58:27 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 20 Mar 2021 03:59:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:367a668e4ea4eecc7411f59b0e710bd8e6f0910afffbc5cf7cc56a9b91cf2097`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 30.4 MB (30421101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d1a50fb15144b9c99d82c9511112522bcbc25c056716cb225e51c2998a3c4c5`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d4006473f93104f15e85c85416b0e4a37cb8c0f58552fc6f9260fe2c58140`  
		Last Modified: Thu, 04 Mar 2021 03:01:48 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59980a4d9c242412ef5a5dfbafd355a75407f666e0da0f08f867f5bba04d0a5f`  
		Last Modified: Thu, 04 Mar 2021 06:12:04 GMT  
		Size: 3.1 MB (3082310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdeb0c471815a83698c6c82fad9ea9e73a11cd6bd734cfe97cf4744d32bbf05`  
		Last Modified: Thu, 11 Mar 2021 21:42:27 GMT  
		Size: 130.4 MB (130406667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a143e82b6c608ddb6344af23d6be218a524b7e0c4d377a6efe1dec0638859eb5`  
		Last Modified: Sat, 20 Mar 2021 04:06:01 GMT  
		Size: 14.0 MB (13989165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5d954d198098ee29756b397e5af9d80e592527095c9316489b814382fb6db5`  
		Last Modified: Sat, 20 Mar 2021 04:05:54 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9be6cc8d0babed969aa1273536b80e189ae255c05293dc1720ec7c4fc1e208`  
		Last Modified: Sat, 20 Mar 2021 04:05:54 GMT  
		Size: 9.6 KB (9558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23552253929c01baf12a31ab6357ee2cdd418b33dd24f6f6a646f83de5042741`  
		Last Modified: Sat, 20 Mar 2021 04:05:54 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc8d4d769e1196c0e7cf2785ea418f318643b3be984405360d34576cf86834f`  
		Last Modified: Sat, 20 Mar 2021 04:05:54 GMT  
		Size: 10.6 KB (10553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3253631158270af6f2cf47e63958d1a500a0846970b1372c6e78c827b556236d`  
		Last Modified: Sat, 20 Mar 2021 04:05:55 GMT  
		Size: 5.3 MB (5254155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210caa65f9d08fbdde8002c13e3d1fcbc7bed1a8fbdf87bfbf5bbebdd3ca0db3`  
		Last Modified: Sat, 20 Mar 2021 04:06:47 GMT  
		Size: 212.4 MB (212414430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef73c2cb727fdc43d287282aa4d87bf07b82cd81d589c2d1af03e1eaccd148`  
		Last Modified: Sat, 20 Mar 2021 04:06:25 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74568cd32b76c9fab5c16a19dfd235cf62fb3f59ecd7958e697596a2b25a3d5f`  
		Last Modified: Sat, 20 Mar 2021 04:06:29 GMT  
		Size: 19.0 MB (19000294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:42f8011da1a97b71d9b75c505ab55014a4c578691bc14abf4c98b898579f2a20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **410.3 MB (410257385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9963dc5e92a125fe788da45a7d12f9555d12b5db88fd0d7ac2f784e4a9adef7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:37:36 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 04 Mar 2021 03:37:42 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Mar 2021 19:41:29 GMT
ENV JAVA_VERSION=1.8.0_sr6fp26
# Thu, 11 Mar 2021 19:42:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='efa4b1b4f163133043eb99d1b276311201fc37bb60bfde051fd06c78cada038b';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='1f16f54b16bb978772c5ace5769a05233ba4a58de0e23d0542b0c0e55f95dd63';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='40b61a9bd4727d5dc1573ab69b1f973ffa14bf18f396a244f7263f7782173c98';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='4f52f3044658a232f2d8e77a275d1e95a6de90a6bf1e63a3ea6d7a87fa576d87';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='024b7c4691233016fff56bc9656e4979b283abbbe5751ddd98917944eaabdb10';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 11 Mar 2021 19:42:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 11 Mar 2021 20:04:10 GMT
ARG VERBOSE=false
# Thu, 11 Mar 2021 20:04:10 GMT
ARG OPENJ9_SCC=true
# Sat, 20 Mar 2021 02:11:25 GMT
ARG EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f
# Sat, 20 Mar 2021 02:11:25 GMT
ARG NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8
# Sat, 20 Mar 2021 02:11:25 GMT
ARG NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075
# Sat, 20 Mar 2021 02:11:25 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=21.0.0.3 org.opencontainers.image.revision=cl210320210309-1101 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 20 Mar 2021 02:11:25 GMT
ENV LIBERTY_VERSION=21.0.0_03
# Sat, 20 Mar 2021 02:11:26 GMT
ARG LIBERTY_URL
# Sat, 20 Mar 2021 02:11:26 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 20 Mar 2021 02:11:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 20 Mar 2021 02:11:38 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 20 Mar 2021 02:11:38 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=21.0.0.3 BuildLabel=cl210320210309-1101
# Sat, 20 Mar 2021 02:11:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 20 Mar 2021 02:11:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 20 Mar 2021 02:11:40 GMT
COPY dir:97a8e76f74c504c9fb35f9416fa56b7ba9d48a4796f6cdac0d566ee62c1fb2fb in /opt/ibm/helpers/ 
# Sat, 20 Mar 2021 02:11:40 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 20 Mar 2021 02:11:41 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 20 Mar 2021 02:11:49 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=1ada8dde94633b139876c01b15c2f47011108bbd38e9d498abe73c7f3682b22f NON_IBM_SHA=a495097ac17101fa55a3b763225b4b814c7d2b3019e55922e095f31351790ed8 NOTICES_SHA=c50d7a288214bf29b9e1f01d10f9f43dce85c73829cc2030a7f398ff9bc0b075 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 20 Mar 2021 02:11:50 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 20 Mar 2021 02:11:50 GMT
USER 1001
# Sat, 20 Mar 2021 02:11:50 GMT
EXPOSE 9080 9443
# Sat, 20 Mar 2021 02:11:50 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 20 Mar 2021 02:11:50 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 20 Mar 2021 02:12:21 GMT
ARG VERBOSE=false
# Sat, 20 Mar 2021 02:12:22 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 20 Mar 2021 02:16:21 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 20 Mar 2021 02:16:26 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 20 Mar 2021 02:16:54 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf803b1a83be792f5b796dfcdfedd1b88a42baee549d3b2aa6279db97d1fa4f2`  
		Last Modified: Thu, 04 Mar 2021 03:41:35 GMT  
		Size: 2.7 MB (2676230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8f2b4238c59099c81bd84242b8f6d8003a8da86d12743cb85e394f08662ec5`  
		Last Modified: Thu, 11 Mar 2021 19:45:09 GMT  
		Size: 128.1 MB (128065747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725131fcc9058947fd55cd11db23c981e68d246dd3c14f817bf0aaa966054fb1`  
		Last Modified: Sat, 20 Mar 2021 02:23:03 GMT  
		Size: 14.0 MB (13988356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ebc4ab7d18112d267ca79012c5645a861aae08bc3cef4fe8e641ad507ceab`  
		Last Modified: Sat, 20 Mar 2021 02:23:01 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39196d46dabb72cb7b7bbc1c5d945285324d6b24913e3a35dcbb0e81bb009e25`  
		Last Modified: Sat, 20 Mar 2021 02:23:01 GMT  
		Size: 9.6 KB (9556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b95e9ab95f9ac8b2160df619884f773bac59dfd2de6ff925c5ee069d368e58`  
		Last Modified: Sat, 20 Mar 2021 02:23:01 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2207b5f344eea7979fbf80bd314a965745aa4a14d287622b1d6e14b39e412bce`  
		Last Modified: Sat, 20 Mar 2021 02:23:01 GMT  
		Size: 10.5 KB (10535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2213ca1dc499a812c8bd0b1d71329e283f17164ef6ed28399fbca4fdbf851c92`  
		Last Modified: Sat, 20 Mar 2021 02:23:01 GMT  
		Size: 5.9 MB (5870556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b25fe07dfaadbe35ed2fdcc89f67f0d1318e3149df7c660276e62b28d067d9`  
		Last Modified: Sat, 20 Mar 2021 02:23:28 GMT  
		Size: 213.0 MB (213027819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2649c24518b6bbfadeb8beec52e63619116173cf10b6a0c7eb31d0b396ae58a`  
		Last Modified: Sat, 20 Mar 2021 02:23:15 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6dafc2fa06d6a5b0dae25abe57040416e0091067a2387377a2216e2164d906`  
		Last Modified: Sat, 20 Mar 2021 02:23:18 GMT  
		Size: 21.2 MB (21224835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
