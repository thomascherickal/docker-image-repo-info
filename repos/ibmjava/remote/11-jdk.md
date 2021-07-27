## `ibmjava:11-jdk`

```console
$ docker pull ibmjava@sha256:68f34d4332ab93da3fbba68e16111db0cbfe9b08f976953d47a780fd949c56e2
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
$ docker pull ibmjava@sha256:adc037d394997f46bfe36765c48dda9ceed248ab08dbdbdca182c75d4f21e55d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.9 MB (267885941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:211fad5facc116182143f4cc37e5846169cf388e444e6d605206fa3504b8ee20`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:24 GMT
ADD file:cdca4c00902f291c6bc305420b891f5149b6833b5f9892232ea690d38adfff3f in / 
# Tue, 13 Jul 2021 23:22:32 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 04:43:22 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 14 Jul 2021 04:44:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 04:44:41 GMT
ENV JAVA_VERSION=11.0.11.0
# Wed, 14 Jul 2021 04:45:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 14 Jul 2021 04:46:08 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:157ef43c951ca9b65226089aef70b09df64b81636884260390a329c24a3c614b`  
		Last Modified: Tue, 13 Jul 2021 23:27:34 GMT  
		Size: 33.3 MB (33287846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025b44975aec895d0939de4760d4933a2b1e003c6ca6fb32160f377842df54c`  
		Last Modified: Wed, 14 Jul 2021 04:48:07 GMT  
		Size: 3.3 MB (3292553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb2ea47bfc77eab220abd4307578ffca026d6c4ffba60f55f956e4b1fe7e332`  
		Last Modified: Wed, 14 Jul 2021 04:48:35 GMT  
		Size: 231.3 MB (231305542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:11-jdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:59ad5ad7e4055dec239875641b055a0cd5ca9e4d3cb5f0108abff41adc969e46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.6 MB (258594834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a614f68ee8490d7c53a69c28817bb4f20a6a42af2ce6531157edcd253e121c14`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:12 GMT
ADD file:b8731edfdacfade2ec96757342f216962f3971b24077a9144da3f80003e6893e in / 
# Mon, 26 Jul 2021 20:55:14 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:16:06 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 21:16:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:16:11 GMT
ENV JAVA_VERSION=11.0.11.0
# Mon, 26 Jul 2021 21:17:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='037363b1dd35d7b6a67137baf1c73589b4f7b4e177d40394897726ad6056babd';          YML_FILE='11.0/jdk/linux/x86_64/index.yml';          ;;        ppc64el|ppc64le)          ESUM='717d3c0427d34af710f10f62be68cc78576ebb80523ff65ab3e8c1fe6a785569';          YML_FILE='11.0/jdk/linux/ppc64le/index.yml';          ;;        s390x)          ESUM='b2e64a73dab3fed0a845144377a9cd2945b87c005ba2418f1abbefea45321167';          YML_FILE='11.0/jdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     mv /opt/ibm/jdk-11* /opt/ibm/java;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Mon, 26 Jul 2021 21:17:17 GMT
ENV JAVA_HOME=/opt/ibm/java PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:38800a0044dea146ca3c3a08bc2c9c956396ad3241a3c343010775650298c379`  
		Last Modified: Mon, 26 Jul 2021 20:57:03 GMT  
		Size: 27.1 MB (27149898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a5d4ce9687b9dddc48ae97759be14d618c5e8b829165a71ccd97bf4302b064`  
		Last Modified: Mon, 26 Jul 2021 21:18:52 GMT  
		Size: 2.7 MB (2737636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577566ca0d9e48ff62df2f07972c71151e6ceef11c58f87f44a3d5173da5575b`  
		Last Modified: Mon, 26 Jul 2021 21:19:07 GMT  
		Size: 228.7 MB (228707300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
