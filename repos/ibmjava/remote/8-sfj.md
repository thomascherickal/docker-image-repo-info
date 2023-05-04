## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:0a19f0df3dfa2c1103d9276d89b8e00bc2ef8c151aa708d19e31dfbe0922eb19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:4610cd79cf72c7f4cad8067449f0bbbadfa46328ed89f1d145995fa6e903d91b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101116205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f75b397010a3a9a22cf972997a2d698879d847fd20a501db1b37e2470c5a1f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:44:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 04 May 2023 07:44:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 07:44:59 GMT
ENV JAVA_VERSION=8.0.8.0
# Thu, 04 May 2023 07:46:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='83aa5cbbf7706def8564c57e92afe8cbd76bfe8af58e03f50cbe4154e9feecc7';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cef1f4a87e4dcd97fb8e99f2c2ddcf18c90b7712e3cb65a561ee3e0013052dd8';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='26833e7defe3fc1705d0068f530bbedbe0d9a12c38db8c4bc0837b595827a62e';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='85ab8a83e67d515a48638c58d9e4931ceecafb6f05e2c9f02cf8d9ff4dbfc116';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 04 May 2023 07:46:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bee7fd4007af244555d448c1fb80ceb220cf70203647e0705bbdd49468c13e4`  
		Last Modified: Thu, 04 May 2023 07:48:21 GMT  
		Size: 1.4 MB (1446362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9725cdc575d1be606b75c2147768e8ecfe42ede151181ec16b98ed5fd937642a`  
		Last Modified: Thu, 04 May 2023 07:48:48 GMT  
		Size: 69.2 MB (69239623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:cf4f08e74120a4400c4026243ccf6e872e9bbfe06b434283ff07c9d7e24c4856
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106859299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e138808e0dfed26a9946b1fcc6599c8ebfc1235ddcd489f0c41300d763012dba`
-	Default Command: `["\/bin\/bash"]`

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
# Thu, 04 May 2023 14:14:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='83aa5cbbf7706def8564c57e92afe8cbd76bfe8af58e03f50cbe4154e9feecc7';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cef1f4a87e4dcd97fb8e99f2c2ddcf18c90b7712e3cb65a561ee3e0013052dd8';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='26833e7defe3fc1705d0068f530bbedbe0d9a12c38db8c4bc0837b595827a62e';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='85ab8a83e67d515a48638c58d9e4931ceecafb6f05e2c9f02cf8d9ff4dbfc116';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 04 May 2023 14:14:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:51d94f198033aaabd21ea8ae1a4d6552d4c80b6e06c0ca32e7671ae41967e869`  
		Last Modified: Thu, 04 May 2023 14:19:03 GMT  
		Size: 69.6 MB (69594195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:7032004252ac333b786812a8c64d8978845c368090eaedf7354c1de827e9f807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.2 MB (100170032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57c1f68afc1b0754a6757611e58281f3e492fd77bc9756a51a2d58d028c2a40`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 25 Apr 2023 17:44:52 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:44:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:44:52 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:44:54 GMT
ADD file:bbc65a9f059dc165e33f9a25ffaa40aab1a1f65164198a44394ec3065c82ae21 in / 
# Tue, 25 Apr 2023 17:44:54 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 08:44:44 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 04 May 2023 08:44:58 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:44:58 GMT
ENV JAVA_VERSION=8.0.8.0
# Thu, 04 May 2023 08:46:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='83aa5cbbf7706def8564c57e92afe8cbd76bfe8af58e03f50cbe4154e9feecc7';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='cef1f4a87e4dcd97fb8e99f2c2ddcf18c90b7712e3cb65a561ee3e0013052dd8';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='26833e7defe3fc1705d0068f530bbedbe0d9a12c38db8c4bc0837b595827a62e';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='85ab8a83e67d515a48638c58d9e4931ceecafb6f05e2c9f02cf8d9ff4dbfc116';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 04 May 2023 08:46:42 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:78722793f0008ff8422830a0106f21e8bc168fb9aac12cc99fb223799951759e`  
		Last Modified: Wed, 03 May 2023 22:33:36 GMT  
		Size: 28.6 MB (28647905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9459c54d841fa6f6b374fa6fe3230943f4104eb1c43155f1255ff1c9e735443`  
		Last Modified: Thu, 04 May 2023 08:48:50 GMT  
		Size: 1.5 MB (1452439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e309f4f98bde0b724a481fb7c27d8c745d9eb4c6d56254003e084df449d08b61`  
		Last Modified: Thu, 04 May 2023 08:49:12 GMT  
		Size: 70.1 MB (70069688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
