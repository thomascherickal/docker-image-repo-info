## `adoptopenjdk:15_36-jdk-openj9-0.22.0`

```console
$ docker pull adoptopenjdk@sha256:3c0488baf7a85a72fedcc2f05fc431b06dd14d23a1c7d489967908d3042a5a51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `adoptopenjdk:15_36-jdk-openj9-0.22.0` - linux; amd64

```console
$ docker pull adoptopenjdk@sha256:41837c3740a473b26d9563d4fdfadcbe4e7862a02d64fc5b5ac4aeeff02bae65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243780197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe137ae7359ac7ff9fc967dc9b936b9e860fcf3f37efe8ee8632caab2a3ab2b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 25 Sep 2020 22:33:49 GMT
ADD file:4974bb5483c392fb54a35f3799802d623d14632747493dce5feb4d435634b4ac in / 
# Fri, 25 Sep 2020 22:33:50 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:33:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:33:52 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:33:52 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:10:55 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 25 Sep 2020 23:11:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 17:15:33 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Tue, 20 Oct 2020 17:15:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='88058a977c63382b59b7aaaec08d656490494b2c9575ae787c873de1b2baeaca';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_ppc64le_linux_openj9_15_36_openj9-0.22.0.tar.gz';          ;;        s390x)          ESUM='1cb8366199635c82a58b2619483f84318e9ead5b542b52ffc355fb561adb0f14';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_s390x_linux_openj9_15_36_openj9-0.22.0.tar.gz';          ;;        amd64|x86_64)          ESUM='3f016e23a1fba0b1d29f03415c36d54a8a33480ce1d238fbef09d38c5a69eff7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_linux_openj9_15_36_openj9-0.22.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 17:15:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Oct 2020 17:15:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Tue, 20 Oct 2020 17:17:12 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 20 Oct 2020 17:17:13 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 20 Oct 2020 17:17:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:171857c49d0f5e2ebf623e6cb36a8bcad585ed0c2aa99c87a055df034c1e5848`  
		Last Modified: Tue, 22 Sep 2020 12:21:27 GMT  
		Size: 26.7 MB (26701612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419640447d267f068d2f84a093cb13a56ce77e130877f5b8bdb4294f4a90a84f`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e52f862619ab016d3bcfbd78e5c7aaaa1989b4c295e6dbcacddd2d7b93e1f5`  
		Last Modified: Fri, 25 Sep 2020 22:36:49 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4d4e9526b1adecc10515315b09e75d88526e75fba0552b3fbb933f40d293e9`  
		Last Modified: Fri, 25 Sep 2020 23:16:31 GMT  
		Size: 13.9 MB (13875646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf7a589de51535ae9650ef7af66981025376c953a43d16b02d603911342c01`  
		Last Modified: Tue, 20 Oct 2020 17:23:03 GMT  
		Size: 197.6 MB (197625629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c760b258470d391ebc12772a694bafeb8ca96db8faced4618019f719995c428`  
		Last Modified: Tue, 20 Oct 2020 17:22:44 GMT  
		Size: 5.6 MB (5576296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-openj9-0.22.0` - linux; s390x

```console
$ docker pull adoptopenjdk@sha256:b50c1de59c4a65e2ffd4af90acb5901993affc08971fe1d5444ab754432ae46d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240215468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad567159469a589d0cdd068a21d74b9717e27ea6b5799897dc651573ed803d1a`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 25 Sep 2020 22:44:45 GMT
ADD file:0a8ec4fb62616b6605197e20e0a7b511dc5b03d4af0e04c929dfd9fb457d2065 in / 
# Fri, 25 Sep 2020 22:44:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:44:48 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 22:44:48 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:44:48 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:07:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 25 Sep 2020 23:07:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 16:52:43 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Tue, 20 Oct 2020 16:52:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='88058a977c63382b59b7aaaec08d656490494b2c9575ae787c873de1b2baeaca';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_ppc64le_linux_openj9_15_36_openj9-0.22.0.tar.gz';          ;;        s390x)          ESUM='1cb8366199635c82a58b2619483f84318e9ead5b542b52ffc355fb561adb0f14';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_s390x_linux_openj9_15_36_openj9-0.22.0.tar.gz';          ;;        amd64|x86_64)          ESUM='3f016e23a1fba0b1d29f03415c36d54a8a33480ce1d238fbef09d38c5a69eff7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_linux_openj9_15_36_openj9-0.22.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 20 Oct 2020 16:53:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 20 Oct 2020 16:53:00 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Tue, 20 Oct 2020 16:54:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     SCC_GEN_RUNS_COUNT=3;     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     for i in $(seq 0 $SCC_GEN_RUNS_COUNT);     do         "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;         sleep 5;         "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh;         sleep 5;     done;         FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 20 Oct 2020 16:54:25 GMT
ENV OPENJ9_JAVA_OPTIONS=-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 20 Oct 2020 16:54:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dd2de95b9a1c45e92bcc791d469201229b58d68187c99de6b08b00a13fa33393`  
		Last Modified: Fri, 25 Sep 2020 22:45:52 GMT  
		Size: 25.4 MB (25371975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38a48ef4dfab2bd639d381d11b3390b6bf8860b2ef3356e9bb55f7cb8c775f9`  
		Last Modified: Fri, 25 Sep 2020 22:45:51 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eced51184728468b347a6e3f143c356cd174c4a54be3cc10ec5aeddb402765fd`  
		Last Modified: Fri, 25 Sep 2020 22:45:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eb688908dd55f188cb3c2b3bb83efc30566ace847ab51ba28adbed5d30266b`  
		Last Modified: Fri, 25 Sep 2020 23:12:47 GMT  
		Size: 13.6 MB (13595725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75870c2e8a6e991b9b98f63bd0f0da128f2230ddac6629a02704d66fe77d86`  
		Last Modified: Tue, 20 Oct 2020 17:00:51 GMT  
		Size: 195.7 MB (195685401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3270172ce1c29aa2af9b03b1b628f42891fca640a16bf3107b74ff694f138791`  
		Last Modified: Tue, 20 Oct 2020 17:00:05 GMT  
		Size: 5.6 MB (5561330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-openj9-0.22.0` - windows version 10.0.17763.1518; amd64

```console
$ docker pull adoptopenjdk@sha256:02cc5dd05846a187738bfd93f4a2eede6fb5b89f1bcc89ca9ab1d8e9a263716b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2756017250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a77a72d6206b17429b2a5e5fc491ba1743f2a16038f49aa88661ecb90be53e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:27:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:34:37 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Sat, 17 Oct 2020 01:37:28 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:37:29 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Sat, 17 Oct 2020 01:37:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5e61fff845eda39f31bdf5d797254fdf656ee79d8c294c1713007864bc4c2535`  
		Last Modified: Wed, 14 Oct 2020 12:50:32 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b72aeaa8c42cf486f1e47e7b58d97f365ca33f5f183447aa42a4f296e2bd85b`  
		Last Modified: Sat, 17 Oct 2020 02:22:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59149a8e1a4d595880d79b242a53396b588c5a52667dceac1d6294e6fe4de019`  
		Last Modified: Sat, 17 Oct 2020 02:23:10 GMT  
		Size: 381.9 MB (381922588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83c6028ca1988dec1ef628f1afc872acc805099e47d6b79488813cf4470e838`  
		Last Modified: Sat, 17 Oct 2020 02:22:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b18514c1fb7253e06e7133b6a8f2a9453d90e82f938b1754cb861b2d48ac55`  
		Last Modified: Sat, 17 Oct 2020 02:22:42 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adoptopenjdk:15_36-jdk-openj9-0.22.0` - windows version 10.0.14393.3986; amd64

```console
$ docker pull adoptopenjdk@sha256:f5957d7c096b4cfe8fbb50dc5867a5cd51a7a03d1e1b7485740ef3356bb6ab77
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6123906946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f7eefa084b3e3ec198004f25f29ed99e746049d97e6ca98faea92398277d09`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 12:31:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 17 Oct 2020 01:37:37 GMT
ENV JAVA_VERSION=jdk-15+36_openj9-0.22.0
# Sat, 17 Oct 2020 01:41:00 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15%2B36_openj9-0.22.0/OpenJDK15U-jdk_x64_windows_openj9_15_36_openj9-0.22.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '88dd04dc008ff18e09ad158046a650797ff8e5ce0f1880515e359c49f0fddd4e') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 17 Oct 2020 01:41:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Sat, 17 Oct 2020 01:41:02 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e300a13db0fbbf48a676ace9db3b0de292c825dfa01e6d82979d96ebc23d3675`  
		Last Modified: Wed, 14 Oct 2020 12:51:34 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086d2ce2178c7eb1c489e3433b970bcb6bfbdb0a09a5c7a1a108e787f63973a8`  
		Last Modified: Sat, 17 Oct 2020 02:23:40 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c377a2f5b23560dee15fcef3762e2741e7e2c5f892ae936e4a1f64cbe0dc30`  
		Last Modified: Sat, 17 Oct 2020 02:24:23 GMT  
		Size: 382.6 MB (382550751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc49d6979355ee36af04e2d228dba89b6516f7ba0a719b56fbafe46a264d41ce`  
		Last Modified: Sat, 17 Oct 2020 02:23:40 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf4dfaf2158f06d28b4b7b43441e3f45d1562e3f2db31a8a70941782bc0a402`  
		Last Modified: Sat, 17 Oct 2020 02:23:41 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
