## `maven:3-jdk-11-openj9`

```console
$ docker pull maven@sha256:1b3c49fefa31e211a4c47cc115fc1e8fdaa77b3e577a95c1db495e33f7b5b145
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-jdk-11-openj9` - linux; amd64

```console
$ docker pull maven@sha256:1dc266f8dd62c2d1eae063de884a6b211fe76495ed0f97ca0563a78b065776ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.1 MB (262128932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac9e90f2c2d2167d105e1cd6d5f9ab378fd88673d159e3ed0c6410666d660012`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 23 Apr 2021 22:21:34 GMT
ADD file:5c44a80f547b7d68b550b0e64aef898b361666857abf9a5c8f3f8d0567b8e8e4 in / 
# Fri, 23 Apr 2021 22:21:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:21:36 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:21:37 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:21:37 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 23:22:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 23:23:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 10 May 2021 18:22:17 GMT
ENV JAVA_VERSION=jdk-11.0.11+9_openj9-0.26.0
# Mon, 10 May 2021 18:22:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='691f2b252b5be5e36079177d56ff7b516e3058277f0ba852a16a9a0cd9668224';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        s390x)          ESUM='6bc30bfbcf689906e3961ba3fa3c183ba232fbf3ddb3206920e8dcddf5c0aae2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        amd64|x86_64)          ESUM='a605ab06f76533d44ce0828bd96836cc9c0e71ec3df3f8672052ea98dcbcca22';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.11%2B9_openj9-0.26.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.11_9_openj9-0.26.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 10 May 2021 18:22:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 10 May 2021 18:22:30 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Mon, 10 May 2021 18:23:06 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Mon, 10 May 2021 18:23:06 GMT
CMD ["jshell"]
# Tue, 11 May 2021 01:45:46 GMT
ARG MAVEN_VERSION=3.8.1
# Tue, 11 May 2021 01:45:46 GMT
ARG USER_HOME_DIR=/root
# Tue, 11 May 2021 01:45:46 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Tue, 11 May 2021 01:45:47 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Tue, 11 May 2021 01:45:56 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 11 May 2021 01:45:56 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 11 May 2021 01:45:56 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 11 May 2021 01:45:56 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 11 May 2021 01:45:56 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Tue, 11 May 2021 01:45:57 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 11 May 2021 01:45:57 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:345e3491a907bb7c6f1bdddcf4a94284b8b6ddd77eb7d93f09432b17b20f2bbe`  
		Last Modified: Fri, 16 Apr 2021 15:20:19 GMT  
		Size: 28.5 MB (28539626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57671312ef6fdbecf340e5fed0fb0863350cd806c92b1fdd7978adbd02afc5c3`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9250ddb7d0fa6d13302c7c3e6a0aa40390e42424caed1e5289077ee4054709`  
		Last Modified: Fri, 23 Apr 2021 22:23:02 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592ec2d7c1370aca6ef48ee1d20fbb3a4c148db400adc5dc575778c681f5dba0`  
		Last Modified: Fri, 23 Apr 2021 23:32:39 GMT  
		Size: 16.0 MB (16034099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103c7533e51ebf59132e96ef0cd9c0377cee19ac65f9878047e7ee72b3347019`  
		Last Modified: Mon, 10 May 2021 18:30:47 GMT  
		Size: 203.0 MB (202968892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f36ce8aad145550638de8659c593ec5ce5ffaa9cf07844a96f59cea4440bf8`  
		Last Modified: Mon, 10 May 2021 18:30:33 GMT  
		Size: 5.0 MB (4973084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1733bcbe01363778c9c4b6164d22907abcabed3082f1387cd0a9e85fcb5ac0fc`  
		Last Modified: Tue, 11 May 2021 01:51:44 GMT  
		Size: 9.6 MB (9610979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a2387caba777d685304d663b1df5246f16b24b3f0aeaa10b557d55aefbc29f`  
		Last Modified: Tue, 11 May 2021 01:51:43 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a16eff8fe99c019ae1ed4e835ae3e9b6e60908e6052b1d7183f9014c674e15c`  
		Last Modified: Tue, 11 May 2021 01:51:43 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-11-openj9` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:59b819d116ca1f73e64c5ad130d4b0d25128ecd12cc9cc86cd2fd2df0daeb866
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.7 MB (250707674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c1307f13788423b3bd82602d27cef742f654776aa82a9b0ef0aeae65136952`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:41:56 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:45:59 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Sat, 03 Apr 2021 05:46:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0ce9a8c38d154540610dfe03e59389734deb91c5cb9258408404c5026d4afa41';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_aarch64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='858f54946df9281a7410fffd3be82f7718d549088ea35c444f0887ac3fa2d3ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='19e76ec32f6dd6820b3e1043b8b30984edc69174ddbc72d1b22f490f245ef0e4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='941d5df125d2ad426391340f539408b13d61d00ed31dd79142ff1ac84864a79f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 05:46:13 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 05:46:14 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 03 Apr 2021 05:46:50 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 03 Apr 2021 05:46:51 GMT
CMD ["jshell"]
# Mon, 05 Apr 2021 17:41:02 GMT
ARG MAVEN_VERSION=3.8.1
# Mon, 05 Apr 2021 17:41:03 GMT
ARG USER_HOME_DIR=/root
# Mon, 05 Apr 2021 17:41:13 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Mon, 05 Apr 2021 17:41:17 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Mon, 05 Apr 2021 17:41:22 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Mon, 05 Apr 2021 17:41:23 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 05 Apr 2021 17:41:24 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 05 Apr 2021 17:41:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Mon, 05 Apr 2021 17:41:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Mon, 05 Apr 2021 17:41:27 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 05 Apr 2021 17:41:28 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f1b84b0f5e74897b899c79e269e294408197cec9b0f1770ff44d654874d22c`  
		Last Modified: Sat, 03 Apr 2021 05:53:32 GMT  
		Size: 15.9 MB (15894829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68fbfcf22c76eff662255b83459c2da834725abbd1e00a4c625bfcdfffc4432`  
		Last Modified: Sat, 03 Apr 2021 05:57:40 GMT  
		Size: 193.2 MB (193185055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915a730e34c1d572e57257ee9114b2837656780d1051f250a9abd835fcce9852`  
		Last Modified: Sat, 03 Apr 2021 05:57:17 GMT  
		Size: 4.8 MB (4837767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e591d28a6effcdb1f4260e516a1fbaa963c5018fda58a973b8f164cfe3ba1`  
		Last Modified: Mon, 05 Apr 2021 17:53:54 GMT  
		Size: 9.6 MB (9610955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477d4c9dfb20a017028022348a8bfeb0e2ec16ddce5d9c7eb8525edc4e6eadb1`  
		Last Modified: Mon, 05 Apr 2021 17:53:53 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18c449ed91aa2ead2744bf10272540ac148e822965ce02cd43416d8ad99a5b`  
		Last Modified: Mon, 05 Apr 2021 17:53:53 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-11-openj9` - linux; ppc64le

```console
$ docker pull maven@sha256:f4239ba52517caf15e181da7bf8412afaadd8397a7035949402b21b32cece753
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262513182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f006636174c5ff2dd2f368566e6767ed741e713742e970721dc76ace076713e7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 23 Apr 2021 22:31:45 GMT
ADD file:ec80070ca931734843261734e9ca18cd45a6130030c1a25abac3268e54776be5 in / 
# Fri, 23 Apr 2021 22:32:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 22:32:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 22:32:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 22:32:38 GMT
CMD ["/bin/bash"]
# Sat, 24 Apr 2021 01:16:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 24 Apr 2021 01:19:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 24 Apr 2021 01:28:36 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Sat, 24 Apr 2021 01:29:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='858f54946df9281a7410fffd3be82f7718d549088ea35c444f0887ac3fa2d3ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='19e76ec32f6dd6820b3e1043b8b30984edc69174ddbc72d1b22f490f245ef0e4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='941d5df125d2ad426391340f539408b13d61d00ed31dd79142ff1ac84864a79f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 24 Apr 2021 01:29:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 24 Apr 2021 01:29:18 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 24 Apr 2021 01:30:04 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 24 Apr 2021 01:30:10 GMT
CMD ["jshell"]
# Sat, 24 Apr 2021 02:49:37 GMT
ARG MAVEN_VERSION=3.8.1
# Sat, 24 Apr 2021 02:49:42 GMT
ARG USER_HOME_DIR=/root
# Sat, 24 Apr 2021 02:49:45 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Sat, 24 Apr 2021 02:49:47 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Sat, 24 Apr 2021 02:49:59 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 24 Apr 2021 02:50:04 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 24 Apr 2021 02:50:07 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 24 Apr 2021 02:50:09 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 24 Apr 2021 02:50:10 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Sat, 24 Apr 2021 02:50:12 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 24 Apr 2021 02:50:20 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8cdb522ceff72cef6133f5b26b5f9eac72760a06a86d5d6b7db34a5dde7b156f`  
		Last Modified: Fri, 23 Apr 2021 22:37:11 GMT  
		Size: 33.3 MB (33255388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21136d6107eea0892211e712ba6b20d15f74a37dd1bde1b2f0802e083e85c183`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a03f1456f472e398050e94cf3ac8873969ce172a153bb511be780fe49403c47`  
		Last Modified: Fri, 23 Apr 2021 22:37:05 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da07529aeac8fe5c90c5bb8c4f516c9d6fd248cc1daa5fecd137c809bce39bb6`  
		Last Modified: Sat, 24 Apr 2021 01:40:58 GMT  
		Size: 17.2 MB (17209103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01232f0a1b9f4d73d72e5caea2509409d605278996adb7f21eb8c9f03a0fb870`  
		Last Modified: Sat, 24 Apr 2021 01:45:57 GMT  
		Size: 198.2 MB (198187826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4ba7dfbeb4268dd7bacfe16a6c81d5e396a18d6a5df9f4b575dcd6b94f36f5`  
		Last Modified: Sat, 24 Apr 2021 01:45:34 GMT  
		Size: 4.2 MB (4247683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d556952c43a21c40ef9f13a92589695bb2381d10dbe54efa39be8bdd2015058`  
		Last Modified: Sat, 24 Apr 2021 03:03:29 GMT  
		Size: 9.6 MB (9610932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60357d7205229d28641c7b24c6b0894bdc04dc7b69dc54be68d3f399676a4cc9`  
		Last Modified: Sat, 24 Apr 2021 03:03:29 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3a4dfe7524aa01258dc9902b8b953ba9dce2ca8b498176fac860867882bb9`  
		Last Modified: Sat, 24 Apr 2021 03:03:28 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-11-openj9` - linux; s390x

```console
$ docker pull maven@sha256:00de93ef5119052f0ca239273d6a9f1d36129f796e6e846dfb0b3b0285a4ac94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.8 MB (252758696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:350433af11527e081321de6f6cefafe919baa012111baf18c28c0bde5468d855`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 23 Apr 2021 21:45:20 GMT
ADD file:282d950116f923276efabd13c7dc17b942821edb14ffac4b89b9a50bcdf99e17 in / 
# Fri, 23 Apr 2021 21:45:26 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Apr 2021 21:45:27 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Apr 2021 21:45:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Apr 2021 21:45:29 GMT
CMD ["/bin/bash"]
# Fri, 23 Apr 2021 22:03:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 23 Apr 2021 22:04:03 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Apr 2021 22:10:11 GMT
ENV JAVA_VERSION=jdk-11.0.10+9_openj9-0.24.0
# Fri, 23 Apr 2021 22:10:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='858f54946df9281a7410fffd3be82f7718d549088ea35c444f0887ac3fa2d3ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_ppc64le_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='19e76ec32f6dd6820b3e1043b8b30984edc69174ddbc72d1b22f490f245ef0e4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_s390x_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='941d5df125d2ad426391340f539408b13d61d00ed31dd79142ff1ac84864a79f';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9_openj9-0.24.0/OpenJDK11U-jdk_x64_linux_openj9_11.0.10_9_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 23 Apr 2021 22:10:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Apr 2021 22:10:43 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 23 Apr 2021 22:11:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 23 Apr 2021 22:11:21 GMT
CMD ["jshell"]
# Fri, 23 Apr 2021 23:08:07 GMT
ARG MAVEN_VERSION=3.8.1
# Fri, 23 Apr 2021 23:08:08 GMT
ARG USER_HOME_DIR=/root
# Fri, 23 Apr 2021 23:08:09 GMT
ARG SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d
# Fri, 23 Apr 2021 23:08:09 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries
# Fri, 23 Apr 2021 23:08:23 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.1/binaries MAVEN_VERSION=3.8.1 SHA=0ec48eb515d93f8515d4abe465570dfded6fa13a3ceb9aab8031428442d9912ec20f066b2afbf56964ffe1ceb56f80321b50db73cf77a0e2445ad0211fb8e38d USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 23 Apr 2021 23:08:24 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 23 Apr 2021 23:08:25 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 23 Apr 2021 23:08:25 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 23 Apr 2021 23:08:26 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 23 Apr 2021 23:08:26 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 23 Apr 2021 23:08:27 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:de53239ada2db01e7972c3f6eddcf6729f7cf3102be78e0b41363125ce7c2425`  
		Last Modified: Fri, 23 Apr 2021 21:47:14 GMT  
		Size: 27.1 MB (27136362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12932016d0f51acb5c5e5ba5b420a369401a7df47a219f24680bbc05ffde7e11`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 840.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46997f76c5876e3274170b667463b3d88475cd696ccbc735d2f63965668673ad`  
		Last Modified: Fri, 23 Apr 2021 21:47:10 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bab416938acf6dd045c9fc9097e5768c61b5899b07d110ab3844f447e12b113`  
		Last Modified: Fri, 23 Apr 2021 22:19:05 GMT  
		Size: 15.7 MB (15741779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c127b61154e18f0bd2feb45f92193c2218f3a1ebea478337beb296916a0543b7`  
		Last Modified: Fri, 23 Apr 2021 22:22:04 GMT  
		Size: 195.5 MB (195455594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a9dcd5840f369a40d4e645c9407f7f69cfb05e41fa2cb2ba49a3d4df4ef740`  
		Last Modified: Fri, 23 Apr 2021 22:21:51 GMT  
		Size: 4.8 MB (4811749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e99d24e60fde9c6f457c7435bff422c0a096f435aa5ac4350dcc6c6b9580179`  
		Last Modified: Fri, 23 Apr 2021 23:14:33 GMT  
		Size: 9.6 MB (9610970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6da8d4bbc1de40aadc9f5540320ea0d2a8d10745b246899a50f476cd41737e8`  
		Last Modified: Fri, 23 Apr 2021 23:14:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d7bdf2640fddaa050990d3e21ae6650a8e7259a868d3ab301862aab2eb577f`  
		Last Modified: Fri, 23 Apr 2021 23:14:32 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
