## `tomcat:8-jre8-temurin`

```console
$ docker pull tomcat@sha256:fef2be09e680e9f25d994cbc82b522144b1004d61de91258bab4b6b658ce7396
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:8-jre8-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:e73bf6ed8765c41087be09a62415f988b762e5da59a61017cc84bb9511d64326
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96977440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e08afcbe3f3694a5e89dab31600529a3d1715cee29440a7ccb183edea81ff182`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:39:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 15:39:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 15:39:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 15:39:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:39:13 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 16 Aug 2023 15:39:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 16 Aug 2023 15:39:39 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 16 Aug 2023 15:39:39 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 15:39:39 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 16 Aug 2023 18:29:49 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 16 Aug 2023 18:29:49 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:29:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 16 Aug 2023 18:29:50 GMT
WORKDIR /usr/local/tomcat
# Wed, 16 Aug 2023 18:29:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 18:29:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 18:35:00 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 16 Aug 2023 18:35:01 GMT
ENV TOMCAT_MAJOR=8
# Wed, 16 Aug 2023 18:35:01 GMT
ENV TOMCAT_VERSION=8.5.92
# Wed, 16 Aug 2023 18:35:01 GMT
ENV TOMCAT_SHA512=faab13a29531a800d38b2602ff76c0041277ffbfb25b938bbefb84ef6ad3ffa26d2c2645cd233eb0d819bcca9887aaeb44df6c044852160d000e5084b1addc2f
# Wed, 16 Aug 2023 18:35:01 GMT
COPY dir:e6ea6e8c9a56b71275dade379f59b43cf92f8f3679804588522d851484353502 in /usr/local/tomcat 
# Wed, 16 Aug 2023 18:35:05 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 18:35:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 16 Aug 2023 18:35:06 GMT
EXPOSE 8080
# Wed, 16 Aug 2023 18:35:06 GMT
ENTRYPOINT []
# Wed, 16 Aug 2023 18:35:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabb03f19f5a305a4162b2dadb7942d094cb8ae82bfbb4ac13d4df822a60ffe3`  
		Last Modified: Wed, 16 Aug 2023 15:43:09 GMT  
		Size: 12.9 MB (12902780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c428299586ef52fd07d7c0d5f704db673cb4e5fee15d57f0660f51caa19063a2`  
		Last Modified: Wed, 16 Aug 2023 15:43:37 GMT  
		Size: 41.9 MB (41851953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251696f718446151beda6737dde2edfa5168af192406e3c7e583e0e81be3cc63`  
		Last Modified: Wed, 16 Aug 2023 15:43:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea682eac76ec559e73c2933dccc1180b2397ba5126267f15568edbb8a713aa0`  
		Last Modified: Wed, 16 Aug 2023 15:43:32 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac71830742ddd7e868ad53b18adfea65964904e3d401a34823840842bd61fc`  
		Last Modified: Wed, 16 Aug 2023 18:44:12 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c31ba88175876d824e90584b807b49b58a71f2fdcd2ac6b5f12d48ca77ae05`  
		Last Modified: Wed, 16 Aug 2023 18:48:00 GMT  
		Size: 11.3 MB (11327978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee6cf1e6e8c83cda7e397882c2639b2c459d8e010fcf6281f2165bc319af902`  
		Last Modified: Wed, 16 Aug 2023 18:47:59 GMT  
		Size: 455.6 KB (455575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42672780f3efec38cb83f2d08727c91b4f261cc8c3cf0164a1d17479e74118e`  
		Last Modified: Wed, 16 Aug 2023 18:47:59 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:06656e808dae0349619612aef53445fd5e791ccc90f913243d5a6a0d1b8dd9d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.6 MB (91552102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1183381c8f46370fd02aff8e260a1a8d3f0ed069e5c528c7f1a6626087b3cb8d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:09:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:09:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:09:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 18:59:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 18:59:01 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 08 Aug 2023 18:59:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 08 Aug 2023 18:59:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Mon, 14 Aug 2023 18:09:39 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:39 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:56:41 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 14 Aug 2023 18:56:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 18:56:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 14 Aug 2023 18:56:42 GMT
WORKDIR /usr/local/tomcat
# Mon, 14 Aug 2023 18:56:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 18:56:42 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 19:01:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 14 Aug 2023 19:01:17 GMT
ENV TOMCAT_MAJOR=8
# Tue, 15 Aug 2023 23:45:52 GMT
ENV TOMCAT_VERSION=8.5.92
# Tue, 15 Aug 2023 23:45:52 GMT
ENV TOMCAT_SHA512=faab13a29531a800d38b2602ff76c0041277ffbfb25b938bbefb84ef6ad3ffa26d2c2645cd233eb0d819bcca9887aaeb44df6c044852160d000e5084b1addc2f
# Tue, 15 Aug 2023 23:45:53 GMT
COPY dir:6c42e14a12c210fbf597335830d3ae36065ab7cc7b4bb96b426da008c1bdd186 in /usr/local/tomcat 
# Tue, 15 Aug 2023 23:45:56 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Aug 2023 23:45:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Aug 2023 23:45:57 GMT
EXPOSE 8080
# Tue, 15 Aug 2023 23:45:58 GMT
ENTRYPOINT []
# Tue, 15 Aug 2023 23:45:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791f420277f117d4cbc9798bac0e3991df4d76dcb209a6289b5474d81f4c32d0`  
		Last Modified: Tue, 08 Aug 2023 19:02:56 GMT  
		Size: 12.5 MB (12491020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69bbce44b7eb87b109043d88470b2a51ac41cbd95acaf03fa655ea8789e1150`  
		Last Modified: Tue, 08 Aug 2023 19:03:35 GMT  
		Size: 40.3 MB (40342272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674a997ba89ff98282958c693d715e0de5b2371892e18ada3ce649747d726ac0`  
		Last Modified: Tue, 08 Aug 2023 19:03:30 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6db0d1ac0fcc9ab92e6e0a39172528a7d62dc81a74924c252fca023f526cb4`  
		Last Modified: Mon, 14 Aug 2023 18:10:53 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06028262254b0f857412cc990c7ea674dbc12074941db145d2906f11e7ac47b`  
		Last Modified: Mon, 14 Aug 2023 19:09:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668439756a42b0b98bb87453ecd585958bfed003b15b74cb3057739e52318690`  
		Last Modified: Tue, 15 Aug 2023 23:57:40 GMT  
		Size: 11.3 MB (11261091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f273d67d59c166c435c8d2b0564764e8ce3075490b2904b584dc500ff03bab9`  
		Last Modified: Tue, 15 Aug 2023 23:57:39 GMT  
		Size: 429.6 KB (429561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4197596e896aa24d4a876edd84e12e33fbe3720179c4c96f920825c87c82e66`  
		Last Modified: Tue, 15 Aug 2023 23:57:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:18cadccd1122620aa33d9ef2ee13812174de81c084d710992786183c52c2da81
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93872513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7692a07465b4a0ed750d715e4825ecfb230ff6e2dfb25c40e94c88430763db56`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 14:23:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 14:23:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 14:23:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 14:23:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 14:23:39 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 16 Aug 2023 14:23:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 16 Aug 2023 14:23:57 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 16 Aug 2023 14:23:57 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 14:23:57 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 16 Aug 2023 22:01:39 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 16 Aug 2023 22:01:39 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 22:01:39 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 16 Aug 2023 22:01:39 GMT
WORKDIR /usr/local/tomcat
# Wed, 16 Aug 2023 22:01:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 22:01:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 22:06:06 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 16 Aug 2023 22:06:06 GMT
ENV TOMCAT_MAJOR=8
# Wed, 16 Aug 2023 22:06:06 GMT
ENV TOMCAT_VERSION=8.5.92
# Wed, 16 Aug 2023 22:06:07 GMT
ENV TOMCAT_SHA512=faab13a29531a800d38b2602ff76c0041277ffbfb25b938bbefb84ef6ad3ffa26d2c2645cd233eb0d819bcca9887aaeb44df6c044852160d000e5084b1addc2f
# Wed, 16 Aug 2023 22:06:07 GMT
COPY dir:6db271381de3a7d18050c81eb894b242152c14b107b23dbfe7ee8c954d217717 in /usr/local/tomcat 
# Wed, 16 Aug 2023 22:06:10 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:06:11 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 16 Aug 2023 22:06:11 GMT
EXPOSE 8080
# Wed, 16 Aug 2023 22:06:11 GMT
ENTRYPOINT []
# Wed, 16 Aug 2023 22:06:11 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9820f088487afe4c2ad735189bd2cca7b6b80af8efbaf6103e1ba1ae78d9f50`  
		Last Modified: Wed, 16 Aug 2023 14:26:46 GMT  
		Size: 12.8 MB (12843960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842eb90ddefb56c65cee49204f2ff2b8ece981dd3eff4e3400c905a8bbfecf9`  
		Last Modified: Wed, 16 Aug 2023 14:27:12 GMT  
		Size: 40.8 MB (40845875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526de63fdf58a686f90b02d93bf4f21da7fabebafc1c29ccc164ad58d87fe2c6`  
		Last Modified: Wed, 16 Aug 2023 14:27:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3cba925c676ed5ceb2b3eb77d1791ee96304c5e207062b2d14655c58e75a55`  
		Last Modified: Wed, 16 Aug 2023 14:27:08 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5717c5a3f42cc42bc36393059a3ddf96fa851ef37d3f808ae11b384b9965b37c`  
		Last Modified: Wed, 16 Aug 2023 22:15:53 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d0c7a43448dc3a89b73b827ba83399a7cf4a8f95a95719cced14cbbd26b9e`  
		Last Modified: Wed, 16 Aug 2023 22:19:38 GMT  
		Size: 11.3 MB (11333706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac88afe182d2e7bbb259a2bd3b9f6889ac3249fdfa3ddde62353326f4281966`  
		Last Modified: Wed, 16 Aug 2023 22:19:38 GMT  
		Size: 455.9 KB (455873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bbf0b31af6b76f6614c2a0a323e5485c306cf167cc988092090e868561a31a`  
		Last Modified: Wed, 16 Aug 2023 22:19:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:bc144ba1140b8d6c13d77f171579865c722bf0e8e4ad726afdff5233cc015d8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102556186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56cb6f63aed3057200809ee244f53034318da0c906932500c1108725be90deb`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 00:18:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 00:18:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 00:18:19 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:19:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:19:32 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 08 Aug 2023 19:20:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 08 Aug 2023 19:20:35 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Mon, 14 Aug 2023 18:09:21 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:21 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 19:53:12 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 14 Aug 2023 19:53:12 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 19:53:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 14 Aug 2023 19:53:14 GMT
WORKDIR /usr/local/tomcat
# Mon, 14 Aug 2023 19:53:15 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 19:53:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 20:05:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 14 Aug 2023 20:06:00 GMT
ENV TOMCAT_MAJOR=8
# Wed, 16 Aug 2023 00:28:50 GMT
ENV TOMCAT_VERSION=8.5.92
# Wed, 16 Aug 2023 00:28:50 GMT
ENV TOMCAT_SHA512=faab13a29531a800d38b2602ff76c0041277ffbfb25b938bbefb84ef6ad3ffa26d2c2645cd233eb0d819bcca9887aaeb44df6c044852160d000e5084b1addc2f
# Wed, 16 Aug 2023 00:28:51 GMT
COPY dir:464ab21a314a4e136e92b56893500a6d78b2853943b0a73f64e0abcf17ab6d0b in /usr/local/tomcat 
# Wed, 16 Aug 2023 00:29:01 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:29:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 16 Aug 2023 00:29:05 GMT
EXPOSE 8080
# Wed, 16 Aug 2023 00:29:06 GMT
ENTRYPOINT []
# Wed, 16 Aug 2023 00:29:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2f5a106d782ce62a5cf92c2a7f53d1b6067d5198e321d1c74bf914ae7b208f`  
		Last Modified: Tue, 08 Aug 2023 19:28:59 GMT  
		Size: 13.8 MB (13770640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a0298dd37fe55e86da60d8f404cf7915b9156664a97446948055249f57ac88`  
		Last Modified: Tue, 08 Aug 2023 19:30:25 GMT  
		Size: 41.2 MB (41229745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a632ba128c74bda719caf4495e6f6066f2bf8249478b0aeeba5f01098beb93e2`  
		Last Modified: Tue, 08 Aug 2023 19:30:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd00f36d8da81151399cba17d54a920e3c76bbabc9d975b4287bc13d1c02c93d`  
		Last Modified: Mon, 14 Aug 2023 18:13:12 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21846e8bf4dc77cdbd9dfa55b4c499b7515b07a82e557b59d61fed0e5d1f06e`  
		Last Modified: Mon, 14 Aug 2023 20:19:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6ee3c9b4df22c1ea5ba3f1030cc5a4e6b6b92eca1c727a48815ce921882aff`  
		Last Modified: Wed, 16 Aug 2023 00:48:10 GMT  
		Size: 11.4 MB (11356247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af972a95d7aaa0b2218d3f984de1fe90a852a5d80fe26963b24a2fc1db527f7`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 486.9 KB (486888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31dc55c3fc7117c06ce9aefb17ee82b2bf3c958224d8fbf4682bab2e1282b91`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
