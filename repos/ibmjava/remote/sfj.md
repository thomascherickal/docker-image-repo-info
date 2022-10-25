## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:bd9e2fd12a671a95eaf0ceeb4a1a66cbcadfd683affee6fc2f56a6752f812e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:3ea5253c17acc8d7754bf33fd31f11a87fd01fd69a21e5480659628893593a2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94688123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49e2894dc3f6b0063a13f30c72d4713bc6c15d1ed2a27e78bda4d6e0d556864`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 17:13:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 17:13:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:13:31 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 17:15:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='14c98ced5d88c2420df74edd155da7610171b441890234706b570e52e8ca92b6';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c9603ebfaf3c6a0737b73ff24bdfe87892df4819d2b52931c9a8b2e69cbbc529';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='ca0625b0e979ae4681a9441ab5e0b777c02885ba0894521166c526cef655e033';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='592758a743ed59742f18deaf4d5b3bf74577c470a306f0304da7d0c317a50dfa';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3255b688a27c7eb5378f706120cccfaaba4f284b33d33324b424dba1a8224fa7';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 17:15:09 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9d8b98df188102d0298ec847e22cee30b83e6a2203144208de17a84f4e915a`  
		Last Modified: Wed, 05 Oct 2022 17:16:34 GMT  
		Size: 3.0 MB (2957821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b587ef064cfb28891b19aa7afccb145157bc50fb3bdc1a3c45d5091a70ed747e`  
		Last Modified: Wed, 05 Oct 2022 17:17:03 GMT  
		Size: 65.0 MB (65018450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:9b2b96296cd7b42df00dc94f8824e36d8c816b7587141abd1f93d6b006286724
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94534098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:141133da1efdb74be240850ce6be8c8cd18ebcca16e70dd163dca60c9db85021`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:51:15 GMT
ADD file:ee35e95b906b98c2d7493d8c365bf5aaf351251abce763f9be2d9fa6cc541aaf in / 
# Tue, 04 Oct 2022 23:51:15 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 14:18:49 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 05 Oct 2022 14:19:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 14:19:08 GMT
ENV JAVA_VERSION=8.0.7.16
# Wed, 05 Oct 2022 14:20:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='14c98ced5d88c2420df74edd155da7610171b441890234706b570e52e8ca92b6';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c9603ebfaf3c6a0737b73ff24bdfe87892df4819d2b52931c9a8b2e69cbbc529';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='ca0625b0e979ae4681a9441ab5e0b777c02885ba0894521166c526cef655e033';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='592758a743ed59742f18deaf4d5b3bf74577c470a306f0304da7d0c317a50dfa';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3255b688a27c7eb5378f706120cccfaaba4f284b33d33324b424dba1a8224fa7';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 05 Oct 2022 14:20:53 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:6d1a231d13b300fc73c20f074f3accd74dcff41afd006c272719fdf8cf9be075`  
		Last Modified: Tue, 04 Oct 2022 23:52:01 GMT  
		Size: 27.2 MB (27165243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766942147a0b9643dde5105adf200582201a20a0ef3ad86d7136e55632dd694c`  
		Last Modified: Wed, 05 Oct 2022 14:22:30 GMT  
		Size: 3.0 MB (2983220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a9105e94ebbb6b06a2102c284e9774caa9c6f039bfd842b52642884dafb4fa`  
		Last Modified: Wed, 05 Oct 2022 14:23:00 GMT  
		Size: 64.4 MB (64385635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:9dabf08ad63af7b663710877b426e3dbfb9853cf78f8ec8d100b2ee55680a472
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98813327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b94b363291300aae078f232ac4e08fc5169dad60c3e24edc04943e5d6ae5506`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 14:07:39 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 25 Oct 2022 14:08:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 14:08:09 GMT
ENV JAVA_VERSION=8.0.7.16
# Tue, 25 Oct 2022 14:12:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='14c98ced5d88c2420df74edd155da7610171b441890234706b570e52e8ca92b6';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c9603ebfaf3c6a0737b73ff24bdfe87892df4819d2b52931c9a8b2e69cbbc529';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='ca0625b0e979ae4681a9441ab5e0b777c02885ba0894521166c526cef655e033';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='592758a743ed59742f18deaf4d5b3bf74577c470a306f0304da7d0c317a50dfa';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3255b688a27c7eb5378f706120cccfaaba4f284b33d33324b424dba1a8224fa7';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 25 Oct 2022 14:12:24 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3bd07fd743978e6c122138fc96d49720949d9378615ea1610865b23325b7af`  
		Last Modified: Tue, 25 Oct 2022 14:16:02 GMT  
		Size: 3.1 MB (3076044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fdefdad1b777f50a38ab5b70f37dd29e150e497fe49e6aec7bd1acf4ab5a9f2`  
		Last Modified: Tue, 25 Oct 2022 14:18:18 GMT  
		Size: 65.3 MB (65294058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:f4213e0f587804451a9e8aa651e0864ed68d872dda08a5f7b08edb7e722d0370
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94161774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e5d3788d4c6c8ff71c0723cdae2b72e1538d6d39eabed4793e3fb4ce8c8db2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:08:47 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 25 Oct 2022 08:09:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:09:02 GMT
ENV JAVA_VERSION=8.0.7.16
# Tue, 25 Oct 2022 08:10:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='14c98ced5d88c2420df74edd155da7610171b441890234706b570e52e8ca92b6';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c9603ebfaf3c6a0737b73ff24bdfe87892df4819d2b52931c9a8b2e69cbbc529';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='ca0625b0e979ae4681a9441ab5e0b777c02885ba0894521166c526cef655e033';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='592758a743ed59742f18deaf4d5b3bf74577c470a306f0304da7d0c317a50dfa';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='3255b688a27c7eb5378f706120cccfaaba4f284b33d33324b424dba1a8224fa7';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 25 Oct 2022 08:10:43 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b48aa864b900d3e1ae35d49fc6be512e393a95d7020a8372679d9d04253958`  
		Last Modified: Tue, 25 Oct 2022 08:12:34 GMT  
		Size: 2.7 MB (2671897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0507b75e796b10ff38699a9e84df563cc47a7f5af9eb937f3ed5f50aad2fe722`  
		Last Modified: Tue, 25 Oct 2022 08:12:58 GMT  
		Size: 66.1 MB (66118416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
