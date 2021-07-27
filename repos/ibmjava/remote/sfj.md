## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:052e610f9730e5013461b6f96f4c65405befe2ce34385ac5e402ad30f3718592
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:90f023e5da42ed70bb47d61a3beec4a21d0eae8f054eef0effb38fb63b5d1294
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94038359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07eb900fb6eb246aae36fc8e58c4f92293c63b39b6d78a54e2881054faeef44d`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:22:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 23:23:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:23:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Mon, 26 Jul 2021 23:24:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 26 Jul 2021 23:24:16 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcc8b59a59a15868e1ba8f0176e149949b7fa1f2c69f90ad72eb7270fdc65f7`  
		Last Modified: Mon, 26 Jul 2021 23:26:50 GMT  
		Size: 3.0 MB (2958819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6ab9fd06ce92824483fb0b99943b89f71296b5c67bc3cc09c44b2550cfdb77`  
		Last Modified: Mon, 26 Jul 2021 23:27:25 GMT  
		Size: 64.4 MB (64370501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:99ec8ba2c4dd49db461777b4b9035c11f02c09aa60fe7176dd87e6e1a0391095
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93888073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35ae669839cbda0de5ae33d4cccb5dde822c053152d064803dac1c8a4098a4ad`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:18:53 GMT
ADD file:45b15f7ce91c2c05cc5e273dee6b36fade4217c3da1d407a6dc8e108f50e2b66 in / 
# Mon, 26 Jul 2021 21:18:53 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:51:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 21:51:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:51:47 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Mon, 26 Jul 2021 21:53:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 26 Jul 2021 21:53:12 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:bc0a67b78038e09ba1732c1a7c63e6c8e924aca7029364acd54d64dd669b151f`  
		Last Modified: Mon, 26 Jul 2021 21:19:48 GMT  
		Size: 27.2 MB (27162925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3e868994170abe61785da91631677200dcc7cec9fc1feeb71f3c5aaa31d6cf`  
		Last Modified: Mon, 26 Jul 2021 21:54:40 GMT  
		Size: 3.0 MB (2988058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fa5a37cef4ca32a8ae5333058ec4e47fb2b6ea51bce38f4fb7ab1614fc1c8`  
		Last Modified: Mon, 26 Jul 2021 21:55:20 GMT  
		Size: 63.7 MB (63737090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:da64748a60ee5be441ede534145404f7ca1fadfbd24567b39eb084ab180d45bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103229086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ca35aa1e774d4c707aa84aa3a41a539a86f2613c1243cc576348b505d4d333`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:55 GMT
ADD file:45b627081344651e16f78f7bbb0da81c1dcc0300835ab0f4bdd6dd93621e461d in / 
# Tue, 13 Jul 2021 23:22:00 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:38:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Jul 2021 04:38:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:38:50 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Wed, 14 Jul 2021 04:41:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 14 Jul 2021 04:41:27 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b4e702a7ed6378fce702bcf7ca7d37185cd6d8387370cd090b9dc4bf5844f47c`  
		Last Modified: Tue, 13 Jul 2021 23:27:12 GMT  
		Size: 30.4 MB (30427987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ab9a4a9b7968cedcece7ccbd278b539ab11dc1c8c1b32042f293b4152f52fd`  
		Last Modified: Wed, 14 Jul 2021 04:46:40 GMT  
		Size: 3.1 MB (3082897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63e575ef18593a4591a7b17be251c5c1b49fd5956290149fc58433dffce5f9f`  
		Last Modified: Wed, 14 Jul 2021 04:47:23 GMT  
		Size: 69.7 MB (69718202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:9087857c6317b6785a26be21b3b561dad88a50d30f861568ee65517bf16c7d9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93512057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdcbaf6b06cf867069ced94efea87a2fa2add0459545fdc2c7b102c7a4dd4860`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:03 GMT
ADD file:edb1df135699bb6ca591e6493c0df55d2030d8990c3e0a3afa80442036f92e16 in / 
# Mon, 26 Jul 2021 20:55:05 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:13:30 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 21:13:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:13:36 GMT
ENV JAVA_VERSION=1.8.0_sr6fp31
# Mon, 26 Jul 2021 21:14:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='459e3c990073af4ccbc7b774b94e495c9a1ab93884fc102b9078450afde345e2';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='b750f58b7623eb184602172122040128d534e3442e2b299670124f5be91cd0db';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='81a3e97371ce2fc85e2e07ad1498c9152a81bfe7d57fe074cd29ecc8df120f86';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='8511e455579014b94a9d8fca686b2bd25391c1ff985cad7320206987b8d4178e';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4857271dfb8db4eb910dc14561789439a4777b8fe1c61a57112592398e6b95e';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 26 Jul 2021 21:14:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cb0153f85b121ce88ea3f3bebbb54c31f8547bed022bd201416974cd40c61f59`  
		Last Modified: Mon, 26 Jul 2021 20:56:50 GMT  
		Size: 25.4 MB (25367016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3beff8b50da678c028627d9aa04a27cce09ff57f8baf2b9c79420f9f2e076484`  
		Last Modified: Mon, 26 Jul 2021 21:17:51 GMT  
		Size: 2.7 MB (2676858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d4818c1be589437d3f85c0af425ef87b25973ea67e849b90130b2c92b19f72`  
		Last Modified: Mon, 26 Jul 2021 21:18:20 GMT  
		Size: 65.5 MB (65468183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
