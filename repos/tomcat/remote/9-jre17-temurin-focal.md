## `tomcat:9-jre17-temurin-focal`

```console
$ docker pull tomcat@sha256:df2a7ba59d9e6c61f56f80253e4bb79a3d6ec03291ae2de0343130ecadba2d37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:9-jre17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:5bbbc1021a6dafcfafc53fe4346fe401de021a8fc0e1c6595562df32c0dc1603
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108054569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4bee0f003abdd638003333bed859aab49dea73baa16f275b16b0096f69cbac`
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
# Wed, 06 Apr 2022 05:12:59 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 06 Apr 2022 05:12:59 GMT
ENV TOMCAT_MAJOR=9
# Wed, 06 Apr 2022 05:12:59 GMT
ENV TOMCAT_VERSION=9.0.62
# Wed, 06 Apr 2022 05:12:59 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Wed, 06 Apr 2022 05:13:00 GMT
COPY dir:8ffb8a853792e8722657ad5883cd13424ef2ef2cf271baac2e9ca539ab8a3a46 in /usr/local/tomcat 
# Wed, 06 Apr 2022 05:13:04 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:13:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Apr 2022 05:13:06 GMT
EXPOSE 8080
# Wed, 06 Apr 2022 05:13:06 GMT
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
	-	`sha256:e34b7a6f3dafc9614dabab3397c170ff30800bbef0b272b065d55d4a3d2533ca`  
		Last Modified: Wed, 06 Apr 2022 05:35:08 GMT  
		Size: 12.2 MB (12229657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b78248b017c277e6ba5d0de0a8fe76899c028b1ffdfb3354d06ffd229710751`  
		Last Modified: Wed, 06 Apr 2022 05:35:07 GMT  
		Size: 448.5 KB (448495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c97c5bef7359d572e10f857a13a3812c7c4b6ebc108a725caf79ef9c89495`  
		Last Modified: Wed, 06 Apr 2022 05:35:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:bbab5e86055a79af7965b29ecc65429bc149b361066fa1f02f9bb25089d0ac10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100481977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e5842bc872459c0432414315bd1e1345c548f528a82f2d52fef76e284ffa4df`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:41 GMT
ADD file:2e353e40ad52bb1b5a10aafb7912657744b02d096925b5bfc6e925ebf7cddede in / 
# Fri, 18 Mar 2022 07:32:42 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:32:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sun, 20 Mar 2022 06:36:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:37:15 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Sun, 20 Mar 2022 06:38:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sun, 20 Mar 2022 06:38:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 06:38:09 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sun, 20 Mar 2022 20:52:08 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 20 Mar 2022 20:52:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 20:52:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 20 Mar 2022 20:52:11 GMT
WORKDIR /usr/local/tomcat
# Sun, 20 Mar 2022 20:52:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 20:52:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 21:06:59 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sun, 20 Mar 2022 21:07:00 GMT
ENV TOMCAT_MAJOR=9
# Fri, 01 Apr 2022 18:45:25 GMT
ENV TOMCAT_VERSION=9.0.62
# Fri, 01 Apr 2022 18:45:25 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Fri, 01 Apr 2022 18:45:27 GMT
COPY dir:c1575744557a70f919ad106cba020ae94bb0ff48e5ba9d32f33f88bc09f991ac in /usr/local/tomcat 
# Fri, 01 Apr 2022 18:45:38 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 18:45:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Apr 2022 18:45:42 GMT
EXPOSE 8080
# Fri, 01 Apr 2022 18:45:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:260b2dce5be1e0d17bf9e2ec2bbde587e5023ab1b48278ddf8396dcfc8eb7e99`  
		Last Modified: Fri, 18 Mar 2022 07:36:23 GMT  
		Size: 24.1 MB (24073481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0025c0f90a7f66ad8f3026ab615333fb7de3a759f2fa27bf660ac1a823998710`  
		Last Modified: Sun, 20 Mar 2022 06:44:24 GMT  
		Size: 19.2 MB (19194875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afba130525c888ef02e02812936b6e8212f6b62dee0235c4f0706646e1402785`  
		Last Modified: Sun, 20 Mar 2022 06:47:53 GMT  
		Size: 44.6 MB (44611491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b643be74d04639ec30eb7613685910dfd752e03ab2ebb50291e35eea6cdc17cd`  
		Last Modified: Sun, 20 Mar 2022 06:47:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c789f916957fe35d24df0f3ef4313ac0f1d001530b9c0b43cc57ee43ad5382`  
		Last Modified: Sun, 20 Mar 2022 21:34:41 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a8f1ff3e419077510f720bc7afb290f50ee71faeef167b697799c851f6c026`  
		Last Modified: Fri, 01 Apr 2022 19:18:50 GMT  
		Size: 12.2 MB (12177006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7375c968129e8f993c78c2a0a9e775ed1a0a060cc8a6a5b16db71fe96345e119`  
		Last Modified: Fri, 01 Apr 2022 19:18:45 GMT  
		Size: 424.7 KB (424660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6e1cae52d7977ab664709efc8b2c2979f3a16d2ad79053eda4c0fd20cba4b9`  
		Last Modified: Fri, 01 Apr 2022 19:18:45 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:d3ec83336b9a2cefaf1e6076e5cdbd8a9e3dc01664c6fa0d5fa49e09c1a7ab7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105609740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452bc97aa9fe473b05dcd120f63043f2562d554f88bb631a69f9ca32d993ba77`
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
# Wed, 06 Apr 2022 06:15:30 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 06 Apr 2022 06:15:31 GMT
ENV TOMCAT_MAJOR=9
# Wed, 06 Apr 2022 06:15:32 GMT
ENV TOMCAT_VERSION=9.0.62
# Wed, 06 Apr 2022 06:15:33 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Wed, 06 Apr 2022 06:15:35 GMT
COPY dir:50ca5124732e976c3f1625a1b6eca6f80f75c8aee9341171132949102f0402a1 in /usr/local/tomcat 
# Wed, 06 Apr 2022 06:15:41 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 06:15:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 06 Apr 2022 06:15:44 GMT
EXPOSE 8080
# Wed, 06 Apr 2022 06:15:45 GMT
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
	-	`sha256:b9cab49a59eee352f805cd91fe22af726b0149d9950ba4ad5b3068348a7212c7`  
		Last Modified: Wed, 06 Apr 2022 08:37:59 GMT  
		Size: 12.2 MB (12246497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f10ee37c547a72e87fe3b5ca22a2b57d7ae8543caddf39edba78dee7a4ac9bb`  
		Last Modified: Wed, 06 Apr 2022 08:37:57 GMT  
		Size: 211.1 KB (211083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:e2afebc23b01c7447c8594896ecfc0a277776bd5bafc8d42764db6f41bddd3c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.4 MB (113352342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:327dab47cd8b3f0f0ef5a8e969287fe0a0b5112e356fc42aebe22a94f79099c1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Mar 2022 00:48:28 GMT
ADD file:4f85f0964cc66c6d7dd6a29e535eb2235ff8847d3c3aa3342c74cc53710ae499 in / 
# Fri, 18 Mar 2022 00:48:34 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 20:09:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 20:14:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 20:14:54 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Sat, 19 Mar 2022 20:15:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='6ef7a28d0d844fe347ab18f65a91db744547321fe8a101d883bd80722183ab64';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='4fd1d11f3008aba1c6c17e1d1c1cf15e2a54e68275ad0874b47a781eaf73450e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='089a940d0feb34e8095dede569492a5c4b1f082898ab02c39465fa76fe85a555';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='26a9b87d7abba7ea2d85f279b7b0109c1653fb3334871d5f3790e23b8d2b34e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='292ed702d95f5690e52e171afe9f3050b9d2fb803456b155c831735fad0f17c0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 20:15:56 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 20:16:03 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Sun, 20 Mar 2022 20:40:15 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 20 Mar 2022 20:40:20 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 20:40:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 20 Mar 2022 20:40:33 GMT
WORKDIR /usr/local/tomcat
# Sun, 20 Mar 2022 20:40:36 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 20:40:40 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 20 Mar 2022 21:12:19 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sun, 20 Mar 2022 21:12:20 GMT
ENV TOMCAT_MAJOR=9
# Fri, 01 Apr 2022 19:04:18 GMT
ENV TOMCAT_VERSION=9.0.62
# Fri, 01 Apr 2022 19:04:21 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Fri, 01 Apr 2022 19:04:23 GMT
COPY dir:c5ef5cc23661fb17449e25cb5aed425812874db29ca9d86cfccd8b7cf7279ddd in /usr/local/tomcat 
# Fri, 01 Apr 2022 19:04:41 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 19:04:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Apr 2022 19:04:56 GMT
EXPOSE 8080
# Fri, 01 Apr 2022 19:04:59 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cf1115d7b3bb72f50de3eb695005fb2c88fb88d73f535f164b306c4ab972c570`  
		Last Modified: Fri, 18 Mar 2022 00:51:19 GMT  
		Size: 33.3 MB (33292416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6497a12e20a4d667325b1e0e9651e8ed921d66c74663b4635145a0e142a9ea05`  
		Last Modified: Sat, 19 Mar 2022 20:20:11 GMT  
		Size: 21.7 MB (21691734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5144e909fb1003112bba3d79c23e9196d05f6f4f9ecdf7defe2c9347f7b8199f`  
		Last Modified: Sat, 19 Mar 2022 20:21:32 GMT  
		Size: 45.6 MB (45621107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdbe30de83357914eefaa03098dfa460a960199bed954348b3edf212895330c`  
		Last Modified: Sat, 19 Mar 2022 20:21:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53440681707cd7c10ae76540cf9731ffa2bb83567fa17524a8edbf8b629a8a12`  
		Last Modified: Sun, 20 Mar 2022 21:48:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c1612588302848749a10db2b10c007b5f48e5bb2f90f2c1125cb85f538fb64`  
		Last Modified: Fri, 01 Apr 2022 19:42:44 GMT  
		Size: 12.3 MB (12272458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4c2260afb55a4e7a5ded1fb409d71bbe03ca656eb3215a75a9c7a13dd66b6`  
		Last Modified: Fri, 01 Apr 2022 19:42:42 GMT  
		Size: 474.2 KB (474165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8dd34418a774a33b466d3de9c09f2f2b1519bad65c8b0c135a42f5eebdba0`  
		Last Modified: Fri, 01 Apr 2022 19:42:42 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:8bf6bde681fc1200fe9b9aa6f470c1e270b296c0e9028f06c0607759c57a21e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102628839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d63a36cd356ca15b8bb0483359e589d3d3744b344dc49c867c66961e9de289`
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
# Tue, 05 Apr 2022 23:52:04 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 05 Apr 2022 23:52:04 GMT
ENV TOMCAT_MAJOR=9
# Tue, 05 Apr 2022 23:52:04 GMT
ENV TOMCAT_VERSION=9.0.62
# Tue, 05 Apr 2022 23:52:04 GMT
ENV TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f
# Tue, 05 Apr 2022 23:52:04 GMT
COPY dir:48d784367f554e0721f460767d17ca52afe9937db26af93215bca23e4a9dbbb4 in /usr/local/tomcat 
# Tue, 05 Apr 2022 23:52:10 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:52:11 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 05 Apr 2022 23:52:11 GMT
EXPOSE 8080
# Tue, 05 Apr 2022 23:52:11 GMT
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
	-	`sha256:18f25c33cdb32c70e539afd2d13ac39147d9ca5d0e430025c93bed44b8c1dce0`  
		Last Modified: Wed, 06 Apr 2022 00:03:39 GMT  
		Size: 12.2 MB (12242633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e5b4905267d28a166646a5f4778dfdf8d1354fe902165d797a67df6b16907`  
		Last Modified: Wed, 06 Apr 2022 00:03:38 GMT  
		Size: 450.0 KB (450038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a7e1c79e7ffec24930203a4526782ef98081426ddd6a58611209de1ec6b2b2`  
		Last Modified: Wed, 06 Apr 2022 00:03:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
