## `tomcat:jre17`

```console
$ docker pull tomcat@sha256:5ef73941215a41b67464b33b4d5a6e6f199798a3acfc065766834ef1c4c8d03b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; s390x

### `tomcat:jre17` - linux; s390x

```console
$ docker pull tomcat@sha256:695405f866b9cac90125ecd9dbe1341407d2f08de11005001bd5e5797a16b843
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.0 MB (103019375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7584910f159701b43c2e07c2655e7dd925357683e74cc3c7845fe8e6d1fc7fcd`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:11:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 06:19:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:36:16 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 07 Jun 2022 06:38:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:38:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:38:56 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 10:37:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 10:37:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 10:37:09 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 10:37:10 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 10:37:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:37:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:37:12 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 07 Jun 2022 10:37:13 GMT
ENV TOMCAT_MAJOR=10
# Mon, 13 Jun 2022 20:55:24 GMT
ENV TOMCAT_VERSION=10.0.22
# Mon, 13 Jun 2022 20:55:24 GMT
ENV TOMCAT_SHA512=fe46db8794f066882b30e7a94bd8d3dbcf29e8e8ffaf67c1355846755745a7c9eafd124819283f218bcf410921a485b44b57b56fd6251fb99d67d95f3dd36826
# Mon, 13 Jun 2022 20:55:26 GMT
COPY dir:80226b45d62a567078eec08218b94f56e357b08786166dd732ce22c45cd6e9b7 in /usr/local/tomcat 
# Mon, 13 Jun 2022 20:55:35 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 13 Jun 2022 20:55:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 13 Jun 2022 20:55:42 GMT
EXPOSE 8080
# Mon, 13 Jun 2022 20:55:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b03f2d497bd002a5fc2d0070513cb6b5efa08e1c570c55fd15d3d4c89622e29`  
		Last Modified: Tue, 07 Jun 2022 06:25:49 GMT  
		Size: 19.2 MB (19229549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a157f755a6f207b2c8fc4a018b5cda6d53c448447f84b315daa72b9fed583a61`  
		Last Modified: Tue, 07 Jun 2022 06:44:39 GMT  
		Size: 43.7 MB (43671718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fd41b6f4e1e27165dbca0a198c8d6fa49517a9699f5cad193672434841b380`  
		Last Modified: Tue, 07 Jun 2022 06:44:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13047eefdf206817f87424fa292284ad1661379fc6f93757b7bed2666e0caea8`  
		Last Modified: Tue, 07 Jun 2022 10:54:50 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d1c3f2aba36350e81efbe8ffb168bd0b5d8768aa3552fb8009d7f71a664abe`  
		Last Modified: Mon, 13 Jun 2022 21:07:49 GMT  
		Size: 12.6 MB (12611300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e8dceb7a5e95939ad2b70b4d632aa07651409d1d892b2b2766d2ccf5b3671e`  
		Last Modified: Mon, 13 Jun 2022 21:07:48 GMT  
		Size: 450.3 KB (450327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08becc4730c2ad49c502eb2e22fc772179426163b86c0f2317da14e11d069233`  
		Last Modified: Mon, 13 Jun 2022 21:07:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
