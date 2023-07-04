## `eclipse-temurin:20-jre`

```console
$ docker pull eclipse-temurin@sha256:0babfb19f29d5d2f606cab236bcdb2d2857376adf159c8008e6b1680cef2ddd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-jre` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:55694de6d6d67e083dfed263d2132c047cdcd70884471fee9172b26a8378a578
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97557123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72757ff3c85e0900f8c117fec53fa73a37a1766253d9ccbca6de52e7ce36a0d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:15:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:15:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:18:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:19:15 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Fri, 16 Jun 2023 02:19:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4b04fcfabf833403cc74dd19105a387563f9ff0fef975c4101f3d74c53eb7745';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_aarch64_linux_hotspot_20.0.1_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='daacf24c15bf7f38a957a98a312911a36ba7f7d97004920a7875791f20e8e1ed';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_linux_hotspot_20.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:19:42 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857412f02e8d49bb7e247b45ce86ce6378bd0bc5e8533e1fffa2a6e7a93aab46`  
		Last Modified: Fri, 16 Jun 2023 02:23:30 GMT  
		Size: 17.0 MB (17040964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9799ab5b2493ba046e5a1ff28cbdb586aa6e04e91dee517ed5bac52399d7ddf3`  
		Last Modified: Fri, 16 Jun 2023 02:25:00 GMT  
		Size: 50.1 MB (50084960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abdbbdff48887dbb7554cc17454611e1f62c1ff8f47a74086ca1c2b01007643`  
		Last Modified: Fri, 16 Jun 2023 02:24:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:8b6d0a7ddfba10d7dd12230473f5b01a7e5c9192520c969f0c1735743b713160
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96170847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8120c519ec2f6893429b9ca964757e8a893c62a9e675ed6038de8f7809c748`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 15:34:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 15:35:22 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Tue, 04 Jul 2023 15:35:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4b04fcfabf833403cc74dd19105a387563f9ff0fef975c4101f3d74c53eb7745';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_aarch64_linux_hotspot_20.0.1_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='daacf24c15bf7f38a957a98a312911a36ba7f7d97004920a7875791f20e8e1ed';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_linux_hotspot_20.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 04 Jul 2023 15:35:45 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f85d89e7da0f3af0f527e7300cced784d0ba64249b8c376690599d313cb056`  
		Last Modified: Tue, 04 Jul 2023 15:39:09 GMT  
		Size: 18.5 MB (18466568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45953d25a53f34169be70bf8fc143e66c68cc46d47629b1b76b28be22647c9a9`  
		Last Modified: Tue, 04 Jul 2023 15:40:26 GMT  
		Size: 49.3 MB (49313108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3654c299169c0f815629af51518c775817d09dd04da9a3bfa510cfa63f12bc`  
		Last Modified: Tue, 04 Jul 2023 15:40:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:f603763b2048fa67f3ddc93a9ab3f532b115f6de37edd7fa5dff11eba4634609
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1504948544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278d2b3f05a15e4ae636d2f5ceadc2f9a66820bed6e5331ef49e48664837de2a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 01:00:36 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:05:38 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 01:06:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2501a8de966d460663959ebf53b37a9487b884766c52a4e324e5047010a539`  
		Last Modified: Sat, 24 Jun 2023 01:31:34 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3fd103c006e24c2f5106cfef71dd48b1c24a6566ec4da658bf062a9a1ddd1b`  
		Last Modified: Sat, 24 Jun 2023 01:33:34 GMT  
		Size: 78.4 MB (78370565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa01d9af7ccbaad7298d3052563fb678418cea8c57e2ad566e836ccbd9ebfe5`  
		Last Modified: Sat, 24 Jun 2023 01:33:24 GMT  
		Size: 276.5 KB (276502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:ab0a0c0e3bbd744788d12f8d24b0f48aa0a21ae07529c50dbeed827675a6bb3b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1732447228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d47d7bcd60044c17dc0561b61af1a3fe920e021472007ee2a0fb247cefb89af`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 01:02:19 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:06:57 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.1_9.msi ;     Write-Host ('Verifying sha256 (2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '2fe49a1545c1f478fae75de7cdbdec8f4301e9917ff3d4598512994205a0cd94') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Sat, 24 Jun 2023 01:07:27 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cc725e51be377d486df843039f1371f7e90bc8e29500b65bf085b11bb56247`  
		Last Modified: Sat, 24 Jun 2023 01:32:12 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8fe5a8a0ba9db4a11398eb6c6f9e34660f149e1dcbd6b8e3ce0c2ada53509e`  
		Last Modified: Sat, 24 Jun 2023 01:33:54 GMT  
		Size: 78.4 MB (78385518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e14e24dd4591557a3d0ff1e49a3086dca539e7a04660dec361d87347a30494`  
		Last Modified: Sat, 24 Jun 2023 01:33:44 GMT  
		Size: 3.3 MB (3322098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
