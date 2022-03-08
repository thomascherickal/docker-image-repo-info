## `tomcat:10-jre17-temurin`

```console
$ docker pull tomcat@sha256:cc0bb3d6f3ee4d1ec5c105da28b76fc3b998d7d71695279fcb1c8cc265b0ec42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:10-jre17-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:ccf49d155fab48b25819b2acb0792310072c73db5c988e745271f591a6320cc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.3 MB (110297191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:438609ff6125ffe4378d806cd4bb78ced52772781eb7919142fec42bc6dd5367`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:23:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 07 Mar 2022 19:28:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:28:27 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Mon, 07 Mar 2022 19:28:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:28:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:28:49 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 07 Mar 2022 20:21:33 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Mar 2022 20:21:33 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 20:21:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Mar 2022 20:21:34 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Mar 2022 20:21:34 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:21:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:21:34 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Mon, 07 Mar 2022 20:21:34 GMT
ENV TOMCAT_MAJOR=10
# Mon, 07 Mar 2022 20:25:25 GMT
ENV TOMCAT_VERSION=10.0.17
# Mon, 07 Mar 2022 20:25:25 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Mon, 07 Mar 2022 20:25:25 GMT
COPY dir:bb884af2f1e69e357c9da22bf5025dde0c4dbb65c73b07187fa2f9d9d17d1d13 in /usr/local/tomcat 
# Mon, 07 Mar 2022 20:25:30 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 20:25:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Mar 2022 20:25:31 GMT
EXPOSE 8080
# Mon, 07 Mar 2022 20:25:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af0b6ae3bc451c2e0d6207a6e51c3fa2470fc260a62d00102a099ed349bf9da`  
		Last Modified: Mon, 07 Mar 2022 19:32:08 GMT  
		Size: 19.8 MB (19772631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6559941aa35988a8caa0109489a820d7f8c7571d05d202cf7077a7fd767ca`  
		Last Modified: Mon, 07 Mar 2022 19:33:09 GMT  
		Size: 47.0 MB (47038144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06a11475ff2bfcfb1c294f660ea7f77579393b570ba5a06a78e5fa326c0bc57`  
		Last Modified: Mon, 07 Mar 2022 19:33:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc83147ed62bb71e8f0fbcf9250e43781cdde7e7e1778d89bfcd642a24ccc81`  
		Last Modified: Mon, 07 Mar 2022 20:48:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c2297618e434cd994c0d330a9f7f2518b6fecdfe8a09f1c2475142460b15f1`  
		Last Modified: Mon, 07 Mar 2022 20:51:16 GMT  
		Size: 12.6 MB (12564977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63dd81d1ec5d189ef2e6f0777127220b9da9abe6c2f5b766b0f211e7c326eb9`  
		Last Modified: Mon, 07 Mar 2022 20:51:15 GMT  
		Size: 2.4 MB (2355226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5419365043fcc0770db3785a15c6e284c6e6eab7678b40d3bbcc07901b7cdf`  
		Last Modified: Mon, 07 Mar 2022 20:51:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:61481a061937140ad4bc3afa00170824517b96677c8595aa4b594d4b5e980406
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100820556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e09500accf156ad1ed72ac0bd9eef35ef221816a04534ca4c2ab01a8fa7106`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 21:21:31 GMT
ADD file:984d3d8b31abd025bb9be52f42d60245a76b1ee991f286db819ae204da45390c in / 
# Thu, 03 Mar 2022 21:21:32 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 04:40:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 07 Mar 2022 20:01:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 20:02:12 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Mon, 07 Mar 2022 20:03:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 20:03:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 20:03:05 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 07 Mar 2022 20:57:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Mar 2022 20:57:56 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 20:57:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Mar 2022 20:57:58 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Mar 2022 20:57:58 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:57:58 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:57:59 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Mon, 07 Mar 2022 20:57:59 GMT
ENV TOMCAT_MAJOR=10
# Mon, 07 Mar 2022 21:04:10 GMT
ENV TOMCAT_VERSION=10.0.17
# Mon, 07 Mar 2022 21:04:10 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Mon, 07 Mar 2022 21:04:13 GMT
COPY dir:e03cb6cd1357b2f3f6a86ce5492d01d5cadc6674a3aae3ba6a79088e75259fed in /usr/local/tomcat 
# Mon, 07 Mar 2022 21:04:23 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 21:04:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Mar 2022 21:04:27 GMT
EXPOSE 8080
# Mon, 07 Mar 2022 21:04:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:12a77aaceb8aa1438ebb61cb4904d74fc225cfa20464a060980580674a0a31e9`  
		Last Modified: Thu, 03 Mar 2022 21:25:09 GMT  
		Size: 24.1 MB (24073718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72a7de35baa71c7eab0c19d4b3b81c8f5e7b807c9088977982926a9f3678ff1`  
		Last Modified: Mon, 07 Mar 2022 20:09:25 GMT  
		Size: 19.2 MB (19194475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4568ea7bcaa0a9dfa01125b71d1fc33b868323a4fea2fa8e1cd17053e325ec14`  
		Last Modified: Mon, 07 Mar 2022 20:12:39 GMT  
		Size: 44.6 MB (44611465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9150deb9b872f5d8bfefce0d406fcfe325ef05aec9b5e7fc4fab8af1997ad45`  
		Last Modified: Mon, 07 Mar 2022 20:12:10 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9078c1b52c4698e6e3d13529986ce55684818755960d41bb52049155dde2300`  
		Last Modified: Mon, 07 Mar 2022 21:39:40 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54805fefa5959dab3df27f82d0c6e173cabe84d21b9ead37321638336206cad`  
		Last Modified: Mon, 07 Mar 2022 21:42:37 GMT  
		Size: 12.5 MB (12515319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a170229435f4eff8c0ff46cd123597b55ca401569375919646be845c216fd21e`  
		Last Modified: Mon, 07 Mar 2022 21:42:32 GMT  
		Size: 425.1 KB (425114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cbbb199f548bf5d48e9a8b1ccd04f311b694ff589187a116532b052d08a80a`  
		Last Modified: Mon, 07 Mar 2022 21:42:32 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:662aa4a0fe9bc1ce4d27bad172e806a3ab9fb2f8057c26567b49b3d15bde5bbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105947510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c418e2e582646cddfccc06fe626c1b0af08ddc431ba5612c073d5ff98b62313`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:02 GMT
ADD file:f2fffe739729839aa17484bc4d79d33425549c5052824eac12131b16c23565d3 in / 
# Thu, 03 Mar 2022 19:41:03 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:21:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 07 Mar 2022 19:44:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:45:10 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Mon, 07 Mar 2022 19:46:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:46:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:46:07 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 07 Mar 2022 20:43:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Mar 2022 20:43:57 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 20:43:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Mar 2022 20:43:59 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Mar 2022 20:44:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:44:01 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:44:02 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Mon, 07 Mar 2022 20:44:03 GMT
ENV TOMCAT_MAJOR=10
# Mon, 07 Mar 2022 20:49:45 GMT
ENV TOMCAT_VERSION=10.0.17
# Mon, 07 Mar 2022 20:49:46 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Mon, 07 Mar 2022 20:49:48 GMT
COPY dir:679e14ed0098b387b2b0310a14bf7afdb9a5a6238054eb05845d1439c296ae86 in /usr/local/tomcat 
# Mon, 07 Mar 2022 20:49:55 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 20:49:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Mar 2022 20:49:57 GMT
EXPOSE 8080
# Mon, 07 Mar 2022 20:49:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5a7855fb0d7ae372c824d9c76be5ad2f42ce178c1910fa54a8543036b5325fd5`  
		Last Modified: Thu, 03 Mar 2022 19:42:38 GMT  
		Size: 27.2 MB (27169631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d202e3388c81be3cb43a323c27796e11c90b4661c95a9fcba928b42d5f1d4237`  
		Last Modified: Mon, 07 Mar 2022 19:49:30 GMT  
		Size: 20.5 MB (20499782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf231e790c3f5240ba9b005cdd448f8ec51c32a6ba83de1392e0e8bbff30c436`  
		Last Modified: Mon, 07 Mar 2022 19:50:43 GMT  
		Size: 45.5 MB (45484487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cfee3dfc7f10eef2ae035fc08736820363573eff3353e24d836e81209ddcd3`  
		Last Modified: Mon, 07 Mar 2022 19:50:36 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7745cf13819a18a49879dcdae5d041520e9ea1239fab7ab9ebc23dee787b605`  
		Last Modified: Mon, 07 Mar 2022 21:31:17 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c219f4b6ae85f05183796dcdb124defbe3966f8e67a8835ceda81b466b61468b`  
		Last Modified: Mon, 07 Mar 2022 21:34:22 GMT  
		Size: 12.6 MB (12581900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d77574a56e4fc259a3ae84ab425ac7a5e0ae1d9e1463c6e786fc59c410d706`  
		Last Modified: Mon, 07 Mar 2022 21:34:21 GMT  
		Size: 211.4 KB (211445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:9a8ac764b4225af56d095aadbedc6378c03893ddf9f69b4f3150489006b0ec4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113687724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acaa29318c701e5828fdcfbc0dcbca3b90a445f880c2edf9aa4a2c6409957d95`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 20:28:30 GMT
ADD file:039f04ac6c5dbbe3fb0a5eee16945cf7c5fb7565751d6bdf8ec0c1102798c1de in / 
# Thu, 03 Mar 2022 20:28:38 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:04:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 07 Mar 2022 19:30:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:32:34 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Mon, 07 Mar 2022 19:33:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:33:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:34:01 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 07 Mar 2022 20:44:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Mar 2022 20:44:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 20:44:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Mar 2022 20:44:19 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Mar 2022 20:44:23 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:44:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:44:27 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Mon, 07 Mar 2022 20:44:29 GMT
ENV TOMCAT_MAJOR=10
# Mon, 07 Mar 2022 21:00:17 GMT
ENV TOMCAT_VERSION=10.0.17
# Mon, 07 Mar 2022 21:00:19 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Mon, 07 Mar 2022 21:00:22 GMT
COPY dir:a110e35543d06a9ee322b843e388071ec9ebf09bad7e9dd37fa67ad7c7b02a4a in /usr/local/tomcat 
# Mon, 07 Mar 2022 21:00:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 21:00:59 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Mar 2022 21:01:02 GMT
EXPOSE 8080
# Mon, 07 Mar 2022 21:01:04 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a16b43de69d1e799ea2cb675e7e605db0ff3a8d692fd326fbde80a370e0676d5`  
		Last Modified: Thu, 03 Mar 2022 20:33:55 GMT  
		Size: 33.3 MB (33292195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe83d48d12b5f1315927dd21902bee72f1d10516a8c8d635cf7cc1d4768127`  
		Last Modified: Mon, 07 Mar 2022 19:38:25 GMT  
		Size: 21.7 MB (21691309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e46ee7aa9ebd09a8132e22537cff17cbb877993fde85cffcaf08ef4a70fb069`  
		Last Modified: Mon, 07 Mar 2022 19:39:48 GMT  
		Size: 45.6 MB (45621129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f41103b113a7f5af0786eff4ace385d6e1185e028a971784998649b8811cae1`  
		Last Modified: Mon, 07 Mar 2022 19:39:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1ac6a907508e47aa40dc1b89a996459f151716fdc00c2f4972d6c0411fa57b`  
		Last Modified: Mon, 07 Mar 2022 22:01:00 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47b6f72201f32f2b4f03b8f82238256dc71b1995bd36e00fc550121512c6243`  
		Last Modified: Mon, 07 Mar 2022 22:03:43 GMT  
		Size: 12.6 MB (12608510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7873064a4f732e9e5675265885a90f8fdca2becd15798ac3e9e8c55d6d0cf13b`  
		Last Modified: Mon, 07 Mar 2022 22:03:42 GMT  
		Size: 474.1 KB (474117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26504446628abadc7cee2a0b5eaffef5e7f764b0d2bafc6496b8f9238cd13506`  
		Last Modified: Mon, 07 Mar 2022 22:03:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre17-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:f42c0ef07697be0e17b5b41997d8e9fad0c65c14a2e0cbc522979f4ac2d8db08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102965039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f5056c6b490e741f2654ae66600c4ba048f7e9a1dcd59f6a4aa3fb78baf165b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:52 GMT
ADD file:3162233da685a36a9f274a7fa1d99452cab76f37e3640d38851c782ca506f75b in / 
# Thu, 03 Mar 2022 19:41:53 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 19:59:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 07 Mar 2022 19:44:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:44:45 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Mon, 07 Mar 2022 19:45:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:45:12 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:45:12 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Mon, 07 Mar 2022 20:21:54 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Mar 2022 20:21:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 20:21:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Mar 2022 20:21:55 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Mar 2022 20:21:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:21:55 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Mar 2022 20:21:55 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Mon, 07 Mar 2022 20:21:55 GMT
ENV TOMCAT_MAJOR=10
# Mon, 07 Mar 2022 20:25:53 GMT
ENV TOMCAT_VERSION=10.0.17
# Mon, 07 Mar 2022 20:25:53 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Mon, 07 Mar 2022 20:25:53 GMT
COPY dir:cc3b501e424972317aa6bb65d0c6b0c528ea16a95af4c16b98dc07b21d4d335d in /usr/local/tomcat 
# Mon, 07 Mar 2022 20:25:58 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 20:25:59 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Mar 2022 20:25:59 GMT
EXPOSE 8080
# Mon, 07 Mar 2022 20:25:59 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ade7e68f4e34f438527a34c9761a285c3c3864e3daab0544b2c4f4163c7c3f56`  
		Last Modified: Thu, 03 Mar 2022 19:43:22 GMT  
		Size: 27.1 MB (27084671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43f6af3ffc9280862abe8d318417ec5189a40bdb95438f0cdacf12ba101e9e9`  
		Last Modified: Mon, 07 Mar 2022 19:46:50 GMT  
		Size: 19.2 MB (19234881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e3b8b0585e837e4a4ed112ad9abb2956d9a6fb4db1cdd151b4fb361fb64127`  
		Last Modified: Mon, 07 Mar 2022 19:47:36 GMT  
		Size: 43.6 MB (43616301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b3d69b5c708a9deaa5de0eae830fdd02779584a487a57b0be81affca3723b58`  
		Last Modified: Mon, 07 Mar 2022 19:47:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dbca531ba269dec939c1bd1f05b2415127d4e73772d6ea0ce093d0c60f1f81`  
		Last Modified: Mon, 07 Mar 2022 20:43:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec9c02ddf902f7f2ca259345f0b8c4f261d2068346095a7a79b977582e22afd`  
		Last Modified: Mon, 07 Mar 2022 20:44:42 GMT  
		Size: 12.6 MB (12578591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafcabc1576ee5f64962edfef820d5c668c617e901e3b4219aa68187bf96ff46`  
		Last Modified: Mon, 07 Mar 2022 20:44:41 GMT  
		Size: 450.1 KB (450133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017ab37b522a0642a41be11c2677fcfefe82efc86dc24d880058abc894793613`  
		Last Modified: Mon, 07 Mar 2022 20:44:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
