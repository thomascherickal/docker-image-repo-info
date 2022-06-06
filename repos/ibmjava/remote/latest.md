## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:150a4e3a30002f3ebe86d7092536b2a8289d313591719a828e98684f764e10f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:latest` - linux; amd64

```console
$ docker pull ibmjava@sha256:27dc49824bcdf6143fd4712c6000a0a9fdef7b5e9ff87e24385091ebb0a94f8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.7 MB (158733401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68b65c236acfdd63bae336acd425df5edaa03c6e666ad55da155de1ad38f9d8f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:51 GMT
ADD file:f657a56a18426c3a88d620a7024e7b91424d926e7b47faa6a97c2369c4c4a228 in / 
# Fri, 29 Apr 2022 23:20:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:06:17 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 30 Apr 2022 01:06:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 17:02:18 GMT
ENV JAVA_VERSION=8.0.7.10
# Wed, 01 Jun 2022 17:02:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 01 Jun 2022 17:02:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:40dd5be53814ae70b2898558673b7ea18d58bf7ab3433560b9ce3cb76d9ff0b1`  
		Last Modified: Fri, 29 Apr 2022 23:22:07 GMT  
		Size: 26.7 MB (26709108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9274cc4ee93edf7c6c542860e9243251f72535f23aa9365dc6f25072d40216`  
		Last Modified: Sat, 30 Apr 2022 01:08:49 GMT  
		Size: 3.0 MB (2959981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464f0bff1557505e412095ed68ad5a6efb9717629c261825ca0dfec69f0049c7`  
		Last Modified: Wed, 01 Jun 2022 17:04:42 GMT  
		Size: 129.1 MB (129064312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; 386

```console
$ docker pull ibmjava@sha256:f0c2ef55db1c4606c537984b8485e341c012ef55f1aa811562ff83c2e46fbb37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147459176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85344acb4dd95b978f4ba5a1b60ae4121b9f3efa8fdf5ae3b3c282380b02552f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 21:18:54 GMT
ADD file:c1118975f50d6835777043d4b807b4fcf30db0151d1e7659e077e9e33c4ea7c7 in / 
# Mon, 06 Jun 2022 21:18:54 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 21:52:30 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 06 Jun 2022 21:52:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 21:52:37 GMT
ENV JAVA_VERSION=8.0.7.10
# Mon, 06 Jun 2022 21:53:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 06 Jun 2022 21:53:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1408ae6e2634d0ef0a2f110363deef0fdf35ee2958852f9d20b92b57495a9fb7`  
		Last Modified: Mon, 06 Jun 2022 21:19:41 GMT  
		Size: 27.2 MB (27165461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2544d5d24f04fcdb404016e3858b5878b2ee1182436bb2acb9f0b694ad952bb2`  
		Last Modified: Mon, 06 Jun 2022 21:55:15 GMT  
		Size: 3.0 MB (2989000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d9bd7420bc1015ca99571ee05ed9b3d26880c5dad4e407d356d52c49b769b9`  
		Last Modified: Mon, 06 Jun 2022 21:55:23 GMT  
		Size: 117.3 MB (117304715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:72eaf310f5d444ad815b47cd7fc2f8b5948c021b2ddb8a3132d5f59dad2ba6e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.1 MB (162108607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6c780dde9bf6f10844a02824451b05b0cf48575c824bcb9df8cad898df9415`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:00 GMT
ADD file:2d91cfcbab5facf9c027064efd477cfde81eca0c1a62c6611ac694bafb94d817 in / 
# Fri, 29 Apr 2022 23:22:04 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:49:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 30 Apr 2022 01:50:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 18:17:09 GMT
ENV JAVA_VERSION=8.0.7.10
# Wed, 01 Jun 2022 18:18:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 01 Jun 2022 18:18:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:c70b79613e1f9e69f0d6473fa0b3f8b10d376e24350617c381ed64978f4bae97`  
		Last Modified: Fri, 29 Apr 2022 23:24:58 GMT  
		Size: 30.4 MB (30443183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b9fc7dc4c2bad9d9f7db0ffd5b499212f90be1d458552dba4bd7e526ede046`  
		Last Modified: Sat, 30 Apr 2022 01:54:24 GMT  
		Size: 3.1 MB (3082255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ff7a5c271ccdc1d007ed16e12fb41d0725701884213399a686c9417d433a53`  
		Last Modified: Wed, 01 Jun 2022 18:21:30 GMT  
		Size: 128.6 MB (128583169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; s390x

```console
$ docker pull ibmjava@sha256:4bef8d9620030eb1f27fe6d661e8957db02d9916ac6c7b00b4b39812065dbe24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.1 MB (154119232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c7b61596d2cccb027bd44953e6d808da2d48c95a1857251054e1a3286ed3c89`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:50 GMT
ADD file:9b5ddd45fc485b5c5ea3d28339d1768fa5d8f60059022a971897d51d94ad5847 in / 
# Fri, 29 Apr 2022 22:49:54 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:15 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 29 Apr 2022 23:27:21 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Jun 2022 15:41:55 GMT
ENV JAVA_VERSION=8.0.7.10
# Wed, 01 Jun 2022 15:42:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='5d779014943fa5957ad5dbf2230e99d6a4e1cdc4e8d906414700309a53716a4f';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='607414268c0e2994f21b9c031a81e515286b4689ce283f03a12cc1a5f956fdd3';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='9f1f5b5ae2cf7ecfef9b3a8871e721724cb8edd50b671c557881d5479ecdf5cf';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='1a9d7b060670ee27f8be95e8b781f5c85b4228ae4fe1b33f1daddb5d2e56c926';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c609d711ba6ba2857faa285bb6df225df31d22a387f0857dc08976d0f65e7ba7';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 01 Jun 2022 15:43:05 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:6a3a8e27eadcc5a6367050ff4089b3a282bdd954a86e38bb735c31a7567ad66a`  
		Last Modified: Wed, 01 Jun 2022 15:46:20 GMT  
		Size: 126.1 MB (126076388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
