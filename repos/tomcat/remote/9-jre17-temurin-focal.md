## `tomcat:9-jre17-temurin-focal`

```console
$ docker pull tomcat@sha256:0700f8f2a5613d3d05f4c3020a5bd298c57fe1fda4b584a795d26dd9d1e74399
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
$ docker pull tomcat@sha256:78999f4c1c8ca4d31262c83d93db3a6ce7e75e16b249f13ba77e24260ee19f7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118754453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8855aac54532bba06def929c4c5a85c0cd5d501b1862eebddf712ea9a3055e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:23:15 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:24:07 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 22 Dec 2021 10:05:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='851205c5036543cbcf1953c3f5768977b9efaf6b86c9fb5ec1b6cab01f781faf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='e1d94e98c47f2530304eb187c74a3e3c1cf46ddb4d86c277edb1e499bb525fe1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0e9eee4977e14edc14d0e2acb97cb413f4a769e2d855d02131af1ccd877779ff';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ff88a8bcdaa8db788b463b14724460f68c4c70c80b86e556012521996281f4bf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9d58cb741509a88e0ae33eb022334fb900b409b198eca6fe76246f0677b392ad';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Dec 2021 10:05:25 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 10:05:26 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 22 Dec 2021 19:11:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 19:11:29 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 19:11:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 19:11:31 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 19:11:31 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 19:11:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 19:15:34 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 22 Dec 2021 19:15:34 GMT
ENV TOMCAT_MAJOR=9
# Wed, 22 Dec 2021 19:15:34 GMT
ENV TOMCAT_VERSION=9.0.56
# Wed, 22 Dec 2021 19:15:35 GMT
ENV TOMCAT_SHA512=b4c2c85891e84f0fbd8fec889ef0890d68a2bfa53eb31d4d39fcf5758aa483694af7ac27533ea4bc3fc3fdae56f2fa9c018d4acf872574c0ec5e37bb443599ce
# Wed, 22 Dec 2021 19:15:36 GMT
COPY dir:8a2f165f80fd76834c810eb8312e6af393c1afed22151e129679be9d7c860243 in /usr/local/tomcat 
# Wed, 22 Dec 2021 19:15:43 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 19:15:45 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 22 Dec 2021 19:15:45 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 19:15:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8329695590e84b5300263017fbf5b303ea7b92c02e4805724cae67d76d617245`  
		Last Modified: Mon, 29 Nov 2021 20:26:59 GMT  
		Size: 28.6 MB (28563394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790e3dba6d93a984d4b737786249c177a18a9b00124db36e50952c3f7bfed065`  
		Last Modified: Wed, 22 Dec 2021 10:07:23 GMT  
		Size: 47.0 MB (47008415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76d1ca8a56d780452a9f984931440d04e1f667e00cd099cd7530a513c400501`  
		Last Modified: Wed, 22 Dec 2021 10:07:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f1ef9d11d5ea24f920fe31816f1994199ffc0c95b6fcf055d30f103a86face`  
		Last Modified: Wed, 22 Dec 2021 19:30:39 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f70dc67e3f99113fcf219481c54d7bb46182a96f58cb45143198ddbbd36013`  
		Last Modified: Wed, 22 Dec 2021 19:34:04 GMT  
		Size: 12.3 MB (12251912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5022540477d90446ca2407a2bf6978341de9b5077718282a89afe7e796bda99`  
		Last Modified: Wed, 22 Dec 2021 19:34:03 GMT  
		Size: 2.4 MB (2363169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd975cbfb05a622d9656e082411404f72b86e5d98fd22b3f38979007da993e12`  
		Last Modified: Wed, 22 Dec 2021 19:34:02 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:5b0eedca489dbfa096de22d279cc24f5c39c7bb3c5e0433c793be3e30e020e7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110198629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:009e1a9dedd0807fa46549cc798df5d1f01770efc35cc5c15004ae6b93699399`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:02:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:02:46 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Thu, 23 Dec 2021 03:59:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='851205c5036543cbcf1953c3f5768977b9efaf6b86c9fb5ec1b6cab01f781faf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='e1d94e98c47f2530304eb187c74a3e3c1cf46ddb4d86c277edb1e499bb525fe1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0e9eee4977e14edc14d0e2acb97cb413f4a769e2d855d02131af1ccd877779ff';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ff88a8bcdaa8db788b463b14724460f68c4c70c80b86e556012521996281f4bf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9d58cb741509a88e0ae33eb022334fb900b409b198eca6fe76246f0677b392ad';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 23 Dec 2021 03:59:02 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 03:59:04 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Thu, 23 Dec 2021 06:04:44 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 23 Dec 2021 06:04:45 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 06:04:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 23 Dec 2021 06:04:46 GMT
WORKDIR /usr/local/tomcat
# Thu, 23 Dec 2021 06:04:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 23 Dec 2021 06:04:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 23 Dec 2021 06:08:52 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 23 Dec 2021 06:08:52 GMT
ENV TOMCAT_MAJOR=9
# Thu, 23 Dec 2021 06:08:53 GMT
ENV TOMCAT_VERSION=9.0.56
# Thu, 23 Dec 2021 06:08:53 GMT
ENV TOMCAT_SHA512=b4c2c85891e84f0fbd8fec889ef0890d68a2bfa53eb31d4d39fcf5758aa483694af7ac27533ea4bc3fc3fdae56f2fa9c018d4acf872574c0ec5e37bb443599ce
# Thu, 23 Dec 2021 06:08:56 GMT
COPY dir:5e191e42871d8e4913b1901fc8bfb9b8fc030d3d27a0ba551748f46773bb7589 in /usr/local/tomcat 
# Thu, 23 Dec 2021 06:09:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Dec 2021 06:09:11 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 23 Dec 2021 06:09:12 GMT
EXPOSE 8080
# Thu, 23 Dec 2021 06:09:12 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01ac063d17e84c31998292290d215bdc4fac4ff250c6809c5fde3571256b123`  
		Last Modified: Mon, 29 Nov 2021 20:09:29 GMT  
		Size: 27.4 MB (27369751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976e41ecc45fb507864396a6f72452e7c32ce567f7304ee820fa971e75391abe`  
		Last Modified: Thu, 23 Dec 2021 04:02:26 GMT  
		Size: 44.6 MB (44583759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0792654afbcfd1a15ba05360a006ff880f4058110a85ee4777de8a87b10d04`  
		Last Modified: Thu, 23 Dec 2021 04:01:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a1491defb377c7c011f337e6ce686ccf5e64ea0865bdab82c15a13ca243ba5`  
		Last Modified: Thu, 23 Dec 2021 06:24:16 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167b80d7dee2759dbd0ff1851ba4f779dafdcee6e63d842112539deb4dad24b4`  
		Last Modified: Thu, 23 Dec 2021 06:27:26 GMT  
		Size: 12.2 MB (12200951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539847dcad862c475f813024f166bcc3b13f06025e678c1a683cd22810183573`  
		Last Modified: Thu, 23 Dec 2021 06:27:22 GMT  
		Size: 2.0 MB (1979255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50368abac56454494f16563ec8f0c39834cc71e1115adde4fb7856538201c29a`  
		Last Modified: Thu, 23 Dec 2021 06:27:21 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:2ee5e51692c3eb974e119befe942647d0cbfe7b5923142957e8fe9aecb25ac0e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116478659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2beb5f35902763905818c1933d078084b117dec3f0cc9c7844f0fe3d06eb9f9a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:25:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:41:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:42:22 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 22 Dec 2021 04:24:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='851205c5036543cbcf1953c3f5768977b9efaf6b86c9fb5ec1b6cab01f781faf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='e1d94e98c47f2530304eb187c74a3e3c1cf46ddb4d86c277edb1e499bb525fe1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0e9eee4977e14edc14d0e2acb97cb413f4a769e2d855d02131af1ccd877779ff';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ff88a8bcdaa8db788b463b14724460f68c4c70c80b86e556012521996281f4bf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9d58cb741509a88e0ae33eb022334fb900b409b198eca6fe76246f0677b392ad';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Dec 2021 04:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 04:24:10 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 22 Dec 2021 19:32:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 19:33:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 19:33:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 19:33:02 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 19:33:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 19:33:04 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 19:38:49 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 22 Dec 2021 19:38:49 GMT
ENV TOMCAT_MAJOR=9
# Wed, 22 Dec 2021 19:38:50 GMT
ENV TOMCAT_VERSION=9.0.56
# Wed, 22 Dec 2021 19:38:51 GMT
ENV TOMCAT_SHA512=b4c2c85891e84f0fbd8fec889ef0890d68a2bfa53eb31d4d39fcf5758aa483694af7ac27533ea4bc3fc3fdae56f2fa9c018d4acf872574c0ec5e37bb443599ce
# Wed, 22 Dec 2021 19:38:53 GMT
COPY dir:67287e1f4a86b9e0d7f9bc2d87e66d33b408f449d5fc6229cb00b2c1941db52b in /usr/local/tomcat 
# Wed, 22 Dec 2021 19:39:01 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 19:39:03 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 22 Dec 2021 19:39:04 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 19:39:05 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bc7e92316b9d4dee98cf60f4fcb0995823e001fcc5448df92e5fb76485370a`  
		Last Modified: Mon, 29 Nov 2021 19:45:52 GMT  
		Size: 29.4 MB (29377186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2556b1b0a2d3afc98ef686b769f959d708ac3b77e69b625a5f0738942f96b04`  
		Last Modified: Wed, 22 Dec 2021 04:26:27 GMT  
		Size: 45.4 MB (45438063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a24ed4ea98ad4e13cdce4d8eb9140a5ccb4970ff96d23f3fe10fa9c4204418`  
		Last Modified: Wed, 22 Dec 2021 04:26:20 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a76d8772686439959166177b555febc81f7b4d3e54f20d9fef4f4d01298415`  
		Last Modified: Wed, 22 Dec 2021 20:01:46 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd30218cbe03faca8bd243108b2cda3550737976a329655e8a95b40d9f03951c`  
		Last Modified: Wed, 22 Dec 2021 20:05:58 GMT  
		Size: 12.3 MB (12267313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b490b81a4c8b13a0cdf1ff5b5b7b2114da9f683d4eba07e521ad325e8b5c753`  
		Last Modified: Wed, 22 Dec 2021 20:05:57 GMT  
		Size: 2.2 MB (2224930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:8fbce5aae280834ef8f4869f706c8734759046d0c6cb1918de3db4434db6c358
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124193358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38dc0c60dc8d82e8b2e67ec780b96bd21073e6157dc3e38897b236e43b0769e5`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:22:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:23:23 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 22 Dec 2021 11:22:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='851205c5036543cbcf1953c3f5768977b9efaf6b86c9fb5ec1b6cab01f781faf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='e1d94e98c47f2530304eb187c74a3e3c1cf46ddb4d86c277edb1e499bb525fe1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0e9eee4977e14edc14d0e2acb97cb413f4a769e2d855d02131af1ccd877779ff';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ff88a8bcdaa8db788b463b14724460f68c4c70c80b86e556012521996281f4bf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9d58cb741509a88e0ae33eb022334fb900b409b198eca6fe76246f0677b392ad';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 22 Dec 2021 11:22:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 11:22:58 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 22 Dec 2021 20:47:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 20:47:18 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 20:47:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 20:47:25 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 20:47:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 20:47:30 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 20:50:30 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 22 Dec 2021 20:50:31 GMT
ENV TOMCAT_MAJOR=9
# Wed, 22 Dec 2021 20:50:32 GMT
ENV TOMCAT_VERSION=9.0.56
# Wed, 22 Dec 2021 20:50:34 GMT
ENV TOMCAT_SHA512=b4c2c85891e84f0fbd8fec889ef0890d68a2bfa53eb31d4d39fcf5758aa483694af7ac27533ea4bc3fc3fdae56f2fa9c018d4acf872574c0ec5e37bb443599ce
# Wed, 22 Dec 2021 20:50:37 GMT
COPY dir:89c9e84192be9f2791e8039bcb2c48130912cb59774fd88cd67a4862555e635c in /usr/local/tomcat 
# Wed, 22 Dec 2021 20:50:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 20:50:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 22 Dec 2021 20:51:00 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 20:51:01 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d71f328d69a3848141b8b31ebd2a2657d78fcb95dfdd3400c8ed3202aa0a24b`  
		Last Modified: Mon, 29 Nov 2021 20:27:29 GMT  
		Size: 31.1 MB (31132613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba929e59de02b2367350431f0207e1ece4c9cd5fe1efc751ad4e524f885cd063`  
		Last Modified: Wed, 22 Dec 2021 11:25:35 GMT  
		Size: 44.9 MB (44921616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a59a4ba76522ec9e0caa26b20415e51fcb78361f802b46dc33d8521beaa129`  
		Last Modified: Wed, 22 Dec 2021 11:25:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc74755c77f954d5d3277205066dc08c999471d087c8d413b97d2d891ab33de`  
		Last Modified: Wed, 22 Dec 2021 20:57:59 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57320be97d7c7d982210fc227e3ed3173ebed017617b56ed28d25ed159b2fcf1`  
		Last Modified: Wed, 22 Dec 2021 20:59:43 GMT  
		Size: 12.3 MB (12293866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c46be6f93873cdd72b70c573cad2f79d704880b693ee9a52257fd98500daaa0`  
		Last Modified: Wed, 22 Dec 2021 20:59:42 GMT  
		Size: 2.6 MB (2557561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0039bca38ba2278bf3e4f788a46421db6bd489b662981b5d349b9339deac8696`  
		Last Modified: Wed, 22 Dec 2021 20:59:42 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:e8651255b22aeae9613787c45cc6945816411869af8b0584b9cb6e5541bb82d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.0 MB (112976291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1bf2c4b8616a27c1fa37a4561f711980c2929b4dc18b01e1418b8c62f25afc5`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:45:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:45:46 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Tue, 21 Dec 2021 19:11:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='851205c5036543cbcf1953c3f5768977b9efaf6b86c9fb5ec1b6cab01f781faf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='e1d94e98c47f2530304eb187c74a3e3c1cf46ddb4d86c277edb1e499bb525fe1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0e9eee4977e14edc14d0e2acb97cb413f4a769e2d855d02131af1ccd877779ff';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ff88a8bcdaa8db788b463b14724460f68c4c70c80b86e556012521996281f4bf';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='9d58cb741509a88e0ae33eb022334fb900b409b198eca6fe76246f0677b392ad';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jre_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 21 Dec 2021 19:11:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 19:11:58 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 22 Dec 2021 19:28:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 19:28:24 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 19:28:25 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 19:28:25 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 19:28:25 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 19:28:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 19:30:04 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 22 Dec 2021 19:30:04 GMT
ENV TOMCAT_MAJOR=9
# Wed, 22 Dec 2021 19:30:04 GMT
ENV TOMCAT_VERSION=9.0.56
# Wed, 22 Dec 2021 19:30:05 GMT
ENV TOMCAT_SHA512=b4c2c85891e84f0fbd8fec889ef0890d68a2bfa53eb31d4d39fcf5758aa483694af7ac27533ea4bc3fc3fdae56f2fa9c018d4acf872574c0ec5e37bb443599ce
# Wed, 22 Dec 2021 19:30:05 GMT
COPY dir:e2d9058777a6bbbd9e873eae0b768edbfff8519f253edb69b775360209336488 in /usr/local/tomcat 
# Wed, 22 Dec 2021 19:30:11 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 19:30:12 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 22 Dec 2021 19:30:12 GMT
EXPOSE 8080
# Wed, 22 Dec 2021 19:30:12 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd1b67c19cd65073e039ddb0ad0478e4ebeff4ccfb02e00bde920aefe11b4b`  
		Last Modified: Mon, 29 Nov 2021 19:47:48 GMT  
		Size: 27.9 MB (27940770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdb6e58eaecc8c9c280c305fd1dee0c0178cc709caaa8363c226947212225fb`  
		Last Modified: Tue, 21 Dec 2021 19:13:06 GMT  
		Size: 43.6 MB (43589282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c81a1922e99deda61fa3200ac30dbdce7a2866e1c9937132a4af4e378d14c6a`  
		Last Modified: Tue, 21 Dec 2021 19:13:00 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615f19e1b9d177a0881c021f0783680d42076dc33a2e1cb3b1fb2de9700783ff`  
		Last Modified: Wed, 22 Dec 2021 19:35:22 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a0f934cdd4835bf6f30d080eed613965580fa6d097d67ab86c09b16e2aa22`  
		Last Modified: Wed, 22 Dec 2021 19:36:51 GMT  
		Size: 12.3 MB (12264764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de29b24e3b38ef1ab96720cca2b3706c1b116f559c90eb2f2e67ac86efec3141`  
		Last Modified: Wed, 22 Dec 2021 19:36:50 GMT  
		Size: 2.1 MB (2060154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81987f2b6686afad2c6d2302a56ad740a4986d24e97003c31f74d30e1c8eb75f`  
		Last Modified: Wed, 22 Dec 2021 19:36:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
