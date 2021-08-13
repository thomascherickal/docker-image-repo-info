## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:f24f06c83ab8eb2de0c9d4bd397541382ac9b40c4bb4b3bd8d154ce438a59b6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:29adf4205e8d886c6b9a6115198214a3ea2b89997b800c4afb40b30ebc97f14a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94011255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37410eb8b00b522cd8b08d1ac01a1924e70a359fc7a752476e03571d33543cbc`
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
# Fri, 13 Aug 2021 17:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:21:45 GMT
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
	-	`sha256:a68f5756b26d7dfa1cb2ff781f8c57f529a1ffb5b06ae9a68ef73edd6c06db78`  
		Last Modified: Fri, 13 Aug 2021 17:25:04 GMT  
		Size: 64.3 MB (64343397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:ee4b497d4a8245b3d0bc88ef8ed0f22729ba7f41948ecf861de5ba4d9e57ce2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93876510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f2105b024913681fbfbdf250c3163034bcf439294c43e73c75b5371e575d69`
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
# Fri, 13 Aug 2021 17:40:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:40:12 GMT
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
	-	`sha256:dc4fba28c9bbe7c05b28f859e70bbfb79abd34830b4daf9081daaf70143ed922`  
		Last Modified: Fri, 13 Aug 2021 17:42:09 GMT  
		Size: 63.7 MB (63725527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5a537246fff29822f19800ee865e6f334cfc4459f4ca023958a829991082e1b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98047551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c8d49302a905fa41939efa41d1b453a8be938fe9059abbf5ed60d6f0f9ec73`
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
# Fri, 13 Aug 2021 17:19:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:19:07 GMT
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
	-	`sha256:0134f6bf2485178363e983f5bf438d0cd4220d27e69ff6c443944c5162041f2b`  
		Last Modified: Fri, 13 Aug 2021 17:21:52 GMT  
		Size: 64.5 MB (64526536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:9595d0dcbfcc93c89d8d3b3c75ea029617d68f3a818ad95bad466b93de542b72
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93410894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f131717970fca2c3794838d21af9cf10a3ffe072a85291f429ae543a67d311b`
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
# Fri, 13 Aug 2021 17:44:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:44:08 GMT
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
	-	`sha256:336ef6e4b6664be22a3c7c64b399af329dfe84412efc49bb6d22da4e6d835ee1`  
		Last Modified: Fri, 13 Aug 2021 17:47:22 GMT  
		Size: 65.4 MB (65367020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
