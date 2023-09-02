## `eclipse-temurin:20-jre`

```console
$ docker pull eclipse-temurin@sha256:c953fd5d9c18d263a31bd223d338f48ebde598a92d36d4425172462cb31c7e68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1906; amd64
	-	windows version 10.0.17763.4737; amd64

### `eclipse-temurin:20-jre` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:199ce96801ae90961fc0dde2a0848ed64f5c8e95dc40bb8bbc7bea3ddceae523
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.2 MB (98197596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf8fa2472af3de9bc772eac721538521611a93073660e63655719a392dd53ba`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:37:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 00:37:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 00:37:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Sep 2023 00:39:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:40:12 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Sat, 02 Sep 2023 00:40:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='63a730d5a3b6d21d31f7cba15dc44b019a8a4d8652e13acec45040f98584112c';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_aarch64_linux_hotspot_20.0.2_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e3592e86290c192804d9c6b5035d42cc32cf04141d1c0b9d1ecb67739826c8c5';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_x64_linux_hotspot_20.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Sat, 02 Sep 2023 00:40:39 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 02 Sep 2023 00:40:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Sep 2023 00:40:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cabec57fa3613116cbc641e1159ee0a7bde39ef9b3046a4e2122a5b390b7db5`  
		Last Modified: Sat, 02 Sep 2023 00:42:56 GMT  
		Size: 17.5 MB (17456268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b91e3900e2ab1e7faf5a89e895d9e5a62071a1610fc0fba34e95b57f6a44d2`  
		Last Modified: Sat, 02 Sep 2023 00:44:08 GMT  
		Size: 50.3 MB (50301458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4916ed74213c483e7fca027eb8efa47ed234dfd8093d2fa747b90e638bd80186`  
		Last Modified: Sat, 02 Sep 2023 00:44:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6f084f3319019a3ab80498ecd00dd52617bf7678fd2ad9eaebc14851bbfbaf`  
		Last Modified: Sat, 02 Sep 2023 00:44:01 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:5b19477bbc6c1dce6c997a01a2cb8aff3e5bbb9bf48379e3d83df09d26ae4171
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96766309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b8a216cfb8115a9df71a81668db4a9fc7c3a184755255107a6d44350087cf2`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:28:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 01 Sep 2023 23:28:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 23:28:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Sep 2023 23:30:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:30:45 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Fri, 01 Sep 2023 23:31:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='63a730d5a3b6d21d31f7cba15dc44b019a8a4d8652e13acec45040f98584112c';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_aarch64_linux_hotspot_20.0.2_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e3592e86290c192804d9c6b5035d42cc32cf04141d1c0b9d1ecb67739826c8c5';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_x64_linux_hotspot_20.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 01 Sep 2023 23:31:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 01 Sep 2023 23:31:08 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Sep 2023 23:31:08 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bccb525aef23b375cbcff84a9e7861c44ea0c0abcb727d4a15c43403b3bf22`  
		Last Modified: Fri, 01 Sep 2023 23:33:13 GMT  
		Size: 18.9 MB (18859695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0884b2bdc88a62ed164cffd6e4137bf7a8c0ac950f170eac01948d545696ff05`  
		Last Modified: Fri, 01 Sep 2023 23:34:16 GMT  
		Size: 49.5 MB (49512743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2778f1dc4e012c7465485e872d39b745aa554082bb509e987e6aa322e8f4cfb`  
		Last Modified: Fri, 01 Sep 2023 23:34:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9341a4fbf6b52a63c590f5bcab915aa9fc14c2a3e95e7b510ae6b6d5901a58a8`  
		Last Modified: Fri, 01 Sep 2023 23:34:09 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre` - windows version 10.0.20348.1906; amd64

```console
$ docker pull eclipse-temurin@sha256:e097ce4c4f22de1bac4383d56a413bc0fddbe32f6206c1fc610c29026fab0c7b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1876288828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f76faf03ec47aeb8e3257734a9b780fbde8a8aab67f1b6abcd8ec4816d2bea`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:02:08 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Thu, 10 Aug 2023 00:08:23 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.2_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.2_9.msi ;     Write-Host ('Verifying sha256 (0217ba025c5ac579982a80791d4637e2b4b6afb14de522fff2b818d0203d4cea) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '0217ba025c5ac579982a80791d4637e2b4b6afb14de522fff2b818d0203d4cea') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Thu, 10 Aug 2023 00:08:49 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c8a6069c3aae0f69ff18f47362cfb218924daef52e27c046f15f4cbfb40220`  
		Last Modified: Thu, 10 Aug 2023 00:27:53 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7779203ea9bd60f2b9181fd973d2af61e4f33192399659e9ab5ede008c9f7a`  
		Last Modified: Thu, 10 Aug 2023 00:29:55 GMT  
		Size: 78.6 MB (78644673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7980caa8dbf8321ec85630f8a0c7715be58503ea719e8221d5d57a0e4e2306`  
		Last Modified: Thu, 10 Aug 2023 00:29:43 GMT  
		Size: 277.5 KB (277534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jre` - windows version 10.0.17763.4737; amd64

```console
$ docker pull eclipse-temurin@sha256:469d5d85500e4055773f0ead7d18dfabdbd25f8244e7824bb96c4012c7a2d229
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077954025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad420b6ff2b36d1258d325b124d0104d0520fb748e36d0221d2503f13485cdc`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 00:03:51 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Thu, 10 Aug 2023 00:10:09 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.2_9.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.2%2B9/OpenJDK20U-jre_x64_windows_hotspot_20.0.2_9.msi ;     Write-Host ('Verifying sha256 (0217ba025c5ac579982a80791d4637e2b4b6afb14de522fff2b818d0203d4cea) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '0217ba025c5ac579982a80791d4637e2b4b6afb14de522fff2b818d0203d4cea') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-20' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Thu, 10 Aug 2023 00:11:02 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'java --version'; java --version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d67511feb7dd186e3a60bc9e347fddab421a33169b1eaa67a701c13be1e589`  
		Last Modified: Thu, 10 Aug 2023 00:28:33 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8669d2774340d833ee7ca5a9bb86edbe8dcd08165ea861c32d034d6e411c87cc`  
		Last Modified: Thu, 10 Aug 2023 00:30:15 GMT  
		Size: 78.7 MB (78706603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e743b42e31df6ae0a5ba78078d46fdabe5ad0c7e9f8140c270512edd80e34e5`  
		Last Modified: Thu, 10 Aug 2023 00:30:05 GMT  
		Size: 3.3 MB (3289319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
