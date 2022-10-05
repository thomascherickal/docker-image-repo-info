## `ibm-semeru-runtimes:open-18.0.2_9-jre-jammy`

```console
$ docker pull ibm-semeru-runtimes@sha256:8d15659b78f20d15e4061a25b084f3ff92dfaba602367fe51215abc9304835b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `ibm-semeru-runtimes:open-18.0.2_9-jre-jammy` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:948b00ee19ac20d3cf42fd9ac333e5a1880a8234424c786e938c35abadb33525
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95343472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac587057919ce226f671441a80c66243c8e52b0a8367d64a1cc9528339d678fd`
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
# Wed, 05 Oct 2022 17:32:22 GMT
ENV JAVA_VERSION=jdk-18.0.2+9_openj9-0.33.1
# Wed, 05 Oct 2022 17:32:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cf42a289c53e6098223223326cd21a152d7102859030e23c52287d82d6d9560e';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='57726d73c644107de26fe6c252a58f477e691b9aa81de0c23251318f87aa621b';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4fb19cedab5967359991b9bcb3be09744fc9ac027d0b773870ee7f7aaf539666';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='74a0bd8e3bd1504df48e1ee83b997ac9993f5d1e8371cd673afb01b9ce611c7c';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 17:32:28 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 17:32:28 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 17:33:03 GMT
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
	-	`sha256:1e20df4e43fa6bc533e83225488bcbe25c5bb75d45bbd556ebd28a47370de90a`  
		Last Modified: Wed, 05 Oct 2022 17:39:36 GMT  
		Size: 48.0 MB (48016074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a07e0f3ed846395d7153c84868763ab03fc1f0a128d5108ebff57a76d229acf`  
		Last Modified: Wed, 05 Oct 2022 17:39:30 GMT  
		Size: 4.8 MB (4794434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18.0.2_9-jre-jammy` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:c6e9ffe6266911511ad67707de782081f97fa00a4600ef58867fb6b5eb180a48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91163654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fcc13478fa96e7e581e6ffae419d2fe53d124c10b9e27ed0bdd6666603a2c`
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
# Wed, 05 Oct 2022 16:44:49 GMT
ENV JAVA_VERSION=jdk-18.0.2+9_openj9-0.33.1
# Wed, 05 Oct 2022 16:44:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cf42a289c53e6098223223326cd21a152d7102859030e23c52287d82d6d9560e';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='57726d73c644107de26fe6c252a58f477e691b9aa81de0c23251318f87aa621b';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4fb19cedab5967359991b9bcb3be09744fc9ac027d0b773870ee7f7aaf539666';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='74a0bd8e3bd1504df48e1ee83b997ac9993f5d1e8371cd673afb01b9ce611c7c';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 16:44:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:44:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 16:45:30 GMT
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
	-	`sha256:1c2b956807c1acaf96044a2bddc72d48c6724ff3e5b1013d188b78ba32a3c031`  
		Last Modified: Wed, 05 Oct 2022 16:53:40 GMT  
		Size: 46.2 MB (46239950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ed305714725191c4c1e3e0694552c7244eaa59e4cda7c965f2323a942e9a80`  
		Last Modified: Wed, 05 Oct 2022 16:53:34 GMT  
		Size: 4.5 MB (4477326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18.0.2_9-jre-jammy` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:88c9aa8643dd0af565b91ab30dfd1b531520a6838bd568f48b54776813ce769d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92806490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a0da819be0d4effc1963200cf359d7c583a558cc323990dcc39365f8ac8c78d`
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
# Wed, 05 Oct 2022 07:30:39 GMT
ENV JAVA_VERSION=jdk-18.0.2+9_openj9-0.33.1
# Wed, 05 Oct 2022 07:30:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cf42a289c53e6098223223326cd21a152d7102859030e23c52287d82d6d9560e';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='57726d73c644107de26fe6c252a58f477e691b9aa81de0c23251318f87aa621b';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4fb19cedab5967359991b9bcb3be09744fc9ac027d0b773870ee7f7aaf539666';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='74a0bd8e3bd1504df48e1ee83b997ac9993f5d1e8371cd673afb01b9ce611c7c';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.2%2B9_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_18.0.2_9_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 07:30:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 07:30:49 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 07:31:25 GMT
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
	-	`sha256:c0b70dc7983b94f3e126dd0b508c0b13e4da08926f942615f1fb0f9945b0dcde`  
		Last Modified: Wed, 05 Oct 2022 07:37:24 GMT  
		Size: 47.1 MB (47108192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae2adcd422745b779668e6efd0e652dd8e51b8946c0774117e89043b0d5b725`  
		Last Modified: Wed, 05 Oct 2022 07:37:19 GMT  
		Size: 4.9 MB (4907976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
