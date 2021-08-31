<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ibmjava`

-	[`ibmjava:11`](#ibmjava11)
-	[`ibmjava:11-jdk`](#ibmjava11-jdk)
-	[`ibmjava:8`](#ibmjava8)
-	[`ibmjava:8-jre`](#ibmjava8-jre)
-	[`ibmjava:8-jre-alpine`](#ibmjava8-jre-alpine)
-	[`ibmjava:8-sdk`](#ibmjava8-sdk)
-	[`ibmjava:8-sdk-alpine`](#ibmjava8-sdk-alpine)
-	[`ibmjava:8-sfj`](#ibmjava8-sfj)
-	[`ibmjava:8-sfj-alpine`](#ibmjava8-sfj-alpine)
-	[`ibmjava:jre`](#ibmjavajre)
-	[`ibmjava:jre-alpine`](#ibmjavajre-alpine)
-	[`ibmjava:latest`](#ibmjavalatest)
-	[`ibmjava:sdk`](#ibmjavasdk)
-	[`ibmjava:sdk-alpine`](#ibmjavasdk-alpine)
-	[`ibmjava:sfj`](#ibmjavasfj)
-	[`ibmjava:sfj-alpine`](#ibmjavasfj-alpine)

## `ibmjava:11`

```console
$ docker pull ibmjava@sha256:fe7787f2c7cdaf8f7e2c82d8bfad1b074c3bc42597b3d1230bd3461fa4382289
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:11` - linux; amd64

```console
$ docker pull ibmjava@sha256:edcd11576ae90b9590cede1a458a948feedc9ffa29a3e90379e394fa4c157f7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.0 MB (261983173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0920dece13e1c5456ba284b03c2bef09e96c2d067cb5f676beac98cdce8699`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:25:19 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 23:25:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:25:25 GMT
ENV JAVA_VERSION=11.0.11.0
# Mon, 26 Jul 2021 23:26:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 26 Jul 2021 23:26:22 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e90bfbf448ca7a8efbef5ea0f79e51d6210ea02d851fa6cc46cb7236dbe0142`  
		Last Modified: Mon, 26 Jul 2021 23:28:01 GMT  
		Size: 3.0 MB (3039015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3b3336362c6ccadf136687acbbb3c3cb4cf2cb494f714e80b3a38f6ff54de`  
		Last Modified: Mon, 26 Jul 2021 23:28:18 GMT  
		Size: 230.4 MB (230376214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:8e8a1f9ab13131b25f7eb693bb493becc204a8331ed3cfd18585ba96e6cf9b48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267888974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5def2354e3de88d539b2b794a96ea5d97482834219bd9ae2bb57b5072d00ca`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:00:48 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 27 Jul 2021 02:01:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:01:29 GMT
ENV JAVA_VERSION=11.0.11.0
# Tue, 27 Jul 2021 02:02:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 27 Jul 2021 02:02:44 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669e58f1f347891c9de25b88b61460bc92fe7348cd685a1e338984b18b4c52f9`  
		Last Modified: Tue, 27 Jul 2021 02:04:48 GMT  
		Size: 3.3 MB (3292569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa664c7a8863f0e1fe63d018f9ba22a169c07ef306f73b33ee700e1747f6bcf`  
		Last Modified: Tue, 27 Jul 2021 02:05:14 GMT  
		Size: 231.3 MB (231305978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11` - linux; s390x

```console
$ docker pull ibmjava@sha256:d1f2d06fd52d221ba1ddb6c728e66138b46d109d6e5384ca7d5342d90e22a1de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260808982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f30a02810cb0a4c615c1ceda9cc06556aa515d0f4fb7b86f2808151d897a74a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:04:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:04:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:12 GMT
ENV JAVA_VERSION=11.0.11.0
# Tue, 31 Aug 2021 02:05:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:05:34 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f82a80fc57ecf5920da007b382a89f3cf656ec0dde08098ce0e2f2225b4eeb`  
		Last Modified: Tue, 31 Aug 2021 02:07:09 GMT  
		Size: 2.7 MB (2738594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bf1d16de5ff4a0dd6c6b6224013a29c99d15478790f88662bb5fc25ca1888`  
		Last Modified: Tue, 31 Aug 2021 02:07:25 GMT  
		Size: 230.9 MB (230942918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:11-jdk`

```console
$ docker pull ibmjava@sha256:fe7787f2c7cdaf8f7e2c82d8bfad1b074c3bc42597b3d1230bd3461fa4382289
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:11-jdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:edcd11576ae90b9590cede1a458a948feedc9ffa29a3e90379e394fa4c157f7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.0 MB (261983173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0920dece13e1c5456ba284b03c2bef09e96c2d067cb5f676beac98cdce8699`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:25:19 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 23:25:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:25:25 GMT
ENV JAVA_VERSION=11.0.11.0
# Mon, 26 Jul 2021 23:26:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 26 Jul 2021 23:26:22 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e90bfbf448ca7a8efbef5ea0f79e51d6210ea02d851fa6cc46cb7236dbe0142`  
		Last Modified: Mon, 26 Jul 2021 23:28:01 GMT  
		Size: 3.0 MB (3039015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3b3336362c6ccadf136687acbbb3c3cb4cf2cb494f714e80b3a38f6ff54de`  
		Last Modified: Mon, 26 Jul 2021 23:28:18 GMT  
		Size: 230.4 MB (230376214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11-jdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:8e8a1f9ab13131b25f7eb693bb493becc204a8331ed3cfd18585ba96e6cf9b48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267888974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d5def2354e3de88d539b2b794a96ea5d97482834219bd9ae2bb57b5072d00ca`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:46 GMT
ADD file:68eb628c2202763afa91d554dde9668d8a468fe53fdbd2fe98627a5f91d224b4 in / 
# Mon, 26 Jul 2021 23:12:49 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 02:00:48 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 27 Jul 2021 02:01:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 02:01:29 GMT
ENV JAVA_VERSION=11.0.11.0
# Tue, 27 Jul 2021 02:02:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 27 Jul 2021 02:02:44 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1a396eed835b3b7b4101a9863d174e145ddbb1de1502a63bae726b0f81e7ca93`  
		Last Modified: Mon, 26 Jul 2021 23:15:51 GMT  
		Size: 33.3 MB (33290427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669e58f1f347891c9de25b88b61460bc92fe7348cd685a1e338984b18b4c52f9`  
		Last Modified: Tue, 27 Jul 2021 02:04:48 GMT  
		Size: 3.3 MB (3292569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa664c7a8863f0e1fe63d018f9ba22a169c07ef306f73b33ee700e1747f6bcf`  
		Last Modified: Tue, 27 Jul 2021 02:05:14 GMT  
		Size: 231.3 MB (231305978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11-jdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:d1f2d06fd52d221ba1ddb6c728e66138b46d109d6e5384ca7d5342d90e22a1de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260808982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f30a02810cb0a4c615c1ceda9cc06556aa515d0f4fb7b86f2808151d897a74a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:04:03 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:04:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:12 GMT
ENV JAVA_VERSION=11.0.11.0
# Tue, 31 Aug 2021 02:05:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:05:34 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f82a80fc57ecf5920da007b382a89f3cf656ec0dde08098ce0e2f2225b4eeb`  
		Last Modified: Tue, 31 Aug 2021 02:07:09 GMT  
		Size: 2.7 MB (2738594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bf1d16de5ff4a0dd6c6b6224013a29c99d15478790f88662bb5fc25ca1888`  
		Last Modified: Tue, 31 Aug 2021 02:07:25 GMT  
		Size: 230.9 MB (230942918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8`

```console
$ docker pull ibmjava@sha256:aa343aacfbd44369af12ab12df02156c08fae08daa815b80be5f3378e3708b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8` - linux; amd64

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

### `ibmjava:8` - linux; 386

```console
$ docker pull ibmjava@sha256:12cb93060e43bf01029f9a569064f9d09132cf8398eb69a540ddb319ef6c9c05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146893527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c670c987f24ba1c0e649f68e9119fa9ef6c80fd3c32687240d12382a1d4f85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ac3b57e0c18b9831eb0ebb14ada401a5e901db11b6d8753d5723f78102ce43`  
		Last Modified: Tue, 31 Aug 2021 02:15:17 GMT  
		Size: 116.7 MB (116741702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; ppc64le

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

### `ibmjava:8` - linux; s390x

```console
$ docker pull ibmjava@sha256:4d35b0111b2c2c4f682bb2cd53b038cd1a672bb7e78b5265caa2034431bb8fd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153498870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cb8566ec7de9103e2e99570c5bc526b7c8f42fe477306044a9e76d57ebd31f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:01:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:01:46 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6435164bedc974ae107c60a6dc9d5b881556e450f0e3668b74c16aca050948c`  
		Last Modified: Tue, 31 Aug 2021 02:06:24 GMT  
		Size: 125.5 MB (125454836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre`

```console
$ docker pull ibmjava@sha256:aa343aacfbd44369af12ab12df02156c08fae08daa815b80be5f3378e3708b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-jre` - linux; amd64

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

### `ibmjava:8-jre` - linux; 386

```console
$ docker pull ibmjava@sha256:12cb93060e43bf01029f9a569064f9d09132cf8398eb69a540ddb319ef6c9c05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146893527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c670c987f24ba1c0e649f68e9119fa9ef6c80fd3c32687240d12382a1d4f85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ac3b57e0c18b9831eb0ebb14ada401a5e901db11b6d8753d5723f78102ce43`  
		Last Modified: Tue, 31 Aug 2021 02:15:17 GMT  
		Size: 116.7 MB (116741702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; ppc64le

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

### `ibmjava:8-jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:4d35b0111b2c2c4f682bb2cd53b038cd1a672bb7e78b5265caa2034431bb8fd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153498870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cb8566ec7de9103e2e99570c5bc526b7c8f42fe477306044a9e76d57ebd31f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:01:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:01:46 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6435164bedc974ae107c60a6dc9d5b881556e450f0e3668b74c16aca050948c`  
		Last Modified: Tue, 31 Aug 2021 02:06:24 GMT  
		Size: 125.5 MB (125454836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre-alpine`

```console
$ docker pull ibmjava@sha256:02b16ad98b13fc9969ea4e2614fa3af04dbf6633b26793bd23deb555eb6dad67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `ibmjava:8-jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:6801e44caf5558d2ed761baab9d140ee7498086a8da28cc43635a4f4f8382ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136838020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d49587f14f958efd8dfa8c8a564e8c429f800bccc4c5ddf4e91e00866d3029`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 13 Aug 2021 17:20:42 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:21:14 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 13 Aug 2021 17:21:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b476a99d3ec5840e040ca3a9005a87e4c8d641a7d8652499573143c0b85183`  
		Last Modified: Fri, 13 Aug 2021 17:24:49 GMT  
		Size: 128.5 MB (128497170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:028d4600c8d181990e573a2ca2ffccd41a9b682e4a8b12345da20111b8008d31
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
$ docker pull ibmjava@sha256:ace025ac0b1d1f16e0b29d41e5ae80d1d5c022682aec829ff02bb4097a2d8151
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.9 MB (183914831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85c5cbb67dc051be1f06ff5d099fc9dce9be7589fa0913600f7d328734e59f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:14:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:14:34 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec608b5e34df195cc546df0cd8681f79c50de2626ab34ac88ded088eeeabdd2`  
		Last Modified: Tue, 31 Aug 2021 02:16:19 GMT  
		Size: 153.8 MB (153763006 bytes)  
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
$ docker pull ibmjava@sha256:a3d401d17e1a065486141ea8e10ff5906f071f624d6f8c0ecd9210b90f8c371b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183785846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8898d6467707589d684465f1d1e50f7cc38a64a488874a9c7bdf60dd6454580`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:03:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:03:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b45f85a7fc9d087b774ff2a8b70f276ef9a21d73a4c0cea48624b4c5665625e`  
		Last Modified: Tue, 31 Aug 2021 02:07:01 GMT  
		Size: 155.7 MB (155741812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk-alpine`

```console
$ docker pull ibmjava@sha256:0a9646c8baabc4a8691362b7d360b85152b1a42080f8e24afe278c02c1993baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `ibmjava:8-sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:165f008e14f9a942d8dbf7fe4c890c8cb099d32b05411c577723b4f1b30e8afd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.0 MB (173969276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d2c24491172c646879581a1404932e9621f052535aa8bd2d7892c1557f0d63`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 13 Aug 2021 17:20:42 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:23:47 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 13 Aug 2021 17:23:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e58e1236ecb91a26886efe0e3bc0f9987c5f9c78e9cbbd2a0928c606c22fae`  
		Last Modified: Fri, 13 Aug 2021 17:26:04 GMT  
		Size: 165.6 MB (165628426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:1426b37092f46c54e20d0da0bd6442093d5bc2d844e98725ba945f9ed03c4a60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

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

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:887c9f2ce25e600a5bf4be416955305e4b861c43dc3d3825e0af284c60f6f4bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93877342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:decfb9ce4e6e2e91f7d3f01135f7b771a0d081dc5e4c54e2b8f376c4d3745737`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd587741057be9756d70f8ab18d1125a760b56daa6b8a5cae94927e996a66d25`  
		Last Modified: Tue, 31 Aug 2021 02:15:44 GMT  
		Size: 63.7 MB (63725517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

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

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:81b010776718b38d7480d1921514b907df374deb08b6f9d8d4ee5d2829056489
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93411032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d11a7b7b65fcd918375630840f85095ae607331d52e0e893f5428a9659453f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:02:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:02:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90483140c8323edda00aa1cb79960f1c07e4689eea1184fea844f457a64a536c`  
		Last Modified: Tue, 31 Aug 2021 02:06:41 GMT  
		Size: 65.4 MB (65366998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj-alpine`

```console
$ docker pull ibmjava@sha256:c88f847ef2c5b73f1f6e5f6b9add320b20334f15f45aa01690c55844f4b4bec9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `ibmjava:8-sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:e601114cc10588c8e374928687f3f9cc6dfbcd78f6b13d3adb521c8bd30ccc34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72691363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:965f0c92472e53a0df57f00f440828fbda0a222fdb8e4af567ad95b77b7a893f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 13 Aug 2021 17:20:42 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:22:13 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 13 Aug 2021 17:22:13 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9a1c56b92b631f405f01a45c95e52568be7cee05a479cd3ad4f92bb7b0e420`  
		Last Modified: Fri, 13 Aug 2021 17:25:20 GMT  
		Size: 64.4 MB (64350513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre`

```console
$ docker pull ibmjava@sha256:aa343aacfbd44369af12ab12df02156c08fae08daa815b80be5f3378e3708b5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:jre` - linux; amd64

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

### `ibmjava:jre` - linux; 386

```console
$ docker pull ibmjava@sha256:12cb93060e43bf01029f9a569064f9d09132cf8398eb69a540ddb319ef6c9c05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146893527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c670c987f24ba1c0e649f68e9119fa9ef6c80fd3c32687240d12382a1d4f85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ac3b57e0c18b9831eb0ebb14ada401a5e901db11b6d8753d5723f78102ce43`  
		Last Modified: Tue, 31 Aug 2021 02:15:17 GMT  
		Size: 116.7 MB (116741702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; ppc64le

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

### `ibmjava:jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:4d35b0111b2c2c4f682bb2cd53b038cd1a672bb7e78b5265caa2034431bb8fd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153498870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cb8566ec7de9103e2e99570c5bc526b7c8f42fe477306044a9e76d57ebd31f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:01:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:01:46 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6435164bedc974ae107c60a6dc9d5b881556e450f0e3668b74c16aca050948c`  
		Last Modified: Tue, 31 Aug 2021 02:06:24 GMT  
		Size: 125.5 MB (125454836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre-alpine`

```console
$ docker pull ibmjava@sha256:02b16ad98b13fc9969ea4e2614fa3af04dbf6633b26793bd23deb555eb6dad67
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `ibmjava:jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:6801e44caf5558d2ed761baab9d140ee7498086a8da28cc43635a4f4f8382ce7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136838020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d49587f14f958efd8dfa8c8a564e8c429f800bccc4c5ddf4e91e00866d3029`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 13 Aug 2021 17:20:42 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:21:14 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 13 Aug 2021 17:21:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b476a99d3ec5840e040ca3a9005a87e4c8d641a7d8652499573143c0b85183`  
		Last Modified: Fri, 13 Aug 2021 17:24:49 GMT  
		Size: 128.5 MB (128497170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:aa343aacfbd44369af12ab12df02156c08fae08daa815b80be5f3378e3708b5a
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
$ docker pull ibmjava@sha256:12cb93060e43bf01029f9a569064f9d09132cf8398eb69a540ddb319ef6c9c05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146893527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c670c987f24ba1c0e649f68e9119fa9ef6c80fd3c32687240d12382a1d4f85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:08 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ac3b57e0c18b9831eb0ebb14ada401a5e901db11b6d8753d5723f78102ce43`  
		Last Modified: Tue, 31 Aug 2021 02:15:17 GMT  
		Size: 116.7 MB (116741702 bytes)  
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
$ docker pull ibmjava@sha256:4d35b0111b2c2c4f682bb2cd53b038cd1a672bb7e78b5265caa2034431bb8fd7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153498870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cb8566ec7de9103e2e99570c5bc526b7c8f42fe477306044a9e76d57ebd31f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:01:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7c12c8fb9be1e2db061f24accfdf94644efcf3e2a8c9054e713c2970b03ab174';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='d744258a04be78f4d97210a2c161c27597ec81c47601352fbf2806ec2e65e221';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='216db2e766718bf6c752ef1f453a339c9eabec2a57e9570a56a933d2059761ed';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='ef91c6d29f6387193b86a73ad07f95c3c765b667e45e82486f73a7a7d0d8507c';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='ee70074a97f36a39f655009d69f4e5de17e3ca6c7fedc6f1cefa6dcec9668373';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:01:46 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6435164bedc974ae107c60a6dc9d5b881556e450f0e3668b74c16aca050948c`  
		Last Modified: Tue, 31 Aug 2021 02:06:24 GMT  
		Size: 125.5 MB (125454836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk`

```console
$ docker pull ibmjava@sha256:028d4600c8d181990e573a2ca2ffccd41a9b682e4a8b12345da20111b8008d31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sdk` - linux; amd64

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

### `ibmjava:sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:ace025ac0b1d1f16e0b29d41e5ae80d1d5c022682aec829ff02bb4097a2d8151
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.9 MB (183914831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85c5cbb67dc051be1f06ff5d099fc9dce9be7589fa0913600f7d328734e59f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:14:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:14:34 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec608b5e34df195cc546df0cd8681f79c50de2626ab34ac88ded088eeeabdd2`  
		Last Modified: Tue, 31 Aug 2021 02:16:19 GMT  
		Size: 153.8 MB (153763006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; ppc64le

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

### `ibmjava:sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:a3d401d17e1a065486141ea8e10ff5906f071f624d6f8c0ecd9210b90f8c371b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.8 MB (183785846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8898d6467707589d684465f1d1e50f7cc38a64a488874a9c7bdf60dd6454580`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:03:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:03:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b45f85a7fc9d087b774ff2a8b70f276ef9a21d73a4c0cea48624b4c5665625e`  
		Last Modified: Tue, 31 Aug 2021 02:07:01 GMT  
		Size: 155.7 MB (155741812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk-alpine`

```console
$ docker pull ibmjava@sha256:0a9646c8baabc4a8691362b7d360b85152b1a42080f8e24afe278c02c1993baa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `ibmjava:sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:165f008e14f9a942d8dbf7fe4c890c8cb099d32b05411c577723b4f1b30e8afd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.0 MB (173969276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d2c24491172c646879581a1404932e9621f052535aa8bd2d7892c1557f0d63`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 13 Aug 2021 17:20:42 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:23:47 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='7dfc22f7c3ba656e33af1728d2f87e854cfc2616f153b3c8310a9d3ed89cd484';          YML_FILE='8.0/sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='2c1363167aa22f6b20f7c5d5a10bef06563a8405835b9e894eaf2fc2c966eca0';          YML_FILE='8.0/sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='f8a837860f8a3142c95b78eb1d9cf36bcb4c633ebde3293dca453ab2cdbd0dc2';          YML_FILE='8.0/sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='421e69d2307c0c8ab0f75fc0a32332f083286f46d4c4ac1742aaf12d7ae0dd99';          YML_FILE='8.0/sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='0dd9fbfe0aa12167d1ad6a482ba1493058440d379bcd0c7d1a18d3b44bcecca5';          YML_FILE='8.0/sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 13 Aug 2021 17:23:47 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e58e1236ecb91a26886efe0e3bc0f9987c5f9c78e9cbbd2a0928c606c22fae`  
		Last Modified: Fri, 13 Aug 2021 17:26:04 GMT  
		Size: 165.6 MB (165628426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:1426b37092f46c54e20d0da0bd6442093d5bc2d844e98725ba945f9ed03c4a60
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
$ docker pull ibmjava@sha256:887c9f2ce25e600a5bf4be416955305e4b861c43dc3d3825e0af284c60f6f4bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93877342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:decfb9ce4e6e2e91f7d3f01135f7b771a0d081dc5e4c54e2b8f376c4d3745737`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd587741057be9756d70f8ab18d1125a760b56daa6b8a5cae94927e996a66d25`  
		Last Modified: Tue, 31 Aug 2021 02:15:44 GMT  
		Size: 63.7 MB (63725517 bytes)  
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
$ docker pull ibmjava@sha256:81b010776718b38d7480d1921514b907df374deb08b6f9d8d4ee5d2829056489
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93411032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d11a7b7b65fcd918375630840f85095ae607331d52e0e893f5428a9659453f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:02:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:02:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90483140c8323edda00aa1cb79960f1c07e4689eea1184fea844f457a64a536c`  
		Last Modified: Tue, 31 Aug 2021 02:06:41 GMT  
		Size: 65.4 MB (65366998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj-alpine`

```console
$ docker pull ibmjava@sha256:c88f847ef2c5b73f1f6e5f6b9add320b20334f15f45aa01690c55844f4b4bec9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `ibmjava:sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:e601114cc10588c8e374928687f3f9cc6dfbcd78f6b13d3adb521c8bd30ccc34
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72691363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:965f0c92472e53a0df57f00f440828fbda0a222fdb8e4af567ad95b77b7a893f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:52:21 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Apr 2021 22:52:22 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Wed, 14 Apr 2021 22:52:39 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Fri, 13 Aug 2021 17:20:42 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:22:13 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Fri, 13 Aug 2021 17:22:13 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2473651455a528e12a77a3f77634a9edcf271c6673a5d553738621ea93c7f661`  
		Last Modified: Wed, 14 Apr 2021 22:54:59 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a476c88f89042a64d394f56be791c17d185be12546f3f0be1966502a0643c`  
		Last Modified: Wed, 14 Apr 2021 22:55:01 GMT  
		Size: 5.5 MB (5539744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9a1c56b92b631f405f01a45c95e52568be7cee05a479cd3ad4f92bb7b0e420`  
		Last Modified: Fri, 13 Aug 2021 17:25:20 GMT  
		Size: 64.4 MB (64350513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
