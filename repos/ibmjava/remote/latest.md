## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:527103288b068853b1418c2a56f3454011e85def542b83814c20edb8188b19fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:latest` - linux; amd64

```console
$ docker pull ibmjava@sha256:2aafe8743b0a13210d02b92a54d69b5f22c0b285c585e5d1541732a258901466
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158152212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f678a84a9decee3c14e90e58a60bbce7ec864db4bdff2cd7087209c5b5ec4f5`
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
# Fri, 13 Aug 2021 17:20:00 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:20:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:20:35 GMT
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
	-	`sha256:fdddaaf62ac54b6731f85929f59ec4241858871fec2bb74017e7bd6c6c22f391`  
		Last Modified: Fri, 13 Aug 2021 17:24:24 GMT  
		Size: 128.5 MB (128484354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; 386

```console
$ docker pull ibmjava@sha256:ac9d91448ec0d033503fe530afbe725ef58999a370bf30ff9ed4f4ef4f59caf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146892775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de791043bd63b794f392dad9016eba7f09256201316e5550ba18af428793bdb1`
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
# Fri, 13 Aug 2021 17:38:56 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:39:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:39:34 GMT
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
	-	`sha256:6aabfa38e7bf7ebd04e4c6326bf775c084edd3f29556d4e8abfd474cc1c4e3bf`  
		Last Modified: Fri, 13 Aug 2021 17:41:42 GMT  
		Size: 116.7 MB (116741792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:48b10f5dddc084bc75fe83703dc2eb14c5c1f06d5b490bd48beab91790122dac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.5 MB (161477660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df94ea5252eb18c45c3276f2742d555735d928c780181f2b2bdd70ce2fcfbd1e`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:55 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 27 Jul 2021 01:56:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Aug 2021 17:16:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:17:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:18:01 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274a7ceecd631ec4df912a3b0382831ab0f4d2796b455732587f4678f12dc8d8`  
		Last Modified: Tue, 27 Jul 2021 02:03:19 GMT  
		Size: 3.1 MB (3083057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a09042d14af73a1633c55245776817263e7af7adf7eb9ff146947d7455c4b8c`  
		Last Modified: Fri, 13 Aug 2021 17:21:24 GMT  
		Size: 128.0 MB (127956645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; s390x

```console
$ docker pull ibmjava@sha256:8cc354ebcf3ea5b4087fad70f94502a3378fd401d0ce8a45bcce3c557aecc04f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153498778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e55c8a7c396f303f22390f3057be11f593ce5f773bc77c9beebf39ee706aca5`
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
# Fri, 13 Aug 2021 17:41:46 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:42:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:42:59 GMT
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
	-	`sha256:5bb0ec02a30a06ad92984623e581cd5e76b3f6669c1bb6bf9f077c20ea242392`  
		Last Modified: Fri, 13 Aug 2021 17:46:57 GMT  
		Size: 125.5 MB (125454904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
