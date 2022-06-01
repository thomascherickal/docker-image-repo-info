## `ibm-semeru-runtimes:open-18.0.1.1_2-jre`

```console
$ docker pull ibm-semeru-runtimes@sha256:1df20065780e5104aa5b377bbc3d1ad15e9f4b473dc8b9cf607298e44558e6d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm64 variant v8
	-	linux; s390x

### `ibm-semeru-runtimes:open-18.0.1.1_2-jre` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:710a28be9dc5b68b6f23a13f8afc6e0bcca1bfa4d0acc959cc2cdc3cb7c29d6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93285518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a36394485deda1ccab62a9406702e6e20dfec249166cefe2bb05778f80fa0e61`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:28:52 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 May 2022 23:54:33 GMT
ENV JAVA_VERSION=jdk-18.0.1.1+2_openj9-0.32.0
# Tue, 31 May 2022 23:54:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='86bf05dae9510bd0679bf7489378b1411cf816885adbde7108d52e3b85d76d84';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b5e650847c39efa65e294df46c073091e9089579decdb125867af8e4bae2cb5';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='761807f0c13500b1e94824928050c3485932cb596e2a499935f67b734c644c97';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='e2b2c19e2db157ceaf1151e88bec94c0e197a593a37a7abf0ce6ae92ab320b45';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 May 2022 23:54:38 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 May 2022 23:54:39 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 May 2022 23:55:15 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce33c7cb386794b97371bf23d6db512379e04036ae033b076a599f51f6416b6`  
		Last Modified: Fri, 29 Apr 2022 23:33:40 GMT  
		Size: 15.9 MB (15897301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49662331becf871941352d50f34fc6666e07343bc62ba920c159c7d1a3c7426`  
		Last Modified: Tue, 31 May 2022 23:59:07 GMT  
		Size: 45.7 MB (45686294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51511b62a0b5e581bf8c9d24fc98ee4b972ff6e4cafb31acd1fa1ae27eef56b`  
		Last Modified: Tue, 31 May 2022 23:59:00 GMT  
		Size: 4.5 MB (4532535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18.0.1.1_2-jre` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:7879ec5475b0918390eda417eaf892078be3927480741c66fc757794eb5345ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (93998604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8ba7ed8baf13229894cb5df236fa561a1765b1592b9ea500b36803080fceccf`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:22:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:22:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 May 2022 23:49:18 GMT
ENV JAVA_VERSION=jdk-18.0.1.1+2_openj9-0.32.0
# Tue, 31 May 2022 23:49:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='86bf05dae9510bd0679bf7489378b1411cf816885adbde7108d52e3b85d76d84';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_aarch64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b5e650847c39efa65e294df46c073091e9089579decdb125867af8e4bae2cb5';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_ppc64le_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='761807f0c13500b1e94824928050c3485932cb596e2a499935f67b734c644c97';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_x64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='e2b2c19e2db157ceaf1151e88bec94c0e197a593a37a7abf0ce6ae92ab320b45';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jre_s390x_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 May 2022 23:49:24 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 May 2022 23:49:24 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 May 2022 23:49:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1002590b38d45b986e07362b8635ab8cb57c796f0a8ae1a3c707970fe0200e54`  
		Last Modified: Fri, 29 Apr 2022 23:25:27 GMT  
		Size: 15.7 MB (15739301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316efa157b565037bb496899f8420efaf1eae415ee86156f52acbd28e1eb23db`  
		Last Modified: Tue, 31 May 2022 23:52:01 GMT  
		Size: 46.3 MB (46333691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9801c748930ad6c6caf2895278961c66972dacb7f40ab00130f9347312db77`  
		Last Modified: Tue, 31 May 2022 23:51:56 GMT  
		Size: 4.9 MB (4860195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
