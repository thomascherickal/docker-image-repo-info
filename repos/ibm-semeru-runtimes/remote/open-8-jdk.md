## `ibm-semeru-runtimes:open-8-jdk`

```console
$ docker pull ibm-semeru-runtimes@sha256:538f9bfa665b4048115c3da9441d63ca8668be3f43f6131d1ce348e63aac441d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `ibm-semeru-runtimes:open-8-jdk` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:ec28b2404eb5be2e687df1f0238802b3f408296d559edf21363e9d351dda9efa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.3 MB (163343163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00424a6646ea204003be49468aef027f341dcc329f0ef419a88e21b690ca5991`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 17:18:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:19:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:19:10 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.1
# Wed, 05 Oct 2022 17:19:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='55eb440eedc331081012664e18b4640988a210d6443289410662ff03c0b2bf05';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7b9da287bd3c77142a1b3e42e0ff3aa3ce5ad9aeb9ae81e4894a742fe08c057f';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='b748ef07a800b4f12ade9337e4f3e42ee5207e57e688367ab0dd978ebd1876ea';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='a87652c8150390777aa98bbe6452788522d01fd0a68ab3133663191a9cd32555';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 17:19:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 17:19:17 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 17:19:52 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223828f10a72de9358a21e0ea6f8da2f9fef1ed531e11a888a42e61b938994a3`  
		Last Modified: Wed, 05 Oct 2022 17:34:34 GMT  
		Size: 12.1 MB (12104036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feaa1a809878c90d57d92594eefcabbae11d027126759e5edaa3563053b4453`  
		Last Modified: Wed, 05 Oct 2022 17:34:42 GMT  
		Size: 116.6 MB (116645147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6e828c8dea30de73ea025b6cdf687fc2beab1d2b41b2d10a4440336eabbf40`  
		Last Modified: Wed, 05 Oct 2022 17:34:33 GMT  
		Size: 4.2 MB (4165052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8-jdk` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:8392c74c80033aa564b8a0740957ae39c2adfced8c3f813b2de0debe43c3febe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158591811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890d6aea82e441a037aa55eb42649c34f87d528c811e58836e159eba49fb9c24`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:30:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 16:30:43 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:30:43 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.1
# Wed, 05 Oct 2022 16:30:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='55eb440eedc331081012664e18b4640988a210d6443289410662ff03c0b2bf05';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7b9da287bd3c77142a1b3e42e0ff3aa3ce5ad9aeb9ae81e4894a742fe08c057f';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='b748ef07a800b4f12ade9337e4f3e42ee5207e57e688367ab0dd978ebd1876ea';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='a87652c8150390777aa98bbe6452788522d01fd0a68ab3133663191a9cd32555';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 16:30:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:30:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 16:31:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70f1e149a1b47a62ec60d4a4b409048e900d6f1fa93d0f7d83287fe79d4457c`  
		Last Modified: Wed, 05 Oct 2022 16:48:02 GMT  
		Size: 12.1 MB (12064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7003b2916316bb3c7aaf51cbea8eb92ae30757489b71e9e5fb586c13d05c8f8`  
		Last Modified: Wed, 05 Oct 2022 16:48:12 GMT  
		Size: 114.1 MB (114111336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b080bef5679587f3e603ac80475d92a17a98ba240f0654ae4670fcb13877b15b`  
		Last Modified: Wed, 05 Oct 2022 16:48:01 GMT  
		Size: 4.0 MB (4034097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8-jdk` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:984ad0755704b75eb8b5d536c73dbfde4c86961f8f0ed07b595f2d47eb9ea6c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161144523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3fc60e4c97095c689feeb20be25ef41fe000a6d3c517694df86d8931d962201`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:57 GMT
ADD file:b1fcc8690fce8195995c8eab6b853225d65017d69692537273760bf84bfb72ec in / 
# Tue, 04 Oct 2022 23:52:59 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:15:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 07:15:44 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:15:45 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.1
# Wed, 05 Oct 2022 07:15:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='55eb440eedc331081012664e18b4640988a210d6443289410662ff03c0b2bf05';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='7b9da287bd3c77142a1b3e42e0ff3aa3ce5ad9aeb9ae81e4894a742fe08c057f';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='b748ef07a800b4f12ade9337e4f3e42ee5207e57e688367ab0dd978ebd1876ea';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='a87652c8150390777aa98bbe6452788522d01fd0a68ab3133663191a9cd32555';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 07:15:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 07:15:55 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 07:16:28 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:29c30188ad5f0c76a8b336bfa488a1bdf199dc8127ed81e4051c1c71d4da8f87`  
		Last Modified: Tue, 04 Oct 2022 23:54:34 GMT  
		Size: 28.6 MB (28643466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a8cc7473330bd6fbc22731594f4d1fd2b17b44ebdd2045c922739d6b0f83c7`  
		Last Modified: Wed, 05 Oct 2022 07:33:32 GMT  
		Size: 12.1 MB (12146856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e61471ecb590e99325925c3666e60677ec4896cc294ad3176313b779d879ca6`  
		Last Modified: Wed, 05 Oct 2022 07:33:39 GMT  
		Size: 116.0 MB (115997371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bfd257e7efe3e0a19e0e279a988fec3abfeb55e63229c4200e234d19f77807`  
		Last Modified: Wed, 05 Oct 2022 07:33:30 GMT  
		Size: 4.4 MB (4356830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
