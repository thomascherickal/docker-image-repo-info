## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:b4a8168ccc78684fdd5d08eed85a3dc6d3d9b25fddd001996f0dccc77e9d91d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:879d84e1c423876759041066a6b0a1de60410b21ae869a72d331db95669cf5f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.8 MB (195813330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f2d1c04b7fd94547d66b044126543f9815c39808c53d8a2dd2f24406a813a95`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:46:26 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 22 Apr 2022 02:46:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:46:34 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 22 Apr 2022 02:48:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='9261e658294baf2367802c07b6b6b8208a453556ca4189839661a54bab40f730';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fde521653a0c85e2a7b579f5ea7453a060e38a6e4f6b19134aed0f246d754146';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d8ed3c8a3756f4d4962bbd3219dfee51a43445ce61d5eeb383ac782884c21c7f';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='911de16288399945444e9a33dbb80f363d512c3864cdbeb9124e8d6d8b33769c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='fcaad2566d4ad801eb6334572940d70d13e540f66a39601fd89d2b8c686519d4';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 22 Apr 2022 02:48:25 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62da0fb33f1f956bb5cd7b0cd80748069becbe26b1ad9eada0d99f9f993c53a0`  
		Last Modified: Fri, 22 Apr 2022 02:48:52 GMT  
		Size: 3.0 MB (2960053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56fccdd5b28435130620597512b3707e8304b158498aacf242b037dde085952`  
		Last Modified: Fri, 22 Apr 2022 02:49:42 GMT  
		Size: 166.1 MB (166143394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:944f2d4f28284392569812fdd313932789b88cd51b78fc9dbde29a04d5f598d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.4 MB (184439232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67dd3909fbe525a0198f55dafee1b9f791fb57c0f59d63987355e26cb97a63d9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:53:57 GMT
ADD file:164f0ee7842870b8f94ab2ee8f9151b49e08f461b99fdfa1b7586fa864d4a320 in / 
# Thu, 21 Apr 2022 23:53:57 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:10:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 22 Apr 2022 00:10:27 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:10:28 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 22 Apr 2022 00:12:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='9261e658294baf2367802c07b6b6b8208a453556ca4189839661a54bab40f730';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fde521653a0c85e2a7b579f5ea7453a060e38a6e4f6b19134aed0f246d754146';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d8ed3c8a3756f4d4962bbd3219dfee51a43445ce61d5eeb383ac782884c21c7f';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='911de16288399945444e9a33dbb80f363d512c3864cdbeb9124e8d6d8b33769c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='fcaad2566d4ad801eb6334572940d70d13e540f66a39601fd89d2b8c686519d4';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 22 Apr 2022 00:12:30 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:57fda0d035c311017871931fe2f2a2c241e46b4bc95d2a87dbf533afd8e72668`  
		Last Modified: Tue, 19 Apr 2022 13:11:34 GMT  
		Size: 27.2 MB (27163453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf89379f0f6a5f1815105d3eccdd37714136125bbdae184d2d74ccbe37b346bf`  
		Last Modified: Fri, 22 Apr 2022 00:13:00 GMT  
		Size: 3.0 MB (2988566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3c48e57a1601fb52430f0a6519b0bebde4a421a2b6ed18e30666da0a4ac03e`  
		Last Modified: Fri, 22 Apr 2022 00:14:16 GMT  
		Size: 154.3 MB (154287213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:b42eea89103997abc29a904370c605f2d4cc8458dfb7f84b06e59d1e7b176f46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.3 MB (199318478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea803faa17fb6d60fbbc6da291ff0192efe51e2fdc4c9072fdd00f7798d8c9bf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 10:03:42 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 22 Apr 2022 10:04:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 10:04:36 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 22 Apr 2022 10:08:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='9261e658294baf2367802c07b6b6b8208a453556ca4189839661a54bab40f730';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fde521653a0c85e2a7b579f5ea7453a060e38a6e4f6b19134aed0f246d754146';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d8ed3c8a3756f4d4962bbd3219dfee51a43445ce61d5eeb383ac782884c21c7f';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='911de16288399945444e9a33dbb80f363d512c3864cdbeb9124e8d6d8b33769c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='fcaad2566d4ad801eb6334572940d70d13e540f66a39601fd89d2b8c686519d4';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 22 Apr 2022 10:08:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6335837c025cb29531b7e6877b94805906b0badbb0e9a6b740b8f8790d328f8`  
		Last Modified: Fri, 22 Apr 2022 10:08:53 GMT  
		Size: 3.1 MB (3082171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd53f1f223ee93792766d855dce49384ad7611bc366bb8fd7f8929051e3f0f36`  
		Last Modified: Fri, 22 Apr 2022 10:10:08 GMT  
		Size: 165.8 MB (165794034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:fbb279ad054791016064dbe6d9da74b9425ca1c5f6baa6cb254dec226b2ca315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.4 MB (184354397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb5d71c8ac94a05fce56fd64b68aa5f5ef0a75f9b71e93f4dc1e2112e88f421`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:17 GMT
ADD file:bc2c78cc62a5e94931f8bd76f2fa050b19598c050fc18aa56bbd202826ec784b in / 
# Fri, 22 Apr 2022 00:39:19 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:27:55 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 22 Apr 2022 02:28:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:28:08 GMT
ENV JAVA_VERSION=8.0.7.6
# Fri, 22 Apr 2022 02:31:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='9261e658294baf2367802c07b6b6b8208a453556ca4189839661a54bab40f730';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='fde521653a0c85e2a7b579f5ea7453a060e38a6e4f6b19134aed0f246d754146';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d8ed3c8a3756f4d4962bbd3219dfee51a43445ce61d5eeb383ac782884c21c7f';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='911de16288399945444e9a33dbb80f363d512c3864cdbeb9124e8d6d8b33769c';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='fcaad2566d4ad801eb6334572940d70d13e540f66a39601fd89d2b8c686519d4';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 22 Apr 2022 02:31:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:18c1f746bcbccc4e7599497df0d1d562571c9ecd9effcfb7bee0bbe17d1156b5`  
		Last Modified: Tue, 19 Apr 2022 13:12:34 GMT  
		Size: 25.4 MB (25365079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049f8dbfa40cf590d86076cb08023486dab11d5fe13be63339cfc959ded1f685`  
		Last Modified: Fri, 22 Apr 2022 02:32:27 GMT  
		Size: 2.7 MB (2677005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea34afda7fa538235475581dac5dd882718d2fac5427f2f611611c8c012435c`  
		Last Modified: Fri, 22 Apr 2022 02:33:12 GMT  
		Size: 156.3 MB (156312313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
