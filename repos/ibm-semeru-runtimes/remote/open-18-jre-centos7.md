## `ibm-semeru-runtimes:open-18-jre-centos7`

```console
$ docker pull ibm-semeru-runtimes@sha256:95300c77f99def13478a82b0620673b2e34339dcb0add9c61a740ea0f8fdc50c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `ibm-semeru-runtimes:open-18-jre-centos7` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:2ee6938b7d4289a2c829630265f6ae3b46ea972ed3f98297162cb192ef7709a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141398219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b93acd3b5cc5bb2921461dc9492735e97eb64443139e3bd5de2228da5a1aabb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 18:51:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 15 Sep 2021 18:51:48 GMT
RUN yum install -y tzdata openssl curl ca-certificates fontconfig gzip tar     && yum clean all
# Wed, 27 Apr 2022 20:08:18 GMT
ENV JAVA_VERSION=jdk-18.0.1+10_openj9-0.32.0
# Wed, 27 Apr 2022 20:08:21 GMT
RUN set -eux;     ARCH="$(uname -m)";     case "${ARCH}" in        aarch64|arm64)          ESUM='637d1399d3e5da6dcbdaaf4ab0610b1320bdeb390e8bc7dd6a1f84d50161e8c8';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='60a3c1d32f60a924687efbccdd410df743cc4098088b5ca6a424509aa0a02eab';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9e23d79cc6d6aa6110f8ff2a4d89c4a323ba0470632ac925f2acd67c2c1b64b8';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Apr 2022 20:08:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Apr 2022 20:08:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 27 Apr 2022 20:08:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df6893209e3a4a16d453c0b998ba34f62067ad6099b971afc4f30040eb1467d`  
		Last Modified: Wed, 15 Sep 2021 18:54:13 GMT  
		Size: 12.7 MB (12706445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66ad1aca1a29c4e476bae1ecde36c8b64182a8324d04f3c13ba9aaba76c3519`  
		Last Modified: Wed, 27 Apr 2022 20:15:24 GMT  
		Size: 47.9 MB (47850119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e080362805a9376151493318e6f2d15a7732a6efb916e07c0397d0e1dc574e`  
		Last Modified: Wed, 27 Apr 2022 20:15:19 GMT  
		Size: 4.7 MB (4744498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18-jre-centos7` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:f241f60c95bfe7eaf917800b58c4640454174cae8a720124947b59fdd298ba56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.7 MB (171677177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2754ce1b17a971c324f199c7fe1373b5bfded4b2cc18699dbf7f42505856394e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 14 Feb 2022 19:39:36 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Mon, 14 Feb 2022 19:39:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Mon, 14 Feb 2022 19:39:38 GMT
CMD ["/bin/bash"]
# Mon, 14 Feb 2022 19:59:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 14 Feb 2022 19:59:30 GMT
RUN yum install -y tzdata openssl curl ca-certificates fontconfig gzip tar     && yum clean all
# Tue, 31 May 2022 23:55:25 GMT
ENV JAVA_VERSION=jdk-18.0.1.1+2_openj9-0.32.0
# Tue, 31 May 2022 23:55:30 GMT
RUN set -eux;     ARCH="$(uname -m)";     case "${ARCH}" in        aarch64|arm64)          ESUM='86bf05dae9510bd0679bf7489378b1411cf816885adbde7108d52e3b85d76d84';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b5e650847c39efa65e294df46c073091e9089579decdb125867af8e4bae2cb5';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='761807f0c13500b1e94824928050c3485932cb596e2a499935f67b734c644c97';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 May 2022 23:55:31 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 May 2022 23:55:31 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 May 2022 23:56:09 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130170151f9f3710dd5b3e651dfb953b4ced0d33d1b4c77d70c35bd91d07e040`  
		Last Modified: Mon, 14 Feb 2022 20:04:32 GMT  
		Size: 13.1 MB (13059526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5085d256fa8caf114c348052cd2ceeec52cf7329581ab65749f2e004f169b8d9`  
		Last Modified: Tue, 31 May 2022 23:59:24 GMT  
		Size: 45.7 MB (45687049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780a8ab18043e0d0c42c0b348cdd9af8227d2513b5672f764d145a7a823c8d3a`  
		Last Modified: Tue, 31 May 2022 23:59:18 GMT  
		Size: 4.6 MB (4555657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18-jre-centos7` - linux; ppc64le

```console
$ docker pull ibm-semeru-runtimes@sha256:3b6ac5a95ad7fde3a6b5c1b775ab69fafbf515aef7664dc368fe6626d0792c58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145049469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ba97adf8ebb1b7c65838b7d252b45f9f11783f1f94a00aeef4b31b96b8487c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Sep 2021 18:29:27 GMT
ADD file:7f21ae7d20a8e347d8b678bcf26be83abb1ee27d3b567c9cddd993e45ce8ac34 in / 
# Wed, 15 Sep 2021 18:29:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:29:40 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 21:27:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 15 Sep 2021 21:29:19 GMT
RUN yum install -y tzdata openssl curl ca-certificates fontconfig gzip tar     && yum clean all
# Wed, 27 Apr 2022 22:38:15 GMT
ENV JAVA_VERSION=jdk-18.0.1+10_openj9-0.32.0
# Wed, 27 Apr 2022 22:38:29 GMT
RUN set -eux;     ARCH="$(uname -m)";     case "${ARCH}" in        aarch64|arm64)          ESUM='637d1399d3e5da6dcbdaaf4ab0610b1320bdeb390e8bc7dd6a1f84d50161e8c8';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='60a3c1d32f60a924687efbccdd410df743cc4098088b5ca6a424509aa0a02eab';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='9e23d79cc6d6aa6110f8ff2a4d89c4a323ba0470632ac925f2acd67c2c1b64b8';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Apr 2022 22:38:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Apr 2022 22:38:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 27 Apr 2022 22:39:18 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:3fe478aaff9b8f3ba958253e7339e9016ec07c075b805ebfc8cd372ddd01ee64`  
		Last Modified: Tue, 17 Nov 2020 04:06:20 GMT  
		Size: 80.5 MB (80516460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f502386ff4e2195af1b6b4432c6ccd0fabc7a63dd38550f635eacaa707c74a`  
		Last Modified: Wed, 15 Sep 2021 21:38:40 GMT  
		Size: 12.6 MB (12616024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c255a02fc110237aeda3bbcebc37fa4031e648cad24cb18db313c6ac932b59`  
		Last Modified: Wed, 27 Apr 2022 22:48:24 GMT  
		Size: 48.2 MB (48215432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62d3919e992ff09ac954691163498708a77456339a964dc431a125d038e34e`  
		Last Modified: Wed, 27 Apr 2022 22:48:16 GMT  
		Size: 3.7 MB (3701553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
