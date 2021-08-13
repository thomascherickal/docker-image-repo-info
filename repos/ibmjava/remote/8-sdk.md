## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:2d24c47c01d8f716b7c73842cfce1ad933ef84fbc23e2e103b7dab1c29c4df0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:84c3e33d98864ca58fc44df23d6dca924bc5107c7c71eeb8a64120e9612ed035
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.3 MB (195292416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa64c9487f9cff3528366e982ae443cf28bc65cb5b5704428a4e401b287cf054`
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
# Fri, 13 Aug 2021 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:23:02 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:0374f1d5f6233b9fb95ad96e7bb99ee0c7ae1c2b461cd128654daeb782bbadcf`  
		Last Modified: Fri, 13 Aug 2021 17:25:42 GMT  
		Size: 165.6 MB (165624558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:1c85a4a6e9d7736951aebd07e4da71c1276ea16005f4273ffdfa779d53242887
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.9 MB (183913749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad15aa10d7b2ce2c4c385d45ac47f3ba75c34466f279117d073feaeeaae97ded`
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
# Fri, 13 Aug 2021 17:40:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:41:00 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:27ddce3cc7da01f2e4024c23637f51df9816a8461a5836890a1a357d4dcc29e7`  
		Last Modified: Fri, 13 Aug 2021 17:42:36 GMT  
		Size: 153.8 MB (153762766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:78edfa8d8d7bb271f5eb1a16d28985b66d9cff4e137b901d993b3391880d783d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.7 MB (198746250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a221bf55a7579a1d3cc29b8d9d3a06111501e64cebb1b2602677e4dbe3277df`
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
# Fri, 13 Aug 2021 17:20:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:20:30 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:59db1bc347dc1c514aa697f4458ad7bbc9a6937ffde23bc2510f3ce26b137d45`  
		Last Modified: Fri, 13 Aug 2021 17:22:23 GMT  
		Size: 165.2 MB (165225235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:644867454e16b6e5e437003cbaed6cdc6b737249d2fb0c9dc92cedbafa65d9ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183785815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ecb95800254e0fede1dd9f512e80dbed26bc5ce84c9a66c7fad344020dd59cb`
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
# Fri, 13 Aug 2021 17:45:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:45:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
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
	-	`sha256:cddcd70367bff0f8365074de2f2a0345a632ea67ad5908a82e798cd797b1026e`  
		Last Modified: Fri, 13 Aug 2021 17:47:45 GMT  
		Size: 155.7 MB (155741941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
