## `tomcat:jre17-temurin-focal`

```console
$ docker pull tomcat@sha256:e8556b5fd71e6cf4b4c48586982814a2633889ce5b8a665ca2b9e829e18b9942
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:603cde703f4eb6e3f83c083d40bdc5a14444c19898f932da433195b87f351e4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.4 MB (108407497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:292db965549e926d7b3278f7f24ccf9008e24604cb38857fc732444493c99418`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:05:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Apr 2022 23:07:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:07:37 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 05 Apr 2022 23:08:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:08:05 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:08:05 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 06 Apr 2022 05:06:18 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 06 Apr 2022 05:06:18 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:06:19 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 06 Apr 2022 05:06:19 GMT
WORKDIR /usr/local/tomcat
# Wed, 06 Apr 2022 05:06:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 05:06:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 05:06:19 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 06 Apr 2022 05:06:20 GMT
ENV TOMCAT_MAJOR=10
# Wed, 06 Apr 2022 05:09:04 GMT
ENV TOMCAT_VERSION=10.0.20
# Wed, 06 Apr 2022 05:09:04 GMT
ENV TOMCAT_SHA512=53bfdbac2e6af5cca97dc01fffb0428380fbe21d8375f45d015c16a57017ff946fdc555ebad9e9fcbcb97b438c4f6daf3aa39d36ca79fd5a372cfc1a80b7117f
# Wed, 06 Apr 2022 05:09:05 GMT
COPY dir:eb7c3b5a86acfd275d046c75750c46999fdaabbf7273fc3118fcf047f00608f5 in /usr/local/tomcat 
# Wed, 06 Apr 2022 05:09:09 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:09:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Apr 2022 05:09:10 GMT
EXPOSE 8080
# Wed, 06 Apr 2022 05:09:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc7fe67d3007d02e7d89c114454bce7134a61ae03f677ea88b6da10596ee38f`  
		Last Modified: Tue, 05 Apr 2022 23:11:07 GMT  
		Size: 19.8 MB (19771517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e584c2234c5f7e14fd9a82f4a766422506631601318435746a239257a6626d8d`  
		Last Modified: Tue, 05 Apr 2022 23:12:10 GMT  
		Size: 47.0 MB (47038145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374eb6c4d8fddb8c49d719b830f249d15e0b814656944e569012606b59ff35bc`  
		Last Modified: Tue, 05 Apr 2022 23:12:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9333e3d9db984d3808fd81d173e21cd15057b2e431a9d3c5f9df5bf62f3fee26`  
		Last Modified: Wed, 06 Apr 2022 05:28:37 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dbeec1b98f4f38ef35f412986274903d45c250da7a25e16c84cc5f96e8ff3e`  
		Last Modified: Wed, 06 Apr 2022 05:31:02 GMT  
		Size: 12.6 MB (12582593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68e4c631e52060e3d71a2eef9d0bba28ebe68ab95e41695a37ac284f4e6bd8a`  
		Last Modified: Wed, 06 Apr 2022 05:31:02 GMT  
		Size: 448.5 KB (448487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8521a926a716806bbde45ca916d52fabd0a1b15dd4b7b94a08e8ba4360cb88`  
		Last Modified: Wed, 06 Apr 2022 05:31:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:7f3320f71057c8ba41fec4139d18389063e9e93e74099204fbe391aee53c4060
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100836213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344f1f0331702a31551baf7e2f4c1a49caacad38e7700e69dfa14c1ee94892e2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 06 Apr 2022 03:26:01 GMT
ADD file:be35fd9a0ef4a49afbe583edf1750187cad18b1bde4e7bf0ab344464740b5749 in / 
# Wed, 06 Apr 2022 03:26:01 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:03:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 06 Apr 2022 04:06:59 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:07:43 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Wed, 06 Apr 2022 04:08:35 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 04:08:36 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 04:08:37 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 06 Apr 2022 07:55:54 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 06 Apr 2022 07:55:55 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 07:55:56 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 06 Apr 2022 07:55:57 GMT
WORKDIR /usr/local/tomcat
# Wed, 06 Apr 2022 07:55:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 07:55:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 07:55:58 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 06 Apr 2022 07:55:58 GMT
ENV TOMCAT_MAJOR=10
# Wed, 06 Apr 2022 08:01:42 GMT
ENV TOMCAT_VERSION=10.0.20
# Wed, 06 Apr 2022 08:01:42 GMT
ENV TOMCAT_SHA512=53bfdbac2e6af5cca97dc01fffb0428380fbe21d8375f45d015c16a57017ff946fdc555ebad9e9fcbcb97b438c4f6daf3aa39d36ca79fd5a372cfc1a80b7117f
# Wed, 06 Apr 2022 08:01:44 GMT
COPY dir:479fa9b31caa6e94beddbe212a8523a25129a250b16cce4070986bee4d8a83e5 in /usr/local/tomcat 
# Wed, 06 Apr 2022 08:01:55 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 08:01:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Apr 2022 08:01:59 GMT
EXPOSE 8080
# Wed, 06 Apr 2022 08:01:59 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:de340d6c69b8bed917b969ad75b8fe4fe951502bc050b013dc9151c3632fb704`  
		Last Modified: Tue, 05 Apr 2022 13:15:39 GMT  
		Size: 24.1 MB (24073792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7eacdd26b0e96742477eb590629e1cb2d76d02c416494f0a25b3916ba4e7f2`  
		Last Modified: Wed, 06 Apr 2022 04:15:51 GMT  
		Size: 19.2 MB (19193623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1261fc56eb1bb2c03bdb5e7a49541f46578e861c49bb8330985151e2c3cd32fc`  
		Last Modified: Wed, 06 Apr 2022 04:19:07 GMT  
		Size: 44.6 MB (44611464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c2d881a68e5c0780809c6e8e36beee11e8a90dbd5006752e14a2f491a1314a`  
		Last Modified: Wed, 06 Apr 2022 04:18:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f308964790a58b35d0622e83b552b8fb1194767f75bbe626c0fa8a3b1ff1cad8`  
		Last Modified: Wed, 06 Apr 2022 10:15:14 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8377ac7907f195a59fd33ba1fe7535d49434eae1f722f02658e77f57dea8c73`  
		Last Modified: Wed, 06 Apr 2022 10:18:10 GMT  
		Size: 12.5 MB (12532385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3851435c1ebfaf36025600c27258771b6048b7fadf40c88e972d6d20e9dc34`  
		Last Modified: Wed, 06 Apr 2022 10:18:06 GMT  
		Size: 424.5 KB (424485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab202be0699b52ebeef8eda78290449ce105f92ca459b2800c242006bea2aa3f`  
		Last Modified: Wed, 06 Apr 2022 10:18:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:db1d96b5c8312e7289bb9f5be6e2cf1ed9e7be8a87706db06c7a3ca9ee56f9b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105962025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc4524c855eaf1a474792aceb6c2a9e361987999eb41622de6184a567af9e902`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:19:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Apr 2022 23:21:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:22:05 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 05 Apr 2022 23:22:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:22:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:22:42 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 06 Apr 2022 06:03:57 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 06 Apr 2022 06:03:58 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 06:03:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 06 Apr 2022 06:04:00 GMT
WORKDIR /usr/local/tomcat
# Wed, 06 Apr 2022 06:04:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 06:04:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 06:04:03 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 06 Apr 2022 06:04:04 GMT
ENV TOMCAT_MAJOR=10
# Wed, 06 Apr 2022 06:08:46 GMT
ENV TOMCAT_VERSION=10.0.20
# Wed, 06 Apr 2022 06:08:47 GMT
ENV TOMCAT_SHA512=53bfdbac2e6af5cca97dc01fffb0428380fbe21d8375f45d015c16a57017ff946fdc555ebad9e9fcbcb97b438c4f6daf3aa39d36ca79fd5a372cfc1a80b7117f
# Wed, 06 Apr 2022 06:08:49 GMT
COPY dir:7f495ad429496cae7122334b6bd62c64923d902b25bbc43f9dac75b67a2ddc2b in /usr/local/tomcat 
# Wed, 06 Apr 2022 06:08:55 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:08:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Apr 2022 06:08:58 GMT
EXPOSE 8080
# Wed, 06 Apr 2022 06:08:59 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbf60885516768e1cf4d85dfe4d2ef57124a0af5e3fc86767efa1ebeea112ed`  
		Last Modified: Tue, 05 Apr 2022 23:26:50 GMT  
		Size: 20.5 MB (20498028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fced41d253069102b2619b4b6f2bd6fbc0eb81cc56473d54f60ec7ed8998b9`  
		Last Modified: Tue, 05 Apr 2022 23:28:05 GMT  
		Size: 45.5 MB (45484473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab5d8618b73dc66cfd2c03843892de68680d48846f69f93be7c80ca66b055a4`  
		Last Modified: Tue, 05 Apr 2022 23:27:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c1773f69859e46ef5ff88575c52cc9c26afea084a2ee694f854349866e488b`  
		Last Modified: Wed, 06 Apr 2022 06:45:19 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52b0a49b88b9dabfecf9c6da5043e77a11e99647fd2b38083e3273bde678630`  
		Last Modified: Wed, 06 Apr 2022 06:48:27 GMT  
		Size: 12.6 MB (12598774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e086fda170e7f1de1fbdc950312d13a75f7dee1a31869d91e72002ce19c81a26`  
		Last Modified: Wed, 06 Apr 2022 06:48:26 GMT  
		Size: 211.1 KB (211091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:449912b66308b3aa9382ddf91fd46a1f6e4af448870a3eba6487eb1f34c6ca77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113702005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46940d61b38753a0067f3b9f2e047fac1e4afd1f1c7428e5243ed7cb3f603baf`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:37 GMT
ADD file:c1af9c0e405f7eecbc87225c13709becfd46d66f87a4c5b8e30a1b82de7337e5 in / 
# Wed, 06 Apr 2022 03:35:41 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:53:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 06 Apr 2022 05:01:20 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:03:00 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Wed, 06 Apr 2022 05:04:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 06 Apr 2022 05:04:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 05:04:41 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 06 Apr 2022 08:40:14 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 06 Apr 2022 08:40:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 06 Apr 2022 08:40:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 06 Apr 2022 08:40:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 06 Apr 2022 08:40:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 08:41:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 06 Apr 2022 08:41:05 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 06 Apr 2022 08:41:07 GMT
ENV TOMCAT_MAJOR=10
# Wed, 06 Apr 2022 09:04:52 GMT
ENV TOMCAT_VERSION=10.0.20
# Wed, 06 Apr 2022 09:05:04 GMT
ENV TOMCAT_SHA512=53bfdbac2e6af5cca97dc01fffb0428380fbe21d8375f45d015c16a57017ff946fdc555ebad9e9fcbcb97b438c4f6daf3aa39d36ca79fd5a372cfc1a80b7117f
# Wed, 06 Apr 2022 09:05:08 GMT
COPY dir:74241ecd30ba3e884a0d2a92ec7c2c214470b93138b5c5205401111475c3eca3 in /usr/local/tomcat 
# Wed, 06 Apr 2022 09:05:30 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 09:05:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Apr 2022 09:05:59 GMT
EXPOSE 8080
# Wed, 06 Apr 2022 09:06:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:83a2da48a82b52067676278a5eb4359bd7a79e7b57cabd370d77e11a9204121c`  
		Last Modified: Tue, 05 Apr 2022 13:16:22 GMT  
		Size: 33.3 MB (33291809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb55998198cd447fabd7426b9b309f4fe1c7fdb07fc7b6e8098af187e5a9e1f`  
		Last Modified: Wed, 06 Apr 2022 05:10:25 GMT  
		Size: 21.7 MB (21690183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f7f710f3bd3cc6daa63daa0bb14629f19e25282a095a38855328f4063867b5`  
		Last Modified: Wed, 06 Apr 2022 05:11:45 GMT  
		Size: 45.6 MB (45621129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ccfa399d67badf3f22df639e5958953e46a92f97b696822f959e9e09fdc0e1`  
		Last Modified: Wed, 06 Apr 2022 05:11:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf46b77dab35c3b7c11a67682b15703cb6d6bfe9fe3daa9d910a0541da11136`  
		Last Modified: Wed, 06 Apr 2022 10:16:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85291800ca30643a74ff496ae313b8e978697a6ec5ed341c66c8fd7a9c04b7f`  
		Last Modified: Wed, 06 Apr 2022 10:19:16 GMT  
		Size: 12.6 MB (12624332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc50224311dd4217238ec4e698985f882377a86e62f2c2c71c6ae31e187c98a1`  
		Last Modified: Wed, 06 Apr 2022 10:19:15 GMT  
		Size: 474.1 KB (474087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56eb20be294a935aed0ab36661464ff09095381e694e55ea676f2f985da51123`  
		Last Modified: Wed, 06 Apr 2022 10:19:14 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:50b39c3b8e991d2b0fcfb296faca08695cdaea3fbbafcfdb6990443a52eeff8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (102981605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6f69efd199753254e6ed434564115306311ac5dbebf831825f57fa844d238a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 05 Apr 2022 22:42:05 GMT
ADD file:44b5cfe67740a0d7e33d6aa2c83d9918fdb30a0649aa3471e2f668dec1ba7f3a in / 
# Tue, 05 Apr 2022 22:42:07 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:59:29 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 05 Apr 2022 23:00:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:01:01 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 05 Apr 2022 23:01:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 05 Apr 2022 23:01:30 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:01:31 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 05 Apr 2022 23:47:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 05 Apr 2022 23:47:25 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 23:47:25 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 05 Apr 2022 23:47:25 GMT
WORKDIR /usr/local/tomcat
# Tue, 05 Apr 2022 23:47:25 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 05 Apr 2022 23:47:26 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 05 Apr 2022 23:47:26 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 05 Apr 2022 23:47:26 GMT
ENV TOMCAT_MAJOR=10
# Tue, 05 Apr 2022 23:49:48 GMT
ENV TOMCAT_VERSION=10.0.20
# Tue, 05 Apr 2022 23:49:48 GMT
ENV TOMCAT_SHA512=53bfdbac2e6af5cca97dc01fffb0428380fbe21d8375f45d015c16a57017ff946fdc555ebad9e9fcbcb97b438c4f6daf3aa39d36ca79fd5a372cfc1a80b7117f
# Tue, 05 Apr 2022 23:49:48 GMT
COPY dir:48d981c60ecb0736c81a4737f7586fcd66dcde883b624bdf5955849daca2c851 in /usr/local/tomcat 
# Tue, 05 Apr 2022 23:49:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:49:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 05 Apr 2022 23:49:54 GMT
EXPOSE 8080
# Tue, 05 Apr 2022 23:49:54 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:502c7975d4ed549ab7d6e63b9ea10b0d24c1c3c12a33540d91d6739a0218faec`  
		Last Modified: Tue, 05 Apr 2022 13:17:47 GMT  
		Size: 27.1 MB (27084913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0e34cdc988538abf4cdb8842ac912ad4ebce5760f9a3f3b5407ed8fb65eddd`  
		Last Modified: Tue, 05 Apr 2022 23:03:02 GMT  
		Size: 19.2 MB (19234416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4dc88275f295fd0b89bea162af5d6d19ff290d482fe5e2a6be60a06dc9f67a`  
		Last Modified: Tue, 05 Apr 2022 23:03:45 GMT  
		Size: 43.6 MB (43616377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2363c1a253fb0f936bd1befdae089cbc3bdd0d716b011a72f8b1da8e20163694`  
		Last Modified: Tue, 05 Apr 2022 23:03:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700efd9745f3503e22bb3b27376779b1359505296b782ee5a54cc387ff2923a8`  
		Last Modified: Wed, 06 Apr 2022 00:00:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379f0a8450f33bf04081a11f7dc666ed88ee5fa6243d96ff83d1105e050e7897`  
		Last Modified: Wed, 06 Apr 2022 00:01:58 GMT  
		Size: 12.6 MB (12595426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9b5d7ea91b8caf41ab5bb7e8b4f8af6b874c27b7207bb3727f22e76fd47b72`  
		Last Modified: Wed, 06 Apr 2022 00:01:57 GMT  
		Size: 450.0 KB (450010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3311eb2ef3c9a5a48fae9a7bf61ca185003ea7d580f1dedf180366e3782178cc`  
		Last Modified: Wed, 06 Apr 2022 00:01:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
