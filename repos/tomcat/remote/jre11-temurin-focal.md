## `tomcat:jre11-temurin-focal`

```console
$ docker pull tomcat@sha256:de0006d3a3828514d04478f58fe7d93abaab0be84cb83dfe02e82f60c0909bf2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre11-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:b03441e74868e7f190ac038d1ce87d2470706e9dbd92267489e86da30ee07c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100688351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f6c89e8edf361b6ffc2bc9f1d56798f692bd1d58123ca245ae3a3a51f046c6f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:19:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:19:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:19:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:20:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:22:25 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:23:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:23:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 21:33:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:33:19 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:33:19 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:33:20 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:33:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:33:20 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:33:20 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:33:20 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:33:20 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:33:20 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:33:21 GMT
COPY dir:bbb865cd15a41d689eaf2b2dc3f054530b60c39649fdbe8dbdb89b408821ef3f in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:33:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:33:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:33:27 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:33:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aaad0dc3faf013330a30e044ebf8fcfe3d73ac2c342d3879297cd427cf888bc`  
		Last Modified: Thu, 11 Aug 2022 19:30:14 GMT  
		Size: 12.6 MB (12550796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715b92e9cbaa1bb2a8be80d0457f3f38125fd0568f518c23def47d3689f0cc6e`  
		Last Modified: Thu, 11 Aug 2022 19:34:27 GMT  
		Size: 46.5 MB (46496205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711a05e44c7ee1e2068339f1d1fd3ec2387189043c8775dbc1a8ef6fda9f9bdf`  
		Last Modified: Thu, 11 Aug 2022 19:34:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ab233b7c074623ddce8d4fc25dfffa272996576108b8e456dd40a36c55758e`  
		Last Modified: Thu, 11 Aug 2022 22:01:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ee8bd7a8aa6d9a95f6cce1c24319ef7cc1de2e22af21adbc736be662aec9f`  
		Last Modified: Thu, 11 Aug 2022 22:01:03 GMT  
		Size: 12.6 MB (12632716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c98ec1d3652939378fcc4a771086428ebf0154d0fa81fcbb8d6081a5d7704d5`  
		Last Modified: Thu, 11 Aug 2022 22:01:03 GMT  
		Size: 435.6 KB (435576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4bf3cb598dac46f126bfdf6a1252fef4e3d87c28634ca79d17d49e976cad2f`  
		Last Modified: Thu, 11 Aug 2022 22:01:02 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:b99512aa4399160e782a9dacf57da342abc4582325167142fe14f66626a00e56
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94214989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91588627668a58ef4690804263d77c92be4249965125a5093b17055c5598d0a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:45 GMT
ADD file:7de7e2c2eb5b05b2449f1e73da223081e27d073990c979ec73afd1893c58c551 in / 
# Tue, 02 Aug 2022 01:40:45 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:57:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:57:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:57:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:57:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:59:28 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:00:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:00:18 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:15:47 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:15:47 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:15:48 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:15:48 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:15:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:15:48 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:15:48 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 20:15:48 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 20:15:48 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 20:15:49 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 20:15:49 GMT
COPY dir:744d67817430cb7c68638550d1a68eef42167ef244606c868ea83a376896bea6 in /usr/local/tomcat 
# Thu, 11 Aug 2022 20:15:56 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 20:15:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 20:15:58 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 20:15:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:de6f11ffeeef9e471776e52baf8cc454a1249e8caf2d8944a5b0387143608310`  
		Last Modified: Tue, 02 Aug 2022 01:43:13 GMT  
		Size: 24.6 MB (24589273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a62569004c1e56a6607db95d1fa179d7810f9f0158dc151120981d8941ccdc`  
		Last Modified: Thu, 11 Aug 2022 19:05:37 GMT  
		Size: 12.0 MB (11955821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2619f5871138d2039668c28cb260a762016f49126d69798db4803d2b978ae70b`  
		Last Modified: Thu, 11 Aug 2022 19:08:10 GMT  
		Size: 44.7 MB (44674788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b8e23504feda579e36920993af0a76b26464c8c6cdedc9b174f3a735342f08`  
		Last Modified: Thu, 11 Aug 2022 19:08:02 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8e1781074a1079a7ed096ae047167970eddc9b848f9dcffa95d81bc74a1f8b`  
		Last Modified: Thu, 11 Aug 2022 20:49:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a6dbbfa2d9961af25d7eeae6a4b649ee36318983bf8f53bc38929034556f20`  
		Last Modified: Thu, 11 Aug 2022 20:49:59 GMT  
		Size: 12.6 MB (12583159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863751af67da0352ce96c3adeb3218200a5c2352433cd82a8af6b2df135232eb`  
		Last Modified: Thu, 11 Aug 2022 20:49:59 GMT  
		Size: 411.5 KB (411487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6904c29468363e1a90b4c820358b16f7a87d6e51d911ca4c0e2a148a5d019377`  
		Last Modified: Thu, 11 Aug 2022 20:49:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:f459ff9cd4ffced1095ee378a0740eefa746514472c18a28cb36b1ba82881965
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97275814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa284036edfbb97c2f915af70c5c110354e1778dbca4f32553d48db6eec4bd54`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:39:54 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:39:55 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:39:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:40:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:42:27 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 18:44:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 18:44:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 21:02:22 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:02:23 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:02:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:02:25 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:02:26 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:02:27 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:02:28 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:02:29 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:02:30 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:02:31 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:02:33 GMT
COPY dir:a2ce057b9b7c299f793a0f63ae3343c0fae69e630ab0a60fc85c6d6e11a98df0 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:02:39 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:02:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:02:42 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:02:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eedefaaae9298d2004182d1bfde0bea8b977b933e65bb038764a6677dd0632f`  
		Last Modified: Thu, 11 Aug 2022 18:52:30 GMT  
		Size: 12.4 MB (12408927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc82df1f27f3923186b743c0c3839b222c478e1ee4bd080f542c0f070e81f9bd`  
		Last Modified: Thu, 11 Aug 2022 18:56:05 GMT  
		Size: 44.8 MB (44825505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fdfd2ae755d854156bee309a3ecaed3c1a1e14b3b9dca8096e6c311cd84cb9`  
		Last Modified: Thu, 11 Aug 2022 18:55:58 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0a7e887a09c3dff2b490e5a45521d9da5e95183dc154180832daecbca5b7a7`  
		Last Modified: Thu, 11 Aug 2022 21:49:24 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd75501e94f2f73a192bfd9fe685d9af78415d16b826e9b765e65fe1f73458c6`  
		Last Modified: Thu, 11 Aug 2022 21:49:25 GMT  
		Size: 12.7 MB (12650498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77546dbd843669bb1c4764ddf29f181d8a6ae73cc52bc9b238121fed190c413f`  
		Last Modified: Thu, 11 Aug 2022 21:49:24 GMT  
		Size: 198.8 KB (198784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:f171ec2aa0b41bf6fda1832d61ff8b9a47851820ca8b9302ca70f9982d7cc665
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101399129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecf3c0132e699bceb0712c4d54f4ce65168c87b55776d3e3a196d8270113e369`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:01 GMT
ADD file:75dd7889d4feb83b8504153b5ea6873e4ab0e616a4f4489ea81fd055b6ce9def in / 
# Tue, 02 Aug 2022 01:31:03 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:16:48 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:16:48 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:16:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:17:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:21:11 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:22:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:22:56 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 21:04:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:04:55 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:04:56 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:04:57 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:04:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:04:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:04:58 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:04:58 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:04:59 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:04:59 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:05:00 GMT
COPY dir:82f953adc89f2bfc8fee418cf499ede44235ad44cd416d15f2d15be75251030d in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:05:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:05:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:05:10 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:05:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bf47d2be67f1a301865e78e8f78cc69c55dcc389921b4ba187dc0d333cbfd63b`  
		Last Modified: Tue, 02 Aug 2022 01:33:30 GMT  
		Size: 33.3 MB (33295352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b71b197bc93f31065ddd7245d2113f873ba097b56794545d788a6630da2b0d`  
		Last Modified: Thu, 11 Aug 2022 19:33:13 GMT  
		Size: 13.1 MB (13083533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb62ec3ebd41d4e27c17c8861ac5fedecf8dc68927ab7b1bc8e19d193c30ce8`  
		Last Modified: Thu, 11 Aug 2022 19:37:43 GMT  
		Size: 41.9 MB (41885429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6e3d1c05ac2ba753f3643b7fad5de182ff693c24edbff5b69d9b86de50dcc6`  
		Last Modified: Thu, 11 Aug 2022 19:37:33 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc3ab7f1b80def57fe68b0add1f59a6e59b7598013ceefbc6527bf49dd73fa0`  
		Last Modified: Thu, 11 Aug 2022 21:45:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a41675abe2d6c8ad16027986b0fab5f88be75ea2b06514b231fbf73f8f0b0dc`  
		Last Modified: Thu, 11 Aug 2022 21:45:37 GMT  
		Size: 12.7 MB (12673276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2059b1fd590d8c9898805eec7a77972b2fc735d6a831e06e4195798a2eb5225c`  
		Last Modified: Thu, 11 Aug 2022 21:45:36 GMT  
		Size: 461.1 KB (461077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b252163f514e1e74dd2a66d92209fb9225fa4ad373e56463dd0f147c3767e9`  
		Last Modified: Thu, 11 Aug 2022 21:45:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:e2449d5da158b785c8afe06354200b6240ce6bd26a6d0643d71c00131ecad568
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.9 MB (92909486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af2ca5101f6238abc7c02c2b96159ca834191adf8661226d89f24270d161525`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:41:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:41:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:41:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:41:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:41:56 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 18:43:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 18:43:06 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 19:52:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 19:52:40 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:52:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 19:52:42 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 19:52:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 19:52:43 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 19:52:43 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 19:52:44 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 19:52:44 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 19:52:45 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 19:52:46 GMT
COPY dir:3b2f63b0db85ebd44edaad15e1674d3d4f2b1f9b72037c8f3c261ef6348836f9 in /usr/local/tomcat 
# Thu, 11 Aug 2022 19:52:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:52:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 19:52:56 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 19:52:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9ad20629597c47f9394c5a3d24300cbb87398097779003382877d6fe4e2625`  
		Last Modified: Thu, 11 Aug 2022 18:49:20 GMT  
		Size: 12.3 MB (12300520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f244a8e5df368df664a5f5359697fb2d04b1f34d43b92c438e2b323c78d1839`  
		Last Modified: Thu, 11 Aug 2022 18:50:08 GMT  
		Size: 40.5 MB (40479813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb1becaee3ed83d32fd9a56f7a612cd4b321520912e63284df72a4fd786dc9b`  
		Last Modified: Thu, 11 Aug 2022 18:50:03 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace5b93085eb59a69c99dcb7062fdbf7e005238331270b99ab8d6b0af876e629`  
		Last Modified: Thu, 11 Aug 2022 20:16:01 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7e3510a2b19a809f17140f63ed40cb88be6fba262b55b83500d2feaf18adb8`  
		Last Modified: Thu, 11 Aug 2022 20:16:03 GMT  
		Size: 12.6 MB (12645958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037e2f2fcc77239c470239c4924844be56e2f2e86614b3274d0dff5be06676c4`  
		Last Modified: Thu, 11 Aug 2022 20:16:01 GMT  
		Size: 437.4 KB (437371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02c86036e2ff414fc3711897a954c5086161d5ec45d456f9c0af010284b5a8d`  
		Last Modified: Thu, 11 Aug 2022 20:16:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
