## `maven:3-ibmjava`

```console
$ docker pull maven@sha256:eef84d476a65d8ef6010cb0b5390cea57d919143440695444e44faf4b19e1b42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-ibmjava` - linux; amd64

```console
$ docker pull maven@sha256:6fef00ad2ad165edaf07559eb4dc18ab4e6a6f3c867b006faaa54ee802e847e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.2 MB (214173248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3574090f569c34be8e6fcfbe6166659fffa52a5eb344121f940084bb6563dacc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:57:15 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 16 Jun 2023 02:57:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 30 Jun 2023 23:23:48 GMT
ENV JAVA_VERSION=8.0.8.6
# Fri, 30 Jun 2023 23:26:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bd95ba315fa0752be3a18fd67c0dbda568313484f21420999766bc46c9af9191';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e159747a1fe64a03a24994887c8e4ab3aea06072f3a2ed99c3db31cec0c224de';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7385da0c5ffde5b81f4830b95aa352db2a89b8380ccef25dcd77fdf5b0af3488';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='096edb7671f217d64ec9a6cf44b4d0e7f56184da1aa32e8d84eebe36c02c80d9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 30 Jun 2023 23:26:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1aab967c9f4d601afc5e8b2023fa6a57cdb9f402102cbf9e941ffab60ec77b`  
		Last Modified: Fri, 16 Jun 2023 03:01:13 GMT  
		Size: 1.5 MB (1469042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3d721224099caff5dc158dbda3b69a0cbd9ba8ee0a5e406a8072f156dcce2d`  
		Last Modified: Fri, 30 Jun 2023 23:28:05 GMT  
		Size: 171.2 MB (171249265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed76abc5551dc6a4eac3cb6bdf21b7ce8c3c9fd25465727f0f7c9c1d9bc1f271`  
		Last Modified: Fri, 30 Jun 2023 23:45:59 GMT  
		Size: 1.7 MB (1694968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d238eaaaa3b0db5bf41773a681b1e64596e823c4a594c070f67cfbbd3eb218e`  
		Last Modified: Fri, 30 Jun 2023 23:45:59 GMT  
		Size: 9.3 MB (9327561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64109400aa5fd90dc0bc9325db1150652cfa36d45d6d650872d8b1563546365e`  
		Last Modified: Fri, 30 Jun 2023 23:45:58 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b728aa32c32a472c740255e9855e9d744a4a4d38476ba0977d292e6a5983ff4`  
		Last Modified: Fri, 30 Jun 2023 23:45:58 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc53d9504c660e9ea52368726226ca6b01833c118ec0f87fd8f1a8a08abc1d8a`  
		Last Modified: Fri, 30 Jun 2023 23:45:58 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; ppc64le

```console
$ docker pull maven@sha256:73a4e563e2d8c6232473a3007d98c848a47626e3be4dd01c8b4f12202665ca18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219744654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54f28971d0723003a7c649e749e899cd7d880279677de463e0d736dd03b68dc`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:00 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:03 GMT
ADD file:00c4f44b35b683caef54d5b8b0e0b1e68872f45eae17dd7543adaf6c54512447 in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:32:04 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 16 Jun 2023 01:32:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 30 Jun 2023 23:34:08 GMT
ENV JAVA_VERSION=8.0.8.6
# Fri, 30 Jun 2023 23:42:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bd95ba315fa0752be3a18fd67c0dbda568313484f21420999766bc46c9af9191';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e159747a1fe64a03a24994887c8e4ab3aea06072f3a2ed99c3db31cec0c224de';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7385da0c5ffde5b81f4830b95aa352db2a89b8380ccef25dcd77fdf5b0af3488';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='096edb7671f217d64ec9a6cf44b4d0e7f56184da1aa32e8d84eebe36c02c80d9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 30 Jun 2023 23:42:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a02dd69d9a8a1e6f4fc2ccb509fb8efd6014b00ff932a757d23b4b012a2bec49`  
		Last Modified: Fri, 16 Jun 2023 00:44:52 GMT  
		Size: 35.7 MB (35711397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3831c1123275dd4d9043ad21bf2c9fb47b24b3ab61e99547e14106df60427380`  
		Last Modified: Fri, 16 Jun 2023 01:40:42 GMT  
		Size: 1.6 MB (1576481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188381b7aa74564ab295f4dd1a086683de39bb4d01038eebbd6818718b35c366`  
		Last Modified: Fri, 30 Jun 2023 23:43:51 GMT  
		Size: 171.1 MB (171069858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaecec47bd90e7e84f5c6573c27c9cdbbb6812ec1ea9bc7673b32699c11d66b`  
		Last Modified: Sat, 01 Jul 2023 00:01:10 GMT  
		Size: 2.1 MB (2057958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84c94096021b17739585cc55702d33d337496abad334fb2f4a7d42f89e71ad4`  
		Last Modified: Sat, 01 Jul 2023 00:01:10 GMT  
		Size: 9.3 MB (9327585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf58c4b5b16cc3755a8bf7177c224cf1eb010e6a53a4630731450ccd4017e6c`  
		Last Modified: Sat, 01 Jul 2023 00:01:09 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fb79e08bef2a9f16086897c70d844a188023b3e82774af82441b7700378fc5`  
		Last Modified: Sat, 01 Jul 2023 00:01:09 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4068adedeac3f93dcb65604b46607ded8d779058bd6b3dac067714a0f69e118`  
		Last Modified: Sat, 01 Jul 2023 00:01:09 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-ibmjava` - linux; s390x

```console
$ docker pull maven@sha256:687ebd6300a342ee1e8ab88d7b1c54657f0c551a9ff13d72527cb4edd309eaab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202065841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d7ab5d488ffe2d20f12ffa7d3546c92d8652bf1fae4be4ebc5bfcdec3316e7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 17:01:02 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:01:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:01:02 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:01:04 GMT
ADD file:2d2f31ec110b9e7ec21a9d4824a430acdaabf0b4e9c1cdd337438992859b57ae in / 
# Mon, 05 Jun 2023 17:01:04 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 18:25:52 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 16 Jun 2023 18:25:56 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 30 Jun 2023 22:42:14 GMT
ENV JAVA_VERSION=8.0.8.6
# Fri, 30 Jun 2023 22:45:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bd95ba315fa0752be3a18fd67c0dbda568313484f21420999766bc46c9af9191';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e159747a1fe64a03a24994887c8e4ab3aea06072f3a2ed99c3db31cec0c224de';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='7385da0c5ffde5b81f4830b95aa352db2a89b8380ccef25dcd77fdf5b0af3488';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='096edb7671f217d64ec9a6cf44b4d0e7f56184da1aa32e8d84eebe36c02c80d9';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 30 Jun 2023 22:45:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
# Mon, 26 Jun 2023 13:48:06 GMT
RUN apt-get update   && apt-get install -y ca-certificates curl --no-install-recommends   && rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 26 Jun 2023 13:48:06 GMT
ARG MAVEN_VERSION=3.9.3
# Mon, 26 Jun 2023 13:48:06 GMT
ARG USER_HOME_DIR=/root
# Mon, 26 Jun 2023 13:48:06 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 26 Jun 2023 13:48:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 26 Jun 2023 13:48:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:fab1a8aa44b00432834b7776a76fd4149ec2fee2336a3521bd5435428df7edc9`  
		Last Modified: Fri, 16 Jun 2023 18:23:35 GMT  
		Size: 28.6 MB (28644581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1521659225e331fd6923943db586c259687a2b65eab1dbc35fce49da80029f3`  
		Last Modified: Fri, 16 Jun 2023 18:37:39 GMT  
		Size: 1.5 MB (1477026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d8e951ec17c9a3c7a70b7e137b59cb0af83aaba951a0c9ab3aa7b960887c9d`  
		Last Modified: Fri, 30 Jun 2023 22:46:04 GMT  
		Size: 160.9 MB (160926181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96334a10f69ae442c1fa1fa1a33f78eaf6399e5cc5817aef6054bd2c34266d7f`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 1.7 MB (1689117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de29434e8232831a8e5ba41eeaf87c5c5ce360b8cddd82cd78c6bcd997f1be0c`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 9.3 MB (9327563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fcdd404222f0827e76ee9138f41c575d02f61f9f4a2166931c08e1eeeb4db6c`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13dc4a195cb9be88aec9ec30df500993a7e779db70f04119fa6b9223fa09ffc9`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d18a834b545d27b327fe21ca73c76f7facff5fc8c94c41360cf5ad7da0c2c9`  
		Last Modified: Fri, 30 Jun 2023 23:02:40 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
