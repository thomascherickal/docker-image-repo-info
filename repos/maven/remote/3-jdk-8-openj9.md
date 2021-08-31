## `maven:3-jdk-8-openj9`

```console
$ docker pull maven@sha256:8ca933d7638cc084c0a61ccb1404cb6d5588f3f7c8bc3785fbe98d9c022975c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-jdk-8-openj9` - linux; amd64

```console
$ docker pull maven@sha256:7c4a75f5071a81e8f021665b677c8926c1c6447611a8807683909e3783d64211
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.4 MB (196411799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96aa1acf9fac6b89e20f2dddcc3b2b90e2f14fbd78f0d493af2fe9a5b4b07d7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 31 Aug 2021 01:20:55 GMT
ADD file:d2abf27fe2e8b0b5f4da68c018560c73e11c53098329246e3e6fe176698ef941 in / 
# Tue, 31 Aug 2021 01:20:56 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:26:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:26:55 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:28:28 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Tue, 31 Aug 2021 02:28:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='bc88be757a884b90a2bb91365b7e922c0e7d0fea991cd69d1f74c59b2257a4b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_ppc64le_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='7aff99f87482d5bb0969f13cddecfb600e755d428ae14f4292d08d4a1ea5f080';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_s390x_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='06d6c9421778575cf59d50f69b7ac6a7bb237485b3a3c2f89cfb61a056c7b2de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:28:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:28:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 Aug 2021 02:29:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 Aug 2021 07:57:21 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 07:57:21 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 07:57:22 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 07:57:22 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 07:57:34 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 07:57:34 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 07:57:34 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 07:57:34 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 07:57:35 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 07:57:35 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 07:57:35 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:35807b77a593c1147d13dc926a91dcc3015616ff7307cc30442c5a8e07546283`  
		Last Modified: Sat, 28 Aug 2021 03:03:19 GMT  
		Size: 28.6 MB (28570074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d71b8f96bb4f1c00b7375be1090b56f03343a56b15fdcdf40d5ac4a207e217`  
		Last Modified: Tue, 31 Aug 2021 02:37:06 GMT  
		Size: 16.0 MB (16033698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d42690ebb2934205c323789717a2550557c8cd0405f8686067655fd1a0afd3`  
		Last Modified: Tue, 31 Aug 2021 02:40:20 GMT  
		Size: 116.5 MB (116501493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579a69ca456a65d253979f4d4d3f91c0228cdf6b914e48eb3e9d06ebf5e3cd40`  
		Last Modified: Tue, 31 Aug 2021 02:40:10 GMT  
		Size: 4.0 MB (4048753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c37c914f558fd37377b99b367c4ec364bbd8675e0d70b5dcf3ad58746e6ba3`  
		Last Modified: Tue, 31 Aug 2021 08:03:38 GMT  
		Size: 31.3 MB (31256568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8061cee3898849ffba3b8a5132b305270120059df75802fd32d9fcf063dbfef`  
		Last Modified: Tue, 31 Aug 2021 08:03:36 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf26c23788d8428b9c8ecb6a5e1745d703f8412aa90c6ccac46cb0f701ae2a58`  
		Last Modified: Tue, 31 Aug 2021 08:03:36 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-8-openj9` - linux; ppc64le

```console
$ docker pull maven@sha256:e0e3dcee47d5c41a4ed04ec59710faebbee5ee09fecabd456526c730726f5508
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.7 MB (199657511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40c83188a7de0b4360beb1323209cd479bcd06a06a0144c2e98bd8d2db1548e5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:31:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:33:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:23 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Tue, 31 Aug 2021 02:39:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='bc88be757a884b90a2bb91365b7e922c0e7d0fea991cd69d1f74c59b2257a4b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_ppc64le_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='7aff99f87482d5bb0969f13cddecfb600e755d428ae14f4292d08d4a1ea5f080';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_s390x_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='06d6c9421778575cf59d50f69b7ac6a7bb237485b3a3c2f89cfb61a056c7b2de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:39:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:39:53 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 Aug 2021 02:40:39 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 Aug 2021 09:28:12 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 09:28:14 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 09:28:17 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 09:28:20 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 09:28:43 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 09:28:49 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 09:28:54 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 09:28:57 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 09:28:59 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 09:29:06 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 09:29:09 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6df1a3e21a26bf9e0775ad823e1762b00bf8c2a0650a891b7860b7fe18741a`  
		Last Modified: Tue, 31 Aug 2021 02:54:54 GMT  
		Size: 17.2 MB (17208636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d975f24a23ee9c958a787375728dd07d4142799be865706d7cd36275008e2569`  
		Last Modified: Tue, 31 Aug 2021 02:58:42 GMT  
		Size: 117.4 MB (117366443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a93cd1eed403588dbe7a3c62673fcd0565f22313ed58250d944b2c9248d2c9`  
		Last Modified: Tue, 31 Aug 2021 02:58:29 GMT  
		Size: 3.4 MB (3436116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca513fdb7b65dd90f3bc45ebb8ad02904ed694755b4d6843eb4730949c12f24e`  
		Last Modified: Tue, 31 Aug 2021 09:57:33 GMT  
		Size: 28.4 MB (28353313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d673ca0d68bf57f9b0fc372cf62e0e0961cbbef1776132b8ec057779500ab1cb`  
		Last Modified: Tue, 31 Aug 2021 09:57:29 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3cb4483ed81886c1cca392491e9af62159ad692ed6b0438bdb183f2dca208f`  
		Last Modified: Tue, 31 Aug 2021 09:57:29 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-8-openj9` - linux; s390x

```console
$ docker pull maven@sha256:d27682640062243b682373e60f0227df712f8ba6ca318047c22944d7a314eb18
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.5 MB (190451222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce05adafacfe2ec90c3096a6fbbc40e91bd135fb0d4cbe4dc1ddd5201a73e25`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:23 GMT
ADD file:979855f79ebaca36cc7878f71b2326f1cd189970fdb223b37cd64ee12d1c9a2b in / 
# Tue, 31 Aug 2021 01:42:27 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:07:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:08:16 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:40 GMT
ENV JAVA_VERSION=jdk8u292-b10_openj9-0.26.0
# Tue, 31 Aug 2021 02:11:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='bc88be757a884b90a2bb91365b7e922c0e7d0fea991cd69d1f74c59b2257a4b5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_ppc64le_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='7aff99f87482d5bb0969f13cddecfb600e755d428ae14f4292d08d4a1ea5f080';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_s390x_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='06d6c9421778575cf59d50f69b7ac6a7bb237485b3a3c2f89cfb61a056c7b2de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u292-b10_openj9-0.26.0/OpenJDK8U-jdk_x64_linux_openj9_8u292b10_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:12:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 02:12:04 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 Aug 2021 02:12:38 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 Aug 2021 03:01:47 GMT
ARG MAVEN_VERSION=3.8.2
# Tue, 31 Aug 2021 03:01:47 GMT
ARG USER_HOME_DIR=/root
# Tue, 31 Aug 2021 03:01:48 GMT
ARG SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222
# Tue, 31 Aug 2021 03:01:48 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries
# Tue, 31 Aug 2021 03:02:01 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.2/binaries MAVEN_VERSION=3.8.2 SHA=b0bf39460348b2d8eae1c861ced6c3e8a077b6e761fb3d4669be5de09490521a74db294cf031b0775b2dfcd57bd82246e42ce10904063ef8e3806222e686f222 USER_HOME_DIR=/root
RUN apt-get update && apt-get install -y curl   && mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 31 Aug 2021 03:02:02 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 31 Aug 2021 03:02:02 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 31 Aug 2021 03:02:03 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 31 Aug 2021 03:02:03 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 31 Aug 2021 03:02:03 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 31 Aug 2021 03:02:04 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:9fbf86d355c92d30b8de4c0360b0d79e1100e392d0885b6b5b302a1c3781dbf1`  
		Last Modified: Tue, 31 Aug 2021 01:44:13 GMT  
		Size: 27.1 MB (27127470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f47f4732fca5d50031ca6edf4776dd30d7e8eda1569ec50c3463d649acfc210`  
		Last Modified: Tue, 31 Aug 2021 02:23:22 GMT  
		Size: 15.7 MB (15741639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64682ead18c5f000dbc2ea8336d99e3b07971eeafa7a57f5a35777e41840c12c`  
		Last Modified: Tue, 31 Aug 2021 02:25:52 GMT  
		Size: 116.1 MB (116093986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d6a7a1a1273f79f89c77d0fad956e4b19613706941fcff8cfdb31d203a1175`  
		Last Modified: Tue, 31 Aug 2021 02:25:43 GMT  
		Size: 3.9 MB (3865428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69ee8b79b21ee8011835403bc46c527e04c1dd3d96d978a9a12e2a224ff58b0`  
		Last Modified: Tue, 31 Aug 2021 03:08:01 GMT  
		Size: 27.6 MB (27621483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4995e3149ea19f431b7b11e66a3a37d618990062a47c57c2b13930711fd33e`  
		Last Modified: Tue, 31 Aug 2021 03:08:00 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82964981b4d7b9589f6f9b687ac1ef873866cb7b5ae476a01b91cfdf362e72d8`  
		Last Modified: Tue, 31 Aug 2021 03:07:59 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
