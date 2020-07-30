<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `websphere-liberty`

-	[`websphere-liberty:20.0.0.3-full-java8-ibmjava`](#websphere-liberty20003-full-java8-ibmjava)
-	[`websphere-liberty:20.0.0.3-kernel-java8-ibmjava`](#websphere-liberty20003-kernel-java8-ibmjava)
-	[`websphere-liberty:20.0.0.6-full-java8-ibmjava`](#websphere-liberty20006-full-java8-ibmjava)
-	[`websphere-liberty:20.0.0.6-kernel-java8-ibmjava`](#websphere-liberty20006-kernel-java8-ibmjava)
-	[`websphere-liberty:20.0.0.8-full-java8-ibmjava`](#websphere-liberty20008-full-java8-ibmjava)
-	[`websphere-liberty:20.0.0.8-kernel-java8-ibmjava`](#websphere-liberty20008-kernel-java8-ibmjava)
-	[`websphere-liberty:beta`](#websphere-libertybeta)
-	[`websphere-liberty:full`](#websphere-libertyfull)
-	[`websphere-liberty:kernel`](#websphere-libertykernel)
-	[`websphere-liberty:latest`](#websphere-libertylatest)

## `websphere-liberty:20.0.0.3-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:3ef4e5496b3b44d00c4c20ca403122525c49b0d9070d194fe9fc0fe68feb1a96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.3-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:713d3c6dd01df3666aca6fe356eb5f51ae6d039283ee07b400cc9aa6f44b6b10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.2 MB (393230678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:196dfd432ce227368d5783c487460a3aaceb658855c58a7a0e4e3cb2a6d5ca7e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:18:43 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 20:18:43 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 24 Jul 2020 20:18:43 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 20:18:43 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 20:18:52 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 20:18:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 20:18:52 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 24 Jul 2020 20:18:53 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:18:54 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 20:18:54 GMT
COPY dir:9bf54ffdc4f4c7668f2f626dc636555b60354b8e5fb3510b77868c9d2b4b15cd in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 20:18:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 20:18:54 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 24 Jul 2020 20:18:55 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 20:19:07 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 20:19:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:19:07 GMT
USER 1001
# Fri, 24 Jul 2020 20:19:07 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 20:19:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 20:19:08 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 20:19:12 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:19:12 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 24 Jul 2020 20:23:34 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 24 Jul 2020 20:23:34 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 24 Jul 2020 20:24:48 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec3875d1981f8340320077504c6a6c93667702173fe043e0489ddd717300bd`  
		Last Modified: Fri, 24 Jul 2020 20:26:11 GMT  
		Size: 13.6 MB (13600360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be31ae85d236398b806e01b917763a6a2e93865c9379874c6a1dc0f0253afb7`  
		Last Modified: Fri, 24 Jul 2020 20:26:09 GMT  
		Size: 676.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0619b60bfbff10c8c4469472a116096723d0974f2d20e39e36a0a1d7491ed3`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 5.6 KB (5623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316afa43b4edf142d60e74140d6094b43144a14393c090203f818e12a08a5f7d`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955621de6b3af6e0596e0ff9ceb59cb968e6079d19a250291ef178f041cf75ac`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 57.4 KB (57421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25992359574a6609f17e53fce3486e5dcf2412387208220b0b2297aeb1b1d821`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 6.5 KB (6486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3188389b530abb3afd44b72899c849f3e6da3e825e7b544bb315076f2527cdc5`  
		Last Modified: Fri, 24 Jul 2020 20:26:09 GMT  
		Size: 5.6 MB (5583146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008fd4c702210819761f44b65dc0a2e1beb6c5ab7376a3da7a726bf025412568`  
		Last Modified: Fri, 24 Jul 2020 20:26:29 GMT  
		Size: 192.2 MB (192179061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f106806aa7ee63bf6849159843ecd9bb12d2884213549353dce34292de0e94f4`  
		Last Modified: Fri, 24 Jul 2020 20:26:14 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42cd3b01fb7531f4c67c43ee3e2b1be5c80df4d23d023cb742adb18ea9a2f36`  
		Last Modified: Fri, 24 Jul 2020 20:26:18 GMT  
		Size: 21.8 MB (21764078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.3-full-java8-ibmjava` - linux; 386

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

### `websphere-liberty:20.0.0.3-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:a340a7877f3540ffa4a22684431149b2d4965fa352ccf1d3a6985d75b2294260
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **401.1 MB (401117859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44357da96b205d9fa5a661d1581cec23ae88532a6ddee0d03dbb76b5e181d8b`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Sat, 25 Jul 2020 00:06:23 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 25 Jul 2020 00:06:28 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Sat, 25 Jul 2020 00:06:34 GMT
ARG LIBERTY_URL
# Sat, 25 Jul 2020 00:06:38 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 25 Jul 2020 00:07:24 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 25 Jul 2020 00:07:30 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Jul 2020 00:07:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Sat, 25 Jul 2020 00:07:39 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 25 Jul 2020 00:07:51 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 25 Jul 2020 00:07:53 GMT
COPY dir:9bf54ffdc4f4c7668f2f626dc636555b60354b8e5fb3510b77868c9d2b4b15cd in /opt/ibm/helpers/ 
# Sat, 25 Jul 2020 00:07:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 25 Jul 2020 00:07:56 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Sat, 25 Jul 2020 00:08:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 25 Jul 2020 00:08:26 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 25 Jul 2020 00:08:28 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 25 Jul 2020 00:08:32 GMT
USER 1001
# Sat, 25 Jul 2020 00:08:36 GMT
EXPOSE 9080 9443
# Sat, 25 Jul 2020 00:08:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 25 Jul 2020 00:08:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Sat, 25 Jul 2020 00:09:04 GMT
ARG VERBOSE=false
# Sat, 25 Jul 2020 00:09:08 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 25 Jul 2020 00:15:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 25 Jul 2020 00:15:42 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 25 Jul 2020 00:16:43 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68390033a4e2962c71f3ced7baad21f26acb7b8dbcae568d847ad3b404758b7`  
		Last Modified: Sat, 25 Jul 2020 00:19:44 GMT  
		Size: 13.6 MB (13600991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcf7d7a32e4f97a61e40c30604f55f21db767b36011a2bdc147a59d0dbdfe77`  
		Last Modified: Sat, 25 Jul 2020 00:19:42 GMT  
		Size: 719.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a114806261868a1d971b16c9fe852267af5bf7faf42a1680b6319366681410d4`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 5.7 KB (5651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751ea1f4cd43f5986ba7a14effe95d80961a747a5a009e2e7a34b1103d0fb439`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fdb69cfdb3c3a243cd47bb19a0e6e715402297b09f3ba260428949cbfb1f63`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16dec1a6a64015615a56421801d1af7b94dac5d75f2e649ac9446f9d4998925`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 6.6 KB (6595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c530a185b1bcf36a530f35e99fc91e5acfcb79e1df394005b77d615379443f`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 5.1 MB (5130688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3b0ee6edf200037e72728d125ac1875c28cff2f3315b7f6dfddd115e231774`  
		Last Modified: Sat, 25 Jul 2020 00:20:11 GMT  
		Size: 191.7 MB (191734259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff539e5195274a35e63f67a1ee5b10acdfb72606ecadc91b99163b94b6712278`  
		Last Modified: Sat, 25 Jul 2020 00:19:53 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89931096a78610e20926f579388adf675a05053f3b2bda65a54ea1125658c2a`  
		Last Modified: Sat, 25 Jul 2020 00:19:58 GMT  
		Size: 18.2 MB (18225201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.3-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:33466c44ca5aa70f73533074a1225beac20a36c9944729f7bd6f758b13c8a468
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.5 MB (388496286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7f1fc5107b7366e103c389cc8b21876af7ee133a20167fe0cb3e1652cec439`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:01:16 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 17:01:17 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 24 Jul 2020 17:01:17 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 17:01:17 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 17:01:26 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:01:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 17:01:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 24 Jul 2020 17:01:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:01:27 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:01:28 GMT
COPY dir:9bf54ffdc4f4c7668f2f626dc636555b60354b8e5fb3510b77868c9d2b4b15cd in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 17:01:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 17:01:28 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 24 Jul 2020 17:01:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 17:01:36 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 17:01:36 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 17:01:36 GMT
USER 1001
# Fri, 24 Jul 2020 17:01:36 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:01:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:01:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 17:01:43 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 17:01:43 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 24 Jul 2020 17:04:41 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 24 Jul 2020 17:04:44 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 24 Jul 2020 17:05:06 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c44e6738468daa98b6d327933034ec0cb733c95a2007674ff05b6c30a5fd70`  
		Last Modified: Fri, 24 Jul 2020 17:06:33 GMT  
		Size: 13.6 MB (13600361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7590c4af8ac9441f141a0c300e9917112e7ba2b9ce930d53ec87af7fac56815`  
		Last Modified: Fri, 24 Jul 2020 17:06:32 GMT  
		Size: 718.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaca23a1a364d9435865be5768b2af5098167221aec2380c5fd62ffddcfe03e`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 5.7 KB (5651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c558a63e757c48d4e48167a1fbed2d9b68f51edb62868eda0d26b1e41f7f4475`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb40616101654b8287326c88de0c3c7ff1f7f658f64b1a344a6bb78193e623eb`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1542378324e868eb6e3c06c31a9cc234527b246c2000d5eb78a1aa62eb24eaf`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 6.6 KB (6588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771e0d85d141d09682f359c596f04c6e8fbd2d568df318380d72d46cc1d8a48c`  
		Last Modified: Fri, 24 Jul 2020 17:06:31 GMT  
		Size: 5.7 MB (5679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f227a136769ee286691d9c81a2572df96610e881aa7649440bcd4e5e81ae036`  
		Last Modified: Fri, 24 Jul 2020 17:06:47 GMT  
		Size: 192.3 MB (192283514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3399d4b60ac3c570ce5fdcdf082362528c8573348f1226b6ecf33f8ebc9ccb96`  
		Last Modified: Fri, 24 Jul 2020 17:06:37 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb9692442b29a0131481d30fe68bf42cbc44d96029c49c3b9073e3d462b56a`  
		Last Modified: Fri, 24 Jul 2020 17:06:40 GMT  
		Size: 21.2 MB (21181242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.3-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:eed85d062260a9b377704280825df242e13d021c024d2de4054cbfcd26325fc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.3-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:293735a316c1c2396b8d6008e6eea5f0ca22a707c88e611b47639b61b4be1253
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.3 MB (179286593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3838bfcdd4e0d825e6759ab529bbf8f23cc7bc48ed5542819c780e59d5e6ad5`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:18:43 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 20:18:43 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 24 Jul 2020 20:18:43 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 20:18:43 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 20:18:52 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 20:18:52 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 20:18:52 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 24 Jul 2020 20:18:53 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:18:54 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 20:18:54 GMT
COPY dir:9bf54ffdc4f4c7668f2f626dc636555b60354b8e5fb3510b77868c9d2b4b15cd in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 20:18:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 20:18:54 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 24 Jul 2020 20:18:55 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 20:19:07 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 20:19:07 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:19:07 GMT
USER 1001
# Fri, 24 Jul 2020 20:19:07 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 20:19:07 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 20:19:08 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec3875d1981f8340320077504c6a6c93667702173fe043e0489ddd717300bd`  
		Last Modified: Fri, 24 Jul 2020 20:26:11 GMT  
		Size: 13.6 MB (13600360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be31ae85d236398b806e01b917763a6a2e93865c9379874c6a1dc0f0253afb7`  
		Last Modified: Fri, 24 Jul 2020 20:26:09 GMT  
		Size: 676.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0619b60bfbff10c8c4469472a116096723d0974f2d20e39e36a0a1d7491ed3`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 5.6 KB (5623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316afa43b4edf142d60e74140d6094b43144a14393c090203f818e12a08a5f7d`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955621de6b3af6e0596e0ff9ceb59cb968e6079d19a250291ef178f041cf75ac`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 57.4 KB (57421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25992359574a6609f17e53fce3486e5dcf2412387208220b0b2297aeb1b1d821`  
		Last Modified: Fri, 24 Jul 2020 20:26:08 GMT  
		Size: 6.5 KB (6486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3188389b530abb3afd44b72899c849f3e6da3e825e7b544bb315076f2527cdc5`  
		Last Modified: Fri, 24 Jul 2020 20:26:09 GMT  
		Size: 5.6 MB (5583146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.3-kernel-java8-ibmjava` - linux; 386

```console
$ docker pull websphere-liberty@sha256:21c2835a021b91c09268f12dc8f3c61f590c1b34d7669aeacf3792d83a7ef016
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162573580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e89243446a76e85ea4bf274dd0ad9e6fd0e763e50ced541577b62bee7dfcb74`
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

### `websphere-liberty:20.0.0.3-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:8f01286547c3e2127193ff96283157ec8b5ea95eda18291a4568907081bbd193
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191157451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b048197867b3349fa53e10152ef42522fa62b89252773c9f0aadb3b6e6b4afb1`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Sat, 25 Jul 2020 00:06:23 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Sat, 25 Jul 2020 00:06:28 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Sat, 25 Jul 2020 00:06:34 GMT
ARG LIBERTY_URL
# Sat, 25 Jul 2020 00:06:38 GMT
ARG DOWNLOAD_OPTIONS=
# Sat, 25 Jul 2020 00:07:24 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Sat, 25 Jul 2020 00:07:30 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Jul 2020 00:07:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Sat, 25 Jul 2020 00:07:39 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Sat, 25 Jul 2020 00:07:51 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Sat, 25 Jul 2020 00:07:53 GMT
COPY dir:9bf54ffdc4f4c7668f2f626dc636555b60354b8e5fb3510b77868c9d2b4b15cd in /opt/ibm/helpers/ 
# Sat, 25 Jul 2020 00:07:54 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Sat, 25 Jul 2020 00:07:56 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Sat, 25 Jul 2020 00:08:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Sat, 25 Jul 2020 00:08:26 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Sat, 25 Jul 2020 00:08:28 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Sat, 25 Jul 2020 00:08:32 GMT
USER 1001
# Sat, 25 Jul 2020 00:08:36 GMT
EXPOSE 9080 9443
# Sat, 25 Jul 2020 00:08:40 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Sat, 25 Jul 2020 00:08:45 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68390033a4e2962c71f3ced7baad21f26acb7b8dbcae568d847ad3b404758b7`  
		Last Modified: Sat, 25 Jul 2020 00:19:44 GMT  
		Size: 13.6 MB (13600991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcf7d7a32e4f97a61e40c30604f55f21db767b36011a2bdc147a59d0dbdfe77`  
		Last Modified: Sat, 25 Jul 2020 00:19:42 GMT  
		Size: 719.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a114806261868a1d971b16c9fe852267af5bf7faf42a1680b6319366681410d4`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 5.7 KB (5651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751ea1f4cd43f5986ba7a14effe95d80961a747a5a009e2e7a34b1103d0fb439`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fdb69cfdb3c3a243cd47bb19a0e6e715402297b09f3ba260428949cbfb1f63`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16dec1a6a64015615a56421801d1af7b94dac5d75f2e649ac9446f9d4998925`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 6.6 KB (6595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c530a185b1bcf36a530f35e99fc91e5acfcb79e1df394005b77d615379443f`  
		Last Modified: Sat, 25 Jul 2020 00:19:39 GMT  
		Size: 5.1 MB (5130688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.3-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:63c1d5d8feeb0aa01bfadbef5b0d6b29d7a7901a37188786730ab814073daf6a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.0 MB (175030584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f27d6e758e90717e1ad284dc94bd8c90dc498da186fa756afd544f5c54db6720`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:01:16 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.3 org.opencontainers.image.revision=cl200320200305-1433 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 17:01:17 GMT
ENV LIBERTY_VERSION=20.0.0_03
# Fri, 24 Jul 2020 17:01:17 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 17:01:17 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 17:01:26 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:01:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 17:01:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.3 BuildLabel=cl200320200305-1433
# Fri, 24 Jul 2020 17:01:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 17:01:27 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 17:01:28 GMT
COPY dir:9bf54ffdc4f4c7668f2f626dc636555b60354b8e5fb3510b77868c9d2b4b15cd in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 17:01:28 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 17:01:28 GMT
COPY dir:9277507d983008afcf8df6e0bfe2735bd4e92717515dbb3a7e268c830f213489 in /licenses/ 
# Fri, 24 Jul 2020 17:01:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 17:01:36 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 17:01:36 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 17:01:36 GMT
USER 1001
# Fri, 24 Jul 2020 17:01:36 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 17:01:36 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 17:01:37 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c44e6738468daa98b6d327933034ec0cb733c95a2007674ff05b6c30a5fd70`  
		Last Modified: Fri, 24 Jul 2020 17:06:33 GMT  
		Size: 13.6 MB (13600361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7590c4af8ac9441f141a0c300e9917112e7ba2b9ce930d53ec87af7fac56815`  
		Last Modified: Fri, 24 Jul 2020 17:06:32 GMT  
		Size: 718.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aaca23a1a364d9435865be5768b2af5098167221aec2380c5fd62ffddcfe03e`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 5.7 KB (5651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c558a63e757c48d4e48167a1fbed2d9b68f51edb62868eda0d26b1e41f7f4475`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb40616101654b8287326c88de0c3c7ff1f7f658f64b1a344a6bb78193e623eb`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 57.4 KB (57426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1542378324e868eb6e3c06c31a9cc234527b246c2000d5eb78a1aa62eb24eaf`  
		Last Modified: Fri, 24 Jul 2020 17:06:30 GMT  
		Size: 6.6 KB (6588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771e0d85d141d09682f359c596f04c6e8fbd2d568df318380d72d46cc1d8a48c`  
		Last Modified: Fri, 24 Jul 2020 17:06:31 GMT  
		Size: 5.7 MB (5679125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.6-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:3e8fab402454b20ac0a6d8a1dd3517d1d6624d158578b57e80da1718aaba3bd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.6-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:0a49e818d465071fb931b6e76095fdb37f9dce1559d7d6eb3fa8efa671b1b76e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.7 MB (394686321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:234230036c2c2155aac55d55e951a08e2c2603d25ff59444b61f4c69863bf1c9`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:12:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.6 org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 20:12:53 GMT
ENV LIBERTY_VERSION=20.0.0_06
# Fri, 24 Jul 2020 20:12:53 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 20:12:54 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 20:13:02 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 20:13:02 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 20:13:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.6 BuildLabel=cl200620200528-0414
# Fri, 24 Jul 2020 20:13:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:13:04 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 20:13:04 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 20:13:04 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 20:13:05 GMT
COPY dir:f50ec19c0b3217fa3d6d42c3ce4a254879f817de03e99e13f96ba6b66fb6862e in /licenses/ 
# Fri, 24 Jul 2020 20:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 20:13:17 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 20:13:17 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:13:17 GMT
USER 1001
# Fri, 24 Jul 2020 20:13:18 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 20:13:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 20:13:18 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 20:13:22 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:13:23 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 24 Jul 2020 20:17:40 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 24 Jul 2020 20:17:40 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 24 Jul 2020 20:18:24 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ef1263502c7b527c0eee13e07e7914b3ba6749920f2a43852ca9831bbc8a25`  
		Last Modified: Fri, 24 Jul 2020 20:25:46 GMT  
		Size: 13.8 MB (13764847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9286cdd6d77ec006f0fa8477fcd84847b00a68ec3c3f591108846fff7cdbd`  
		Last Modified: Fri, 24 Jul 2020 20:25:44 GMT  
		Size: 652.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73b8d72ac274a1c0beb37bdbddf5e586026370304f307bade20548323d87a`  
		Last Modified: Fri, 24 Jul 2020 20:25:43 GMT  
		Size: 9.0 KB (9034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c552730893695ee2ad7e4492173a4829369b43af7773fd0fa74c3988650f081`  
		Last Modified: Fri, 24 Jul 2020 20:25:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c17708317690a45c443ff3458b2c60b6f9e31c9582577327c920979c686274f`  
		Last Modified: Fri, 24 Jul 2020 20:25:43 GMT  
		Size: 57.2 KB (57201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6263da67822f1d137e928334af740d9f30d3fb96f64c9bfb2419c364e418adc3`  
		Last Modified: Fri, 24 Jul 2020 20:25:44 GMT  
		Size: 9.9 KB (9915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7560c198c89bcd9ae0892cb3a6bde5d6fe82ef1df6654ffa26da964cdb11c2`  
		Last Modified: Fri, 24 Jul 2020 20:25:44 GMT  
		Size: 5.5 MB (5524368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197d384ce8e90a6163112c8e10790d49cbeccb06cbdfdc10b21e3aa112bd4652`  
		Last Modified: Fri, 24 Jul 2020 20:26:05 GMT  
		Size: 194.6 MB (194571574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694d47079e092db1dddfcdd93c4dcab466eb4c63afe120ca3bd435006d7a5292`  
		Last Modified: Fri, 24 Jul 2020 20:25:49 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc49e4efebc0b84764b9eaa3215a248c131ebfe02dc3ae6646ea9821e61cae5`  
		Last Modified: Fri, 24 Jul 2020 20:25:54 GMT  
		Size: 20.7 MB (20714900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.6-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:0b65a33c54ffbecb20271582e55f6cacb165094d5c17377917d93ffd2710ce59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.2 MB (404170976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:764904c1b482c4dee7e3e96ca763ded6e25a46e08eb76fc70d6734dd155b4626`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 23:55:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.6 org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 23:55:13 GMT
ENV LIBERTY_VERSION=20.0.0_06
# Fri, 24 Jul 2020 23:55:20 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 23:55:34 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 23:56:28 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 23:56:32 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 23:56:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.6 BuildLabel=cl200620200528-0414
# Fri, 24 Jul 2020 23:56:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 23:56:45 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 23:56:47 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 23:56:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 23:56:52 GMT
COPY dir:f50ec19c0b3217fa3d6d42c3ce4a254879f817de03e99e13f96ba6b66fb6862e in /licenses/ 
# Fri, 24 Jul 2020 23:57:08 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 23:57:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 23:57:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:57:41 GMT
USER 1001
# Fri, 24 Jul 2020 23:57:47 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 23:57:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 23:57:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 23:58:06 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:58:10 GMT
ARG REPOSITORIES_PROPERTIES=
# Sat, 25 Jul 2020 00:04:29 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Sat, 25 Jul 2020 00:04:38 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Sat, 25 Jul 2020 00:05:59 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c2ffb156f34435d8442c358b7ff42341e45881a567b41bbcece8dfc82b7a30`  
		Last Modified: Sat, 25 Jul 2020 00:19:02 GMT  
		Size: 13.8 MB (13765363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6662e13d4e904cf2ebb57e1869c0590d2805e98c8873b7ecabbf365780146`  
		Last Modified: Sat, 25 Jul 2020 00:18:59 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe0559d3d2e6ed739d4d0492371f6df834b9056cb0cd43792ed0723b2b211bf`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d9acb2f8b1998988e5aea6d43f21c25aea647d05a87f652db0db8fda100718`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164773c2489a0292abcd9a8a9be71f3b4f561e9b7b0aa23bdd5524feb081374`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 57.2 KB (57209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6726814067f57cdf140f4dedb42e17a9d81b5861e719992b391d9b3943d94c0a`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 10.0 KB (10028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1315728af23fe53027582ad2aaa93e485a6a39b7f1b328e29492b32853968ac5`  
		Last Modified: Sat, 25 Jul 2020 00:18:56 GMT  
		Size: 5.1 MB (5133171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db8ba188ae85d86d423799e64df746d0f34d4900973de6a75b562a9e481bed2`  
		Last Modified: Sat, 25 Jul 2020 00:19:29 GMT  
		Size: 194.2 MB (194188775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad25fc845092175e91659cbd5e43ffa0be29ed404fd8b0100a5318527d8cf76`  
		Last Modified: Sat, 25 Jul 2020 00:19:12 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8325fe7164b0a14900e9bfb1de64b31fb4f697d8f62f6607db0f489940d784d`  
		Last Modified: Sat, 25 Jul 2020 00:19:16 GMT  
		Size: 18.7 MB (18650347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.6-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:3dfcc8ecd7fd21febf91a744119a753cdb0ddc6b175e5210ef237ebe1d3edecf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.4 MB (391399863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9791940a33dbeeba38daa69b1bea49516398b6385279124ba578cd71522fd51e`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 16:57:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.6 org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 16:57:02 GMT
ENV LIBERTY_VERSION=20.0.0_06
# Fri, 24 Jul 2020 16:57:03 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 16:57:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 16:57:11 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:57:12 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 16:57:12 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.6 BuildLabel=cl200620200528-0414
# Fri, 24 Jul 2020 16:57:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 16:57:13 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 16:57:13 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 16:57:13 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 16:57:13 GMT
COPY dir:f50ec19c0b3217fa3d6d42c3ce4a254879f817de03e99e13f96ba6b66fb6862e in /licenses/ 
# Fri, 24 Jul 2020 16:57:14 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 16:57:21 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 16:57:21 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:57:21 GMT
USER 1001
# Fri, 24 Jul 2020 16:57:22 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 16:57:22 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 16:57:22 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Fri, 24 Jul 2020 16:57:26 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:57:26 GMT
ARG REPOSITORIES_PROPERTIES=
# Fri, 24 Jul 2020 17:00:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Fri, 24 Jul 2020 17:00:41 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Fri, 24 Jul 2020 17:01:07 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738703e59adf35bd04e99e0f22e878f0451b9e009eebd5432c87d638f2c3d207`  
		Last Modified: Fri, 24 Jul 2020 17:06:11 GMT  
		Size: 13.8 MB (13764811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9b9392588c43af0cfff578e8af18f00a7f05a4d9e6f6c2498736bb6c805f4e`  
		Last Modified: Fri, 24 Jul 2020 17:06:10 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0f5c1b5493ccb321c6e5d6a4bd0e31ea975dd226eaad29bf03dff8d81339a1`  
		Last Modified: Fri, 24 Jul 2020 17:06:07 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd1d1f406567023adede406c210030620162956073e98b3ac5a33da4eb18d35`  
		Last Modified: Fri, 24 Jul 2020 17:06:08 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028c52383870053a804588d566d818b96701a51396de55ac006d6d8292a17d`  
		Last Modified: Fri, 24 Jul 2020 17:06:07 GMT  
		Size: 57.2 KB (57207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4c9c15027da9dc65e7d2179a36d1c5870c18782ae70bb743cd1850f45ff471`  
		Last Modified: Fri, 24 Jul 2020 17:06:07 GMT  
		Size: 10.0 KB (10009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45f9cdeaad3457dc2a60abb01e83e92fe1dca7acbc33f95f06739419899f72d`  
		Last Modified: Fri, 24 Jul 2020 17:06:08 GMT  
		Size: 5.7 MB (5658321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae1336eca9f26460fd103a43ed99770d41b5f6b242d4093a7a7fb7f2178bded`  
		Last Modified: Fri, 24 Jul 2020 17:06:25 GMT  
		Size: 194.7 MB (194713484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f0cd16aeee16261868b59366e4b9ee7bfa0530c80b35cf745aa7a544e71266`  
		Last Modified: Fri, 24 Jul 2020 17:06:16 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60142683eb3ed1942cb9b9e88347cc7cce57015c4e2ecc37176445389240eca`  
		Last Modified: Fri, 24 Jul 2020 17:06:18 GMT  
		Size: 21.5 MB (21504610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.6-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:526c196aede934ef9680a203bf87b218f1ca9fc00d54ab83bcb7b82d0723dc29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.6-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:af13259e98c20190c2c33caac2e99292256dd2450a66e9751d6dd553600bcbc4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.4 MB (179398899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50cb05b24a5940f983c709122515a93fdbe362d8b6d96c596f1cc9526772a949`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:12:53 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.6 org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 20:12:53 GMT
ENV LIBERTY_VERSION=20.0.0_06
# Fri, 24 Jul 2020 20:12:53 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 20:12:54 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 20:13:02 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 20:13:02 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 20:13:03 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.6 BuildLabel=cl200620200528-0414
# Fri, 24 Jul 2020 20:13:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 20:13:04 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 20:13:04 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 20:13:04 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 20:13:05 GMT
COPY dir:f50ec19c0b3217fa3d6d42c3ce4a254879f817de03e99e13f96ba6b66fb6862e in /licenses/ 
# Fri, 24 Jul 2020 20:13:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 20:13:17 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 20:13:17 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:13:17 GMT
USER 1001
# Fri, 24 Jul 2020 20:13:18 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 20:13:18 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 20:13:18 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ef1263502c7b527c0eee13e07e7914b3ba6749920f2a43852ca9831bbc8a25`  
		Last Modified: Fri, 24 Jul 2020 20:25:46 GMT  
		Size: 13.8 MB (13764847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb9286cdd6d77ec006f0fa8477fcd84847b00a68ec3c3f591108846fff7cdbd`  
		Last Modified: Fri, 24 Jul 2020 20:25:44 GMT  
		Size: 652.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73b8d72ac274a1c0beb37bdbddf5e586026370304f307bade20548323d87a`  
		Last Modified: Fri, 24 Jul 2020 20:25:43 GMT  
		Size: 9.0 KB (9034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c552730893695ee2ad7e4492173a4829369b43af7773fd0fa74c3988650f081`  
		Last Modified: Fri, 24 Jul 2020 20:25:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c17708317690a45c443ff3458b2c60b6f9e31c9582577327c920979c686274f`  
		Last Modified: Fri, 24 Jul 2020 20:25:43 GMT  
		Size: 57.2 KB (57201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6263da67822f1d137e928334af740d9f30d3fb96f64c9bfb2419c364e418adc3`  
		Last Modified: Fri, 24 Jul 2020 20:25:44 GMT  
		Size: 9.9 KB (9915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7560c198c89bcd9ae0892cb3a6bde5d6fe82ef1df6654ffa26da964cdb11c2`  
		Last Modified: Fri, 24 Jul 2020 20:25:44 GMT  
		Size: 5.5 MB (5524368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.6-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:b28c23ac67d85889c3d179f0197f813bf68ca036e1548f52bfc7080d54878108
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191330906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc6b56ee48300a4a7a94181efeb308e1405d1dc69b58d2c17e50de23a458bcf`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 23:55:07 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.6 org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 23:55:13 GMT
ENV LIBERTY_VERSION=20.0.0_06
# Fri, 24 Jul 2020 23:55:20 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 23:55:34 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 23:56:28 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 23:56:32 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 23:56:36 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.6 BuildLabel=cl200620200528-0414
# Fri, 24 Jul 2020 23:56:38 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 23:56:45 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 23:56:47 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 23:56:50 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 23:56:52 GMT
COPY dir:f50ec19c0b3217fa3d6d42c3ce4a254879f817de03e99e13f96ba6b66fb6862e in /licenses/ 
# Fri, 24 Jul 2020 23:57:08 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 23:57:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 23:57:35 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:57:41 GMT
USER 1001
# Fri, 24 Jul 2020 23:57:47 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 23:57:49 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 23:57:53 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c2ffb156f34435d8442c358b7ff42341e45881a567b41bbcece8dfc82b7a30`  
		Last Modified: Sat, 25 Jul 2020 00:19:02 GMT  
		Size: 13.8 MB (13765363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6662e13d4e904cf2ebb57e1869c0590d2805e98c8873b7ecabbf365780146`  
		Last Modified: Sat, 25 Jul 2020 00:18:59 GMT  
		Size: 694.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe0559d3d2e6ed739d4d0492371f6df834b9056cb0cd43792ed0723b2b211bf`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 9.1 KB (9059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d9acb2f8b1998988e5aea6d43f21c25aea647d05a87f652db0db8fda100718`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e164773c2489a0292abcd9a8a9be71f3b4f561e9b7b0aa23bdd5524feb081374`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 57.2 KB (57209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6726814067f57cdf140f4dedb42e17a9d81b5861e719992b391d9b3943d94c0a`  
		Last Modified: Sat, 25 Jul 2020 00:18:55 GMT  
		Size: 10.0 KB (10028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1315728af23fe53027582ad2aaa93e485a6a39b7f1b328e29492b32853968ac5`  
		Last Modified: Sat, 25 Jul 2020 00:18:56 GMT  
		Size: 5.1 MB (5133171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.6-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:ce9070e9b8e0327ea6675376d58f0066508206424fb0e0d18633f07ed4c8f27e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.2 MB (175180819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49046289e4466ad223970fe1eb455071e1f9f70c2f7b5b3111a5b1d56bbdd2b7`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Fri, 24 Jul 2020 16:57:02 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.6 org.opencontainers.image.revision=cl200620200528-0414 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Fri, 24 Jul 2020 16:57:02 GMT
ENV LIBERTY_VERSION=20.0.0_06
# Fri, 24 Jul 2020 16:57:03 GMT
ARG LIBERTY_URL
# Fri, 24 Jul 2020 16:57:03 GMT
ARG DOWNLOAD_OPTIONS=
# Fri, 24 Jul 2020 16:57:11 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:57:12 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 16:57:12 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.6 BuildLabel=cl200620200528-0414
# Fri, 24 Jul 2020 16:57:12 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Fri, 24 Jul 2020 16:57:13 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 16:57:13 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Fri, 24 Jul 2020 16:57:13 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Fri, 24 Jul 2020 16:57:13 GMT
COPY dir:f50ec19c0b3217fa3d6d42c3ce4a254879f817de03e99e13f96ba6b66fb6862e in /licenses/ 
# Fri, 24 Jul 2020 16:57:14 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 16:57:21 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Fri, 24 Jul 2020 16:57:21 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:57:21 GMT
USER 1001
# Fri, 24 Jul 2020 16:57:22 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 16:57:22 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Fri, 24 Jul 2020 16:57:22 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738703e59adf35bd04e99e0f22e878f0451b9e009eebd5432c87d638f2c3d207`  
		Last Modified: Fri, 24 Jul 2020 17:06:11 GMT  
		Size: 13.8 MB (13764811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9b9392588c43af0cfff578e8af18f00a7f05a4d9e6f6c2498736bb6c805f4e`  
		Last Modified: Fri, 24 Jul 2020 17:06:10 GMT  
		Size: 692.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0f5c1b5493ccb321c6e5d6a4bd0e31ea975dd226eaad29bf03dff8d81339a1`  
		Last Modified: Fri, 24 Jul 2020 17:06:07 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd1d1f406567023adede406c210030620162956073e98b3ac5a33da4eb18d35`  
		Last Modified: Fri, 24 Jul 2020 17:06:08 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da028c52383870053a804588d566d818b96701a51396de55ac006d6d8292a17d`  
		Last Modified: Fri, 24 Jul 2020 17:06:07 GMT  
		Size: 57.2 KB (57207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4c9c15027da9dc65e7d2179a36d1c5870c18782ae70bb743cd1850f45ff471`  
		Last Modified: Fri, 24 Jul 2020 17:06:07 GMT  
		Size: 10.0 KB (10009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45f9cdeaad3457dc2a60abb01e83e92fe1dca7acbc33f95f06739419899f72d`  
		Last Modified: Fri, 24 Jul 2020 17:06:08 GMT  
		Size: 5.7 MB (5658321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.8-full-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:11576f331db34eb78d772eb70ce4365abefeec5495128e0021cc5db28112ef73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.8-full-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:7db591017b3034538a4c0a96274c5be8027321a81958a9171fe57830c4256caf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396132731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfac0cead3d5f6a8ddf105f86acb9067db2012820b0e1faab09c75e55c94c0c4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:53:14 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:53:14 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:53:15 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:53:25 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:53:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:53:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:53:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:53:30 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:53:46 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:53:46 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:53:46 GMT
USER 1001
# Thu, 30 Jul 2020 22:53:47 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:53:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:53:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:53:54 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:53:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:57:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:57:18 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:58:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d81557d9cc6e59acdc25818a46ac945a48485de139eafe8bb30d05354c5663`  
		Last Modified: Thu, 30 Jul 2020 22:59:14 GMT  
		Size: 13.8 MB (13783714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c62bea2d5f1dbecdfea3cfc3ce8dbb0110306e3253a8aee0bac9727927313bd`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75f940f290330a5ec1d3cb97465332a686e2cfb2043698beeb50af24401e2f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.0 KB (9036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8160cd73a82cb75737ff72bb9e5c2cd4a33bc6719cee4a7f1fc72020fd04ec3f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aae8a6f675ecb553ec4c147a415cfedec03e426d59cad79e1901c7cfa1ee41f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 57.3 KB (57343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acbfae58da0e5272fe9e835ebc7f7038640b3db4287da710ee115f49638df96`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.9 KB (9922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37146a46875370b17578a3e68e6bee5257a810ff04066dfac7b4aab9ec66e205`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 5.7 MB (5653146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7cd1a65c8aa35cbc26ee655a792d4bb7f90799023cda6475cc1e77c600e2df`  
		Last Modified: Thu, 30 Jul 2020 22:59:33 GMT  
		Size: 194.8 MB (194771855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926165a268d82024ede2797d8b3921a0903ff61c73de3897b7781e103dd99b4e`  
		Last Modified: Thu, 30 Jul 2020 22:59:17 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f9345f344474ecf0956527041c1c5ceed467816820d14c0ab0438ddf61177c`  
		Last Modified: Thu, 30 Jul 2020 22:59:21 GMT  
		Size: 21.8 MB (21813225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.8-full-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:430f15ad7d64a12f0756f0990bfaee07c072040d71fa611dfd1c25a0deafc42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.3 MB (404303249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ad7606f69c19e69a11b7db356fc1cdf166271143f41d40e77a6d18ba18cf55`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:34:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:34:43 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:34:50 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:34:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:35:33 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:35:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:35:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:35:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:36:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:36:08 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:36:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:36:11 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:36:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:36:59 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:37:03 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:37:06 GMT
USER 1001
# Thu, 30 Jul 2020 22:37:08 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:37:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:37:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:37:47 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:38:00 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:42:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:42:45 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:44:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a068ff0da5b15b15ba95339c011442006ce76ce4486a0df1d1253334750430dc`  
		Last Modified: Thu, 30 Jul 2020 22:45:17 GMT  
		Size: 13.8 MB (13784331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d084fee2f71c0a9c627cae934b97e3d7fd0264b883e2e0577d504ac127f6`  
		Last Modified: Thu, 30 Jul 2020 22:45:13 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4a673c35c7b2ee99c2cc4b4fe32b90e224e208e59254216feaa12a7e8f5bf9`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d9962284e436c4de6df54d7b161a85de69aaa4abc0aa94d29e9dadd428032`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3984e000819787c569ebfb279b6e64feff4f4bd0e22e092d6712dd81b5a6e5`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 57.3 KB (57338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425b10ab6483f5b2d6caf62c9223d3d9ae41255ece708dabc9e39a85fe005f9b`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 10.0 KB (10029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7002fa317a4748e3779742ee40bf208b1150736b7e138a65cc50931c862be67`  
		Last Modified: Thu, 30 Jul 2020 22:45:12 GMT  
		Size: 5.1 MB (5148853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7781f340ee342e4e325d6d6620b79a479948c31a7c9720c8aa0d661cd93776dd`  
		Last Modified: Thu, 30 Jul 2020 22:45:43 GMT  
		Size: 194.3 MB (194285373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa37cf123a052f161a723ef3bb27d8ced6bcc4ae679c9dd121267b853ed8840`  
		Last Modified: Thu, 30 Jul 2020 22:45:25 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94826eb4daee4759e15bfffe1978f4357f6a806be74e2a9b54fe290dfcf6cc5`  
		Last Modified: Thu, 30 Jul 2020 22:45:29 GMT  
		Size: 18.7 MB (18651233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.8-full-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:fb94705fc4dcd69a6aed5e9bbd5cc77b07550af31a08026c34b8c8219a858e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.6 MB (391608162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60602e1245dd6f8c53834774155a20632c21c1e39c8e0b8a0c7a35e28da5779f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:54:13 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:54:13 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:54:14 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:54:22 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:54:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:54:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:54:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:24 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:54:25 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:54:32 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:54:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:54:33 GMT
USER 1001
# Thu, 30 Jul 2020 22:54:33 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:54:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:54:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:54:40 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:54:40 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:58:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:58:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:58:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8346e72ed70efe0c0afcb3f476069fa0dd103c6e8eaca1a7dc766312488a38f`  
		Last Modified: Thu, 30 Jul 2020 22:59:32 GMT  
		Size: 13.8 MB (13783695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188b9215c9f1f5e014b767c988af83915874b6256073df6b9d4d35f52a44859`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83fae6751a1269cdd545d2c07a3b1b0ffe8cc135724d3a4fce7525a834c0b5a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 9.1 KB (9064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850405cc03be76d38215a47e3ffa25cd8b5972d9068d3f9cbf57f70be3922a9`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5937f0b9af37ba1e917a21ca9e650eed812ed9e0e399d1a8196f4e53dad97a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 57.3 KB (57346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be67f780d9694352da879fd5c0a3331267cf90e7ab2c311e10e6a6d9ac4824a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 10.0 KB (10016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c85c5c2e67f168f813579e6d9c843a3ecc0df1092afa9a14ad1d57dd08c21c`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 5.7 MB (5665376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f578b4f9b115993a3432a3b58d2b8d36878374169ee38d8061b01ff03168cd1`  
		Last Modified: Thu, 30 Jul 2020 22:59:46 GMT  
		Size: 194.8 MB (194805693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d174a918ac23ee6556cb2fcefce022416c92ce3439d40ff6efc64f2ef430b30`  
		Last Modified: Thu, 30 Jul 2020 22:59:36 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4dd1686e619f35bfcffb45f5754ee58834a05edf5595d594c80cca0f27b2265`  
		Last Modified: Thu, 30 Jul 2020 22:59:39 GMT  
		Size: 21.6 MB (21594611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:20.0.0.8-kernel-java8-ibmjava`

```console
$ docker pull websphere-liberty@sha256:4d9418f0f4712265ced855b5d3349bb961cfb930a44955fe280dc34abcf6a1a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:20.0.0.8-kernel-java8-ibmjava` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:0482d46102f07ec8569774e4b397b6185f0fefbe4c240820d2e0b00fc1899e26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d2ea8a2db41d6dd356c634d44facd87f775678aa6acb5737e07008f6aacbbe`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:53:14 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:53:14 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:53:15 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:53:25 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:53:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:53:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:53:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:53:30 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:53:46 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:53:46 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:53:46 GMT
USER 1001
# Thu, 30 Jul 2020 22:53:47 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:53:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:53:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d81557d9cc6e59acdc25818a46ac945a48485de139eafe8bb30d05354c5663`  
		Last Modified: Thu, 30 Jul 2020 22:59:14 GMT  
		Size: 13.8 MB (13783714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c62bea2d5f1dbecdfea3cfc3ce8dbb0110306e3253a8aee0bac9727927313bd`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75f940f290330a5ec1d3cb97465332a686e2cfb2043698beeb50af24401e2f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.0 KB (9036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8160cd73a82cb75737ff72bb9e5c2cd4a33bc6719cee4a7f1fc72020fd04ec3f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aae8a6f675ecb553ec4c147a415cfedec03e426d59cad79e1901c7cfa1ee41f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 57.3 KB (57343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acbfae58da0e5272fe9e835ebc7f7038640b3db4287da710ee115f49638df96`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.9 KB (9922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37146a46875370b17578a3e68e6bee5257a810ff04066dfac7b4aab9ec66e205`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 5.7 MB (5653146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.8-kernel-java8-ibmjava` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:e0f5dd1bebce3bc4b563b49c9cde2cbcc25436a89dfb08aa9b139b43f6f5c7b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191365694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8954cf9046bbe4e4792fde5bb6fcfef148c350b0c3e5fddf209687568cf698`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:34:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:34:43 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:34:50 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:34:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:35:33 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:35:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:35:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:35:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:36:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:36:08 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:36:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:36:11 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:36:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:36:59 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:37:03 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:37:06 GMT
USER 1001
# Thu, 30 Jul 2020 22:37:08 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:37:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:37:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a068ff0da5b15b15ba95339c011442006ce76ce4486a0df1d1253334750430dc`  
		Last Modified: Thu, 30 Jul 2020 22:45:17 GMT  
		Size: 13.8 MB (13784331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d084fee2f71c0a9c627cae934b97e3d7fd0264b883e2e0577d504ac127f6`  
		Last Modified: Thu, 30 Jul 2020 22:45:13 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4a673c35c7b2ee99c2cc4b4fe32b90e224e208e59254216feaa12a7e8f5bf9`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d9962284e436c4de6df54d7b161a85de69aaa4abc0aa94d29e9dadd428032`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3984e000819787c569ebfb279b6e64feff4f4bd0e22e092d6712dd81b5a6e5`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 57.3 KB (57338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425b10ab6483f5b2d6caf62c9223d3d9ae41255ece708dabc9e39a85fe005f9b`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 10.0 KB (10029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7002fa317a4748e3779742ee40bf208b1150736b7e138a65cc50931c862be67`  
		Last Modified: Thu, 30 Jul 2020 22:45:12 GMT  
		Size: 5.1 MB (5148853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:20.0.0.8-kernel-java8-ibmjava` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f75f7ecfb79b65f65a4bf85e89156859511db509d8ad0a959120cdb769aecaf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.2 MB (175206909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0489e34c5bf4ccbc796c2f9a9ce1c15583ea96d38ae63d4a5a1ddb26ad028a8c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:54:13 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:54:13 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:54:14 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:54:22 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:54:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:54:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:54:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:24 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:54:25 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:54:32 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:54:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:54:33 GMT
USER 1001
# Thu, 30 Jul 2020 22:54:33 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:54:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:54:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8346e72ed70efe0c0afcb3f476069fa0dd103c6e8eaca1a7dc766312488a38f`  
		Last Modified: Thu, 30 Jul 2020 22:59:32 GMT  
		Size: 13.8 MB (13783695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188b9215c9f1f5e014b767c988af83915874b6256073df6b9d4d35f52a44859`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83fae6751a1269cdd545d2c07a3b1b0ffe8cc135724d3a4fce7525a834c0b5a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 9.1 KB (9064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850405cc03be76d38215a47e3ffa25cd8b5972d9068d3f9cbf57f70be3922a9`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5937f0b9af37ba1e917a21ca9e650eed812ed9e0e399d1a8196f4e53dad97a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 57.3 KB (57346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be67f780d9694352da879fd5c0a3331267cf90e7ab2c311e10e6a6d9ac4824a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 10.0 KB (10016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c85c5c2e67f168f813579e6d9c843a3ecc0df1092afa9a14ad1d57dd08c21c`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 5.7 MB (5665376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:beta`

```console
$ docker pull websphere-liberty@sha256:3046d85c565439c48ee498055fbc67317de36f78446a67d1509b789f0ca5534b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:beta` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:76a252b9b49db7fd1b0434caa3708d870e39aed6d1021f66d637d164b3eaf149
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.7 MB (260656576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d0f1f55716fa315e1011e8df5e1b91dc23a51f66a54f947d692eb984cf3576`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:52:40 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=2020.8.0.0 org.opencontainers.image.revision=cl200820200721-1900
# Thu, 30 Jul 2020 22:52:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends unzip     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default
# Thu, 30 Jul 2020 22:52:47 GMT
ENV LIBERTY_VERSION=2020.8.0_0
# Thu, 30 Jul 2020 22:53:02 GMT
RUN LIBERTY_URL=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 3 | sed -n 's/\s*webProfile7:\s//p' | tr -d '\r')      && echo $LIBERTY_URL     && wget -q $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp-beta.zip     && unzip -q /tmp/wlp-beta.zip -d /opt/ibm     && rm /tmp/wlp-beta.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp
# Thu, 30 Jul 2020 22:53:03 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:53:03 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:53:05 GMT
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:53:05 GMT
COPY file:f1015ab5ca098f3a04cde2e721a2aa35a1ebb2e9f5eb01d378eb2264cff9a268 in /opt/ibm/wlp/usr/servers/defaultServer/ 
# Thu, 30 Jul 2020 22:53:06 GMT
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:53:07 GMT
USER 1001
# Thu, 30 Jul 2020 22:53:07 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:53:07 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e6651bad4e26bb5df12ea749faa078deebec32737274c3db71c63659146d5a`  
		Last Modified: Thu, 30 Jul 2020 22:58:59 GMT  
		Size: 377.5 KB (377500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a467f7b15e65c85be3dac5ff69bb54306feaf7edd58cc13bceb6690c88b432b4`  
		Last Modified: Thu, 30 Jul 2020 22:59:07 GMT  
		Size: 100.2 MB (100243887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8893b1cf603bd54b335d75cb5e5044cb59edb75b7328eff9acf8d122bec0a058`  
		Last Modified: Thu, 30 Jul 2020 22:58:59 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e51b1d1280979f113069e9b94d471afbd0719e7925a740ad26137448718d957`  
		Last Modified: Thu, 30 Jul 2020 22:58:59 GMT  
		Size: 426.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c14e78fc962c58f2363ae0d1e52e94e153026a33eedce3582255c692d37a76`  
		Last Modified: Thu, 30 Jul 2020 22:58:59 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:beta` - linux; 386

```console
$ docker pull websphere-liberty@sha256:a230b44724fb1d39355ff5c67c5c8a2c6a35515ba48f88efbd9573337972024b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.4 MB (249424380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9c3a6c43e11dd8ad44c7e8ed4f6d894e3c66840ec7a6c795c77f170a30964e`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:18 GMT
ADD file:1041a59a13c0d49b1cb87f211694f68be4c9b76f2deb36e2d8955b77c4d2836f in / 
# Fri, 24 Jul 2020 14:40:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:40:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:21 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 14:56:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 14:56:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:56:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 14:57:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 14:57:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 15:35:50 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=2020.7.0.0 org.opencontainers.image.revision=cl200720200625-0300
# Fri, 24 Jul 2020 15:35:57 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends unzip     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default
# Fri, 24 Jul 2020 15:35:58 GMT
ENV LIBERTY_VERSION=2020.7.0_0
# Fri, 24 Jul 2020 15:36:13 GMT
RUN LIBERTY_URL=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 3 | sed -n 's/\s*webProfile7:\s//p' | tr -d '\r')      && echo $LIBERTY_URL     && wget -q $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp-beta.zip     && unzip -q /tmp/wlp-beta.zip -d /opt/ibm     && rm /tmp/wlp-beta.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp
# Fri, 24 Jul 2020 15:36:14 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 24 Jul 2020 15:36:14 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Fri, 24 Jul 2020 15:36:16 GMT
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Fri, 24 Jul 2020 15:36:16 GMT
COPY file:f1015ab5ca098f3a04cde2e721a2aa35a1ebb2e9f5eb01d378eb2264cff9a268 in /opt/ibm/wlp/usr/servers/defaultServer/ 
# Fri, 24 Jul 2020 15:36:17 GMT
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Fri, 24 Jul 2020 15:36:17 GMT
USER 1001
# Fri, 24 Jul 2020 15:36:18 GMT
EXPOSE 9080 9443
# Fri, 24 Jul 2020 15:36:18 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:89823af3b784a3ef6d57a90159cbd5f28c863927aa03d4c43b44b6c37479fa1c`  
		Last Modified: Mon, 13 Jul 2020 15:46:56 GMT  
		Size: 27.1 MB (27123624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28677484c2569b014ecb876df3111b11e825c82629306b3af99a1c12f3b234e2`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 34.6 KB (34611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c914b15d9c03339769ddd662b893654bbc371dbed4f8cdfa29ca1c57c0bb98e`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc7dbf6d65bca5959e6f7c892f468288c27e6a0ef07eec142d4497ee07e6cd`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6390acddeaf0d5abd6917da9b4934d31bc7973be5b9dceb484774c00312c178`  
		Last Modified: Fri, 24 Jul 2020 14:59:13 GMT  
		Size: 3.0 MB (2982896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b177f3853d875c18d17b4e8f702b7a1748b053c1ef83d54efd67ab2f8450ac6`  
		Last Modified: Fri, 24 Jul 2020 14:59:27 GMT  
		Size: 118.7 MB (118707507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571258cba14f8d16169656353c609df4d23ed1c2f92392fbe75fb82720951300`  
		Last Modified: Fri, 24 Jul 2020 15:38:04 GMT  
		Size: 365.4 KB (365416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bef92777b4f3d7c19f1fbf0f09b4e63a69dda979c7c80907ebb914a5373c42`  
		Last Modified: Fri, 24 Jul 2020 15:38:13 GMT  
		Size: 100.2 MB (100206775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd909c9d78987040d776030d2c8d2e3f25b7b187acef1d216aff88bf5bd67d42`  
		Last Modified: Fri, 24 Jul 2020 15:38:03 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e94f31cf0770ed675601386730a3e7832ecb0d8afc29cc359bacc4e540b1e1`  
		Last Modified: Fri, 24 Jul 2020 15:38:03 GMT  
		Size: 425.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961b137ce0c475febe3ce5836da5e4f2da6115451252a637a3a83f88896183c6`  
		Last Modified: Fri, 24 Jul 2020 15:38:03 GMT  
		Size: 917.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:beta` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:2e9c6ec52e72187242ddf68664ab3f065edcb9206ff038c8623967bda1116d24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.0 MB (273006939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb81f2bfd8906d95a346baf419ea33612bb2c1c6346e9b7f055490cb0f130638`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:31:15 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=2020.8.0.0 org.opencontainers.image.revision=cl200820200721-1900
# Thu, 30 Jul 2020 22:32:00 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends unzip     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default
# Thu, 30 Jul 2020 22:32:09 GMT
ENV LIBERTY_VERSION=2020.8.0_0
# Thu, 30 Jul 2020 22:32:43 GMT
RUN LIBERTY_URL=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 3 | sed -n 's/\s*webProfile7:\s//p' | tr -d '\r')      && echo $LIBERTY_URL     && wget -q $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp-beta.zip     && unzip -q /tmp/wlp-beta.zip -d /opt/ibm     && rm /tmp/wlp-beta.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp
# Thu, 30 Jul 2020 22:32:55 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:33:04 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:33:39 GMT
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:33:43 GMT
COPY file:f1015ab5ca098f3a04cde2e721a2aa35a1ebb2e9f5eb01d378eb2264cff9a268 in /opt/ibm/wlp/usr/servers/defaultServer/ 
# Thu, 30 Jul 2020 22:33:59 GMT
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:34:02 GMT
USER 1001
# Thu, 30 Jul 2020 22:34:10 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:34:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991b3a61068ac77c2473e16e40957c52b97489140ccdbfecf1b1f154136f5eeb`  
		Last Modified: Thu, 30 Jul 2020 22:44:51 GMT  
		Size: 405.2 KB (405249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a8f376bae69d66e4562d36882fa91574fc19caad643b10b9cbf6f6e23b7f2`  
		Last Modified: Thu, 30 Jul 2020 22:45:00 GMT  
		Size: 100.2 MB (100243888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1274b2a346b7981aa3c3a0d1afa2e9abf97c9fe010dc5424fb6910694ff1c472`  
		Last Modified: Thu, 30 Jul 2020 22:44:51 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5786ec7e3386ed635e4c2e346e2fa6b1a5cb45719cf360c494eb3b72aca9754`  
		Last Modified: Thu, 30 Jul 2020 22:44:51 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf2fb735b811604c08427e6631284426647ee75e0eda5e4319cb21552ae0f8b`  
		Last Modified: Thu, 30 Jul 2020 22:44:51 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:beta` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:fa7dda7f2b91b3c5b1daeb53a75357764073d027179f2ba574a18c116f34d0a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256298843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6354a5696ddba5d0460bf30d372ea41b7f4646ffcd607e27e304ef1b89c8c8b9`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:53:42 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=2020.8.0.0 org.opencontainers.image.revision=cl200820200721-1900
# Thu, 30 Jul 2020 22:53:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends unzip     && rm -rf /var/lib/apt/lists/*     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default
# Thu, 30 Jul 2020 22:53:47 GMT
ENV LIBERTY_VERSION=2020.8.0_0
# Thu, 30 Jul 2020 22:54:03 GMT
RUN LIBERTY_URL=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 3 | sed -n 's/\s*webProfile7:\s//p' | tr -d '\r')      && echo $LIBERTY_URL     && wget -q $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp-beta.zip     && unzip -q /tmp/wlp-beta.zip -d /opt/ibm     && rm /tmp/wlp-beta.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp
# Thu, 30 Jul 2020 22:54:05 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:54:05 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:54:06 GMT
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:54:06 GMT
COPY file:f1015ab5ca098f3a04cde2e721a2aa35a1ebb2e9f5eb01d378eb2264cff9a268 in /opt/ibm/wlp/usr/servers/defaultServer/ 
# Thu, 30 Jul 2020 22:54:07 GMT
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:54:07 GMT
USER 1001
# Thu, 30 Jul 2020 22:54:07 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:54:08 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd0616bcf913010a9627813bfed05e4594b3bd2193c89b31d87a427b4984c45`  
		Last Modified: Thu, 30 Jul 2020 22:59:19 GMT  
		Size: 371.9 KB (371878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57970ee23f38cd089524d10e29d323fb03722c6f68b396121ec02f9b47fd9e4d`  
		Last Modified: Thu, 30 Jul 2020 22:59:24 GMT  
		Size: 100.2 MB (100243846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ab5d86f858aaecf20b15b9aa5918d45d32705ccc0b7428cf466461b6b98f9c`  
		Last Modified: Thu, 30 Jul 2020 22:59:18 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2585c1cfcc8b09eaddb30f9cb5f3813b2b7c68748bdbc911952382136d6e14`  
		Last Modified: Thu, 30 Jul 2020 22:59:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae8a780287a43df1f86f6556bef1b2c94eeb60a7519799bb6a35200c1261c5`  
		Last Modified: Thu, 30 Jul 2020 22:59:19 GMT  
		Size: 1.0 KB (1009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:full`

```console
$ docker pull websphere-liberty@sha256:d43e16e8b35b7226698ef2a328018590564c7292c2be971736f71cdd80792cff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:7db591017b3034538a4c0a96274c5be8027321a81958a9171fe57830c4256caf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396132731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfac0cead3d5f6a8ddf105f86acb9067db2012820b0e1faab09c75e55c94c0c4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:53:14 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:53:14 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:53:15 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:53:25 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:53:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:53:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:53:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:53:30 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:53:46 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:53:46 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:53:46 GMT
USER 1001
# Thu, 30 Jul 2020 22:53:47 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:53:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:53:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:53:54 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:53:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:57:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:57:18 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:58:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d81557d9cc6e59acdc25818a46ac945a48485de139eafe8bb30d05354c5663`  
		Last Modified: Thu, 30 Jul 2020 22:59:14 GMT  
		Size: 13.8 MB (13783714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c62bea2d5f1dbecdfea3cfc3ce8dbb0110306e3253a8aee0bac9727927313bd`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75f940f290330a5ec1d3cb97465332a686e2cfb2043698beeb50af24401e2f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.0 KB (9036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8160cd73a82cb75737ff72bb9e5c2cd4a33bc6719cee4a7f1fc72020fd04ec3f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aae8a6f675ecb553ec4c147a415cfedec03e426d59cad79e1901c7cfa1ee41f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 57.3 KB (57343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acbfae58da0e5272fe9e835ebc7f7038640b3db4287da710ee115f49638df96`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.9 KB (9922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37146a46875370b17578a3e68e6bee5257a810ff04066dfac7b4aab9ec66e205`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 5.7 MB (5653146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7cd1a65c8aa35cbc26ee655a792d4bb7f90799023cda6475cc1e77c600e2df`  
		Last Modified: Thu, 30 Jul 2020 22:59:33 GMT  
		Size: 194.8 MB (194771855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926165a268d82024ede2797d8b3921a0903ff61c73de3897b7781e103dd99b4e`  
		Last Modified: Thu, 30 Jul 2020 22:59:17 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f9345f344474ecf0956527041c1c5ceed467816820d14c0ab0438ddf61177c`  
		Last Modified: Thu, 30 Jul 2020 22:59:21 GMT  
		Size: 21.8 MB (21813225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; 386

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

### `websphere-liberty:full` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:430f15ad7d64a12f0756f0990bfaee07c072040d71fa611dfd1c25a0deafc42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.3 MB (404303249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ad7606f69c19e69a11b7db356fc1cdf166271143f41d40e77a6d18ba18cf55`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:34:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:34:43 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:34:50 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:34:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:35:33 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:35:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:35:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:35:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:36:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:36:08 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:36:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:36:11 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:36:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:36:59 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:37:03 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:37:06 GMT
USER 1001
# Thu, 30 Jul 2020 22:37:08 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:37:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:37:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:37:47 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:38:00 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:42:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:42:45 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:44:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a068ff0da5b15b15ba95339c011442006ce76ce4486a0df1d1253334750430dc`  
		Last Modified: Thu, 30 Jul 2020 22:45:17 GMT  
		Size: 13.8 MB (13784331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d084fee2f71c0a9c627cae934b97e3d7fd0264b883e2e0577d504ac127f6`  
		Last Modified: Thu, 30 Jul 2020 22:45:13 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4a673c35c7b2ee99c2cc4b4fe32b90e224e208e59254216feaa12a7e8f5bf9`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d9962284e436c4de6df54d7b161a85de69aaa4abc0aa94d29e9dadd428032`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3984e000819787c569ebfb279b6e64feff4f4bd0e22e092d6712dd81b5a6e5`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 57.3 KB (57338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425b10ab6483f5b2d6caf62c9223d3d9ae41255ece708dabc9e39a85fe005f9b`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 10.0 KB (10029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7002fa317a4748e3779742ee40bf208b1150736b7e138a65cc50931c862be67`  
		Last Modified: Thu, 30 Jul 2020 22:45:12 GMT  
		Size: 5.1 MB (5148853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7781f340ee342e4e325d6d6620b79a479948c31a7c9720c8aa0d661cd93776dd`  
		Last Modified: Thu, 30 Jul 2020 22:45:43 GMT  
		Size: 194.3 MB (194285373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa37cf123a052f161a723ef3bb27d8ced6bcc4ae679c9dd121267b853ed8840`  
		Last Modified: Thu, 30 Jul 2020 22:45:25 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94826eb4daee4759e15bfffe1978f4357f6a806be74e2a9b54fe290dfcf6cc5`  
		Last Modified: Thu, 30 Jul 2020 22:45:29 GMT  
		Size: 18.7 MB (18651233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:fb94705fc4dcd69a6aed5e9bbd5cc77b07550af31a08026c34b8c8219a858e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.6 MB (391608162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60602e1245dd6f8c53834774155a20632c21c1e39c8e0b8a0c7a35e28da5779f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:54:13 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:54:13 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:54:14 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:54:22 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:54:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:54:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:54:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:24 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:54:25 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:54:32 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:54:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:54:33 GMT
USER 1001
# Thu, 30 Jul 2020 22:54:33 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:54:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:54:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:54:40 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:54:40 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:58:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:58:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:58:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8346e72ed70efe0c0afcb3f476069fa0dd103c6e8eaca1a7dc766312488a38f`  
		Last Modified: Thu, 30 Jul 2020 22:59:32 GMT  
		Size: 13.8 MB (13783695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188b9215c9f1f5e014b767c988af83915874b6256073df6b9d4d35f52a44859`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83fae6751a1269cdd545d2c07a3b1b0ffe8cc135724d3a4fce7525a834c0b5a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 9.1 KB (9064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850405cc03be76d38215a47e3ffa25cd8b5972d9068d3f9cbf57f70be3922a9`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5937f0b9af37ba1e917a21ca9e650eed812ed9e0e399d1a8196f4e53dad97a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 57.3 KB (57346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be67f780d9694352da879fd5c0a3331267cf90e7ab2c311e10e6a6d9ac4824a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 10.0 KB (10016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c85c5c2e67f168f813579e6d9c843a3ecc0df1092afa9a14ad1d57dd08c21c`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 5.7 MB (5665376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f578b4f9b115993a3432a3b58d2b8d36878374169ee38d8061b01ff03168cd1`  
		Last Modified: Thu, 30 Jul 2020 22:59:46 GMT  
		Size: 194.8 MB (194805693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d174a918ac23ee6556cb2fcefce022416c92ce3439d40ff6efc64f2ef430b30`  
		Last Modified: Thu, 30 Jul 2020 22:59:36 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4dd1686e619f35bfcffb45f5754ee58834a05edf5595d594c80cca0f27b2265`  
		Last Modified: Thu, 30 Jul 2020 22:59:39 GMT  
		Size: 21.6 MB (21594611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:kernel`

```console
$ docker pull websphere-liberty@sha256:70a328cb0255f1597a899ab1618a23b2b80891b74c25ee5b3b3cde8aaba000f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:0482d46102f07ec8569774e4b397b6185f0fefbe4c240820d2e0b00fc1899e26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.5 MB (179546698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d2ea8a2db41d6dd356c634d44facd87f775678aa6acb5737e07008f6aacbbe`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:53:14 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:53:14 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:53:15 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:53:25 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:53:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:53:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:53:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:53:30 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:53:46 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:53:46 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:53:46 GMT
USER 1001
# Thu, 30 Jul 2020 22:53:47 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:53:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:53:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d81557d9cc6e59acdc25818a46ac945a48485de139eafe8bb30d05354c5663`  
		Last Modified: Thu, 30 Jul 2020 22:59:14 GMT  
		Size: 13.8 MB (13783714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c62bea2d5f1dbecdfea3cfc3ce8dbb0110306e3253a8aee0bac9727927313bd`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75f940f290330a5ec1d3cb97465332a686e2cfb2043698beeb50af24401e2f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.0 KB (9036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8160cd73a82cb75737ff72bb9e5c2cd4a33bc6719cee4a7f1fc72020fd04ec3f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aae8a6f675ecb553ec4c147a415cfedec03e426d59cad79e1901c7cfa1ee41f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 57.3 KB (57343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acbfae58da0e5272fe9e835ebc7f7038640b3db4287da710ee115f49638df96`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.9 KB (9922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37146a46875370b17578a3e68e6bee5257a810ff04066dfac7b4aab9ec66e205`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 5.7 MB (5653146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; 386

```console
$ docker pull websphere-liberty@sha256:21c2835a021b91c09268f12dc8f3c61f590c1b34d7669aeacf3792d83a7ef016
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.6 MB (162573580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e89243446a76e85ea4bf274dd0ad9e6fd0e763e50ced541577b62bee7dfcb74`
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

### `websphere-liberty:kernel` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:e0f5dd1bebce3bc4b563b49c9cde2cbcc25436a89dfb08aa9b139b43f6f5c7b8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191365694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8954cf9046bbe4e4792fde5bb6fcfef148c350b0c3e5fddf209687568cf698`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:34:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:34:43 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:34:50 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:34:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:35:33 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:35:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:35:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:35:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:36:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:36:08 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:36:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:36:11 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:36:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:36:59 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:37:03 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:37:06 GMT
USER 1001
# Thu, 30 Jul 2020 22:37:08 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:37:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:37:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a068ff0da5b15b15ba95339c011442006ce76ce4486a0df1d1253334750430dc`  
		Last Modified: Thu, 30 Jul 2020 22:45:17 GMT  
		Size: 13.8 MB (13784331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d084fee2f71c0a9c627cae934b97e3d7fd0264b883e2e0577d504ac127f6`  
		Last Modified: Thu, 30 Jul 2020 22:45:13 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4a673c35c7b2ee99c2cc4b4fe32b90e224e208e59254216feaa12a7e8f5bf9`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d9962284e436c4de6df54d7b161a85de69aaa4abc0aa94d29e9dadd428032`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3984e000819787c569ebfb279b6e64feff4f4bd0e22e092d6712dd81b5a6e5`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 57.3 KB (57338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425b10ab6483f5b2d6caf62c9223d3d9ae41255ece708dabc9e39a85fe005f9b`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 10.0 KB (10029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7002fa317a4748e3779742ee40bf208b1150736b7e138a65cc50931c862be67`  
		Last Modified: Thu, 30 Jul 2020 22:45:12 GMT  
		Size: 5.1 MB (5148853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:f75f7ecfb79b65f65a4bf85e89156859511db509d8ad0a959120cdb769aecaf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.2 MB (175206909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0489e34c5bf4ccbc796c2f9a9ce1c15583ea96d38ae63d4a5a1ddb26ad028a8c`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:54:13 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:54:13 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:54:14 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:54:22 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:54:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:54:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:54:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:24 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:54:25 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:54:32 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:54:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:54:33 GMT
USER 1001
# Thu, 30 Jul 2020 22:54:33 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:54:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:54:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8346e72ed70efe0c0afcb3f476069fa0dd103c6e8eaca1a7dc766312488a38f`  
		Last Modified: Thu, 30 Jul 2020 22:59:32 GMT  
		Size: 13.8 MB (13783695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188b9215c9f1f5e014b767c988af83915874b6256073df6b9d4d35f52a44859`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83fae6751a1269cdd545d2c07a3b1b0ffe8cc135724d3a4fce7525a834c0b5a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 9.1 KB (9064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850405cc03be76d38215a47e3ffa25cd8b5972d9068d3f9cbf57f70be3922a9`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5937f0b9af37ba1e917a21ca9e650eed812ed9e0e399d1a8196f4e53dad97a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 57.3 KB (57346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be67f780d9694352da879fd5c0a3331267cf90e7ab2c311e10e6a6d9ac4824a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 10.0 KB (10016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c85c5c2e67f168f813579e6d9c843a3ecc0df1092afa9a14ad1d57dd08c21c`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 5.7 MB (5665376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `websphere-liberty:latest`

```console
$ docker pull websphere-liberty@sha256:d43e16e8b35b7226698ef2a328018590564c7292c2be971736f71cdd80792cff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:latest` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:7db591017b3034538a4c0a96274c5be8027321a81958a9171fe57830c4256caf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396132731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfac0cead3d5f6a8ddf105f86acb9067db2012820b0e1faab09c75e55c94c0c4`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 20:06:05 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 20:06:05 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:14 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:53:14 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:53:14 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:53:15 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:53:25 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:53:26 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:53:26 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:53:26 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:53:29 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:53:29 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:53:30 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:53:46 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:53:46 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:53:46 GMT
USER 1001
# Thu, 30 Jul 2020 22:53:47 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:53:47 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:53:47 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:53:54 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:53:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:57:17 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:57:18 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:58:14 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d81557d9cc6e59acdc25818a46ac945a48485de139eafe8bb30d05354c5663`  
		Last Modified: Thu, 30 Jul 2020 22:59:14 GMT  
		Size: 13.8 MB (13783714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c62bea2d5f1dbecdfea3cfc3ce8dbb0110306e3253a8aee0bac9727927313bd`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f75f940f290330a5ec1d3cb97465332a686e2cfb2043698beeb50af24401e2f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.0 KB (9036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8160cd73a82cb75737ff72bb9e5c2cd4a33bc6719cee4a7f1fc72020fd04ec3f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aae8a6f675ecb553ec4c147a415cfedec03e426d59cad79e1901c7cfa1ee41f`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 57.3 KB (57343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acbfae58da0e5272fe9e835ebc7f7038640b3db4287da710ee115f49638df96`  
		Last Modified: Thu, 30 Jul 2020 22:59:11 GMT  
		Size: 9.9 KB (9922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37146a46875370b17578a3e68e6bee5257a810ff04066dfac7b4aab9ec66e205`  
		Last Modified: Thu, 30 Jul 2020 22:59:12 GMT  
		Size: 5.7 MB (5653146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7cd1a65c8aa35cbc26ee655a792d4bb7f90799023cda6475cc1e77c600e2df`  
		Last Modified: Thu, 30 Jul 2020 22:59:33 GMT  
		Size: 194.8 MB (194771855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926165a268d82024ede2797d8b3921a0903ff61c73de3897b7781e103dd99b4e`  
		Last Modified: Thu, 30 Jul 2020 22:59:17 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f9345f344474ecf0956527041c1c5ceed467816820d14c0ab0438ddf61177c`  
		Last Modified: Thu, 30 Jul 2020 22:59:21 GMT  
		Size: 21.8 MB (21813225 bytes)  
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
$ docker pull websphere-liberty@sha256:430f15ad7d64a12f0756f0990bfaee07c072040d71fa611dfd1c25a0deafc42a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.3 MB (404303249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ad7606f69c19e69a11b7db356fc1cdf166271143f41d40e77a6d18ba18cf55`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 23:43:31 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 23:43:40 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:34:35 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:34:43 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:34:50 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:34:54 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:35:33 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:35:37 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:35:45 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:35:52 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:36:06 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:36:08 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:36:09 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:36:11 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:36:31 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:36:59 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:37:03 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:37:06 GMT
USER 1001
# Thu, 30 Jul 2020 22:37:08 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:37:15 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:37:24 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:37:47 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:38:00 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:42:38 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:42:45 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:44:01 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a068ff0da5b15b15ba95339c011442006ce76ce4486a0df1d1253334750430dc`  
		Last Modified: Thu, 30 Jul 2020 22:45:17 GMT  
		Size: 13.8 MB (13784331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d084fee2f71c0a9c627cae934b97e3d7fd0264b883e2e0577d504ac127f6`  
		Last Modified: Thu, 30 Jul 2020 22:45:13 GMT  
		Size: 697.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4a673c35c7b2ee99c2cc4b4fe32b90e224e208e59254216feaa12a7e8f5bf9`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 9.1 KB (9063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16d9962284e436c4de6df54d7b161a85de69aaa4abc0aa94d29e9dadd428032`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3984e000819787c569ebfb279b6e64feff4f4bd0e22e092d6712dd81b5a6e5`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 57.3 KB (57338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425b10ab6483f5b2d6caf62c9223d3d9ae41255ece708dabc9e39a85fe005f9b`  
		Last Modified: Thu, 30 Jul 2020 22:45:11 GMT  
		Size: 10.0 KB (10029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7002fa317a4748e3779742ee40bf208b1150736b7e138a65cc50931c862be67`  
		Last Modified: Thu, 30 Jul 2020 22:45:12 GMT  
		Size: 5.1 MB (5148853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7781f340ee342e4e325d6d6620b79a479948c31a7c9720c8aa0d661cd93776dd`  
		Last Modified: Thu, 30 Jul 2020 22:45:43 GMT  
		Size: 194.3 MB (194285373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa37cf123a052f161a723ef3bb27d8ced6bcc4ae679c9dd121267b853ed8840`  
		Last Modified: Thu, 30 Jul 2020 22:45:25 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94826eb4daee4759e15bfffe1978f4357f6a806be74e2a9b54fe290dfcf6cc5`  
		Last Modified: Thu, 30 Jul 2020 22:45:29 GMT  
		Size: 18.7 MB (18651233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:latest` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:fb94705fc4dcd69a6aed5e9bbd5cc77b07550af31a08026c34b8c8219a858e4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.6 MB (391608162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60602e1245dd6f8c53834774155a20632c21c1e39c8e0b8a0c7a35e28da5779f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Fri, 24 Jul 2020 16:52:02 GMT
ARG VERBOSE=false
# Fri, 24 Jul 2020 16:52:03 GMT
ARG OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:13 GMT
LABEL org.opencontainers.image.authors=Arthur De Magalhaes, Chris Potter org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=20.0.0.8 org.opencontainers.image.revision=cl200820200721-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM's Java and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 30 Jul 2020 22:54:13 GMT
ENV LIBERTY_VERSION=20.0.0_08
# Thu, 30 Jul 2020 22:54:13 GMT
ARG LIBERTY_URL
# Thu, 30 Jul 2020 22:54:14 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 30 Jul 2020 22:54:22 GMT
# ARGS: DOWNLOAD_OPTIONS= OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 30 Jul 2020 22:54:22 GMT
ENV PATH=/opt/ibm/wlp/bin:/opt/ibm/helpers/build:/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jul 2020 22:54:23 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=20.0.0.8 BuildLabel=cl200820200721-1900
# Thu, 30 Jul 2020 22:54:23 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 30 Jul 2020 22:54:24 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:eea9bd687cda20807296939d3f98c70b1d48a11ffe1e23ee8f0c373a62cce55b in /opt/ibm/helpers/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 30 Jul 2020 22:54:24 GMT
COPY dir:43d57c83c75dd6d28e2edcce4973d45cc52cb0321988aa3589fe22dc022f86e3 in /licenses/ 
# Thu, 30 Jul 2020 22:54:25 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 30 Jul 2020 22:54:32 GMT
# ARGS: DOWNLOAD_OPTIONS= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 30 Jul 2020 22:54:33 GMT
ENV RANDFILE=/tmp/.rnd IBM_JAVA_OPTIONS=-Xshareclasses:name=liberty,nonfatal,cacheDir=/output/.classCache/ -XX:+UseContainerSupport
# Thu, 30 Jul 2020 22:54:33 GMT
USER 1001
# Thu, 30 Jul 2020 22:54:33 GMT
EXPOSE 9080 9443
# Thu, 30 Jul 2020 22:54:33 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 30 Jul 2020 22:54:34 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Thu, 30 Jul 2020 22:54:40 GMT
ARG VERBOSE=false
# Thu, 30 Jul 2020 22:54:40 GMT
ARG REPOSITORIES_PROPERTIES=
# Thu, 30 Jul 2020 22:58:03 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && chmod -R g+rwx /opt/ibm/wlp/output/*
# Thu, 30 Jul 2020 22:58:07 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Thu, 30 Jul 2020 22:58:31 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8346e72ed70efe0c0afcb3f476069fa0dd103c6e8eaca1a7dc766312488a38f`  
		Last Modified: Thu, 30 Jul 2020 22:59:32 GMT  
		Size: 13.8 MB (13783695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188b9215c9f1f5e014b767c988af83915874b6256073df6b9d4d35f52a44859`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 695.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83fae6751a1269cdd545d2c07a3b1b0ffe8cc135724d3a4fce7525a834c0b5a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 9.1 KB (9064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850405cc03be76d38215a47e3ffa25cd8b5972d9068d3f9cbf57f70be3922a9`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5937f0b9af37ba1e917a21ca9e650eed812ed9e0e399d1a8196f4e53dad97a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 57.3 KB (57346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be67f780d9694352da879fd5c0a3331267cf90e7ab2c311e10e6a6d9ac4824a`  
		Last Modified: Thu, 30 Jul 2020 22:59:29 GMT  
		Size: 10.0 KB (10016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c85c5c2e67f168f813579e6d9c843a3ecc0df1092afa9a14ad1d57dd08c21c`  
		Last Modified: Thu, 30 Jul 2020 22:59:30 GMT  
		Size: 5.7 MB (5665376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f578b4f9b115993a3432a3b58d2b8d36878374169ee38d8061b01ff03168cd1`  
		Last Modified: Thu, 30 Jul 2020 22:59:46 GMT  
		Size: 194.8 MB (194805693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d174a918ac23ee6556cb2fcefce022416c92ce3439d40ff6efc64f2ef430b30`  
		Last Modified: Thu, 30 Jul 2020 22:59:36 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4dd1686e619f35bfcffb45f5754ee58834a05edf5595d594c80cca0f27b2265`  
		Last Modified: Thu, 30 Jul 2020 22:59:39 GMT  
		Size: 21.6 MB (21594611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
