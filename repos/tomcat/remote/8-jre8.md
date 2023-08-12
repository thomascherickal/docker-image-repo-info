## `tomcat:8-jre8`

```console
$ docker pull tomcat@sha256:2b5171410955c0e785c280817c7550a6076d96cfc9b25b38f288ea5462b37187
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:8-jre8` - linux; amd64

```console
$ docker pull tomcat@sha256:2d84e2d40afca85b9db33f057ec8e4587fdae4308c0889ea58137308b4d075c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96964937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e0353c14be3a26423464caf8225acf21ff990b448d6078348e183489d9eb1b3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:33:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:33:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:33:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:21:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:21:02 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 08 Aug 2023 19:21:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 08 Aug 2023 19:21:35 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 08 Aug 2023 19:21:35 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:21:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:23:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:23:45 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:23:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:23:46 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:23:46 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:23:46 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:28:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 08 Aug 2023 21:29:00 GMT
ENV TOMCAT_MAJOR=8
# Tue, 08 Aug 2023 21:29:00 GMT
ENV TOMCAT_VERSION=8.5.91
# Tue, 08 Aug 2023 21:29:00 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Tue, 08 Aug 2023 21:29:00 GMT
COPY dir:b9f5e53e045a58e3f0a82de8522d99cdeab16329f4412ae9ceed4d3387b17161 in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:29:04 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:29:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:29:05 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:22:19 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:22:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1d9603a2223f0c0337b5489031adc59113c119d64dfce6852f6114f42f2f05`  
		Last Modified: Tue, 08 Aug 2023 19:27:08 GMT  
		Size: 12.9 MB (12902861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a576d6a0d2efa763e6b6ce16640dc71b247749a6b110c4f1d29204f07f58b86e`  
		Last Modified: Tue, 08 Aug 2023 19:28:20 GMT  
		Size: 41.9 MB (41851990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa50292584c003c7b42874eed2834511e81c5ba97c1dc0226ee157070373774`  
		Last Modified: Tue, 08 Aug 2023 19:28:15 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f855056850dfcc3d0c1187544169b8e9684f8171dfd16ce248f2738000c71620`  
		Last Modified: Tue, 08 Aug 2023 19:28:15 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d59edba175c2ebb6bcc499ef14ef306db12004bb3ccda083a50f2d5955d16`  
		Last Modified: Tue, 08 Aug 2023 21:37:33 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf0147500805c5386c7b77a8e1595f2362225786f12a2b564ece8b9d275a707`  
		Last Modified: Tue, 08 Aug 2023 21:41:34 GMT  
		Size: 11.3 MB (11322098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504f23452ee6858248191c962553fb7deb31468bde7cab1416d777cad4a01bc8`  
		Last Modified: Tue, 08 Aug 2023 21:41:33 GMT  
		Size: 455.6 KB (455627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d2f6914d21c92a568ff6c995cee09a7d4c8ee8f15a2e4e56d339c38778bd42`  
		Last Modified: Tue, 08 Aug 2023 21:41:33 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:461f89cf557fb9c0c9892d0f51778a1fab7674abbffcebb93174d459f651688e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.5 MB (91545553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42da9de8cb1d944a62bde9b8180bc49382ec5aa99f4e8164e404cc7bc2c167dd`
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
# Tue, 08 Aug 2023 18:59:44 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 18:59:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 20:00:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 20:00:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:00:52 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 20:00:52 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 20:00:53 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 20:00:53 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 20:05:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 08 Aug 2023 20:05:43 GMT
ENV TOMCAT_MAJOR=8
# Tue, 08 Aug 2023 20:05:43 GMT
ENV TOMCAT_VERSION=8.5.91
# Tue, 08 Aug 2023 20:05:43 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Tue, 08 Aug 2023 20:05:44 GMT
COPY dir:6fa03df03c930face7bd40f4dd34895cbb8a7cdeec68d99c24f2cdc8c6eae756 in /usr/local/tomcat 
# Tue, 08 Aug 2023 20:05:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 20:05:50 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 20:05:50 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:26:17 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:26:18 GMT
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
	-	`sha256:702d75f83f116f2aa335a26b157e7143ca6ae05f822bd5e6d640044d4844fa82`  
		Last Modified: Tue, 08 Aug 2023 19:03:30 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c18d1a60a011082aa980e01d29d7784a4699f2142007825ad9817e974d87cbd`  
		Last Modified: Tue, 08 Aug 2023 20:14:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b2c8dbde22a67ec93962c4db58a1944550aec8edb8510f299237b592a9f441`  
		Last Modified: Tue, 08 Aug 2023 20:18:09 GMT  
		Size: 11.3 MB (11254618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38add1d918cdd228adf82ffce656de4e09f71b03da0d48ce9621cf3c638e2406`  
		Last Modified: Tue, 08 Aug 2023 20:18:08 GMT  
		Size: 429.6 KB (429553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25a6384d69a33a6f27d585ff4dca50f30ab7f9a8304ba7ffbf27db4c73df165`  
		Last Modified: Tue, 08 Aug 2023 20:18:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:a869050d57c688ada30e426e76b87e2f5098da7b5a3986b3bdf1548f7fe02596
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93868400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6a3d9154bc0633c1f9857678f706e1a045eabaccb725110fd60dc24b88c285`
-	Default Command: `["catalina.sh","run"]`

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
# Tue, 08 Aug 2023 19:40:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:40:41 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Tue, 08 Aug 2023 19:41:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 08 Aug 2023 19:41:03 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 08 Aug 2023 19:41:03 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:41:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 22:39:12 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 22:39:12 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:39:13 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 22:39:13 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 22:39:13 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 22:39:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 22:43:24 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 08 Aug 2023 22:43:24 GMT
ENV TOMCAT_MAJOR=8
# Tue, 08 Aug 2023 22:43:24 GMT
ENV TOMCAT_VERSION=8.5.91
# Tue, 08 Aug 2023 22:43:25 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Tue, 08 Aug 2023 22:43:25 GMT
COPY dir:b94ab3b8d3a9af13e7507074006d86c228a351a6619f5a74d949d9754d05d591 in /usr/local/tomcat 
# Tue, 08 Aug 2023 22:43:28 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 22:43:29 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 22:43:29 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 01:07:32 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 01:07:32 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91712d801b234a271df55fd60b35e7d2918ce5ae0fb7ce56a8de0edb8151fd0e`  
		Last Modified: Tue, 08 Aug 2023 19:44:21 GMT  
		Size: 12.8 MB (12844180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4729969e9cc70325084074568e57d6d47ab5f017d72a01a263e276d3163c976c`  
		Last Modified: Tue, 08 Aug 2023 19:45:17 GMT  
		Size: 40.8 MB (40845812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b211a894e85210fc6d9125093ffdab6bec0324b1dfc15872deb9d95e05a122`  
		Last Modified: Tue, 08 Aug 2023 19:45:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888221d0d24b27dea55656661c27e8148fcbe841d3ac1e918df308718c43036`  
		Last Modified: Tue, 08 Aug 2023 19:45:13 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f838e6579c988914cd0f73f4c2e61ef3b02ec9b323194f91f5fe32d6aeb46449`  
		Last Modified: Tue, 08 Aug 2023 22:51:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2293a7329fe8013c9779dda3f29bd81683f06c377be41b0a7fac105392f6266`  
		Last Modified: Tue, 08 Aug 2023 22:55:39 GMT  
		Size: 11.3 MB (11330342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d9d1d35f2f9667807d4eac3c32a1efce8e46502e77531eef2cad7a731c0476`  
		Last Modified: Tue, 08 Aug 2023 22:55:38 GMT  
		Size: 455.9 KB (455928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ec5600d089e2a14ae17a2174c13e47844ade7251a2778fdc5ed66a7004d86f`  
		Last Modified: Tue, 08 Aug 2023 22:55:38 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8` - linux; ppc64le

```console
$ docker pull tomcat@sha256:74c8df8c0245d0740eb9cc02c636fdc9ed8d6ced353044f97d5227d179934dec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102548994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54a5189a8d93fd20057c8136edf4184faf1f35735b16e111b7c97fe9a71238c4`
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
# Tue, 08 Aug 2023 19:20:35 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:17:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:17:31 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:17:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:17:33 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:17:34 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:17:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:32:26 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 08 Aug 2023 21:32:26 GMT
ENV TOMCAT_MAJOR=8
# Tue, 08 Aug 2023 21:32:27 GMT
ENV TOMCAT_VERSION=8.5.91
# Tue, 08 Aug 2023 21:32:27 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Tue, 08 Aug 2023 21:32:28 GMT
COPY dir:5c537ee70ca2608423116992dc802d10a6afe8c5eba558fe8e10e7666b825250 in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:32:41 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:32:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:32:44 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:17:12 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:17:13 GMT
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
	-	`sha256:9b473565a12ecd6fc818e1353d204dbd79e69447e13d903260b75617df8129f2`  
		Last Modified: Tue, 08 Aug 2023 19:30:17 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb130c2a84f73b97c42e00d2eb4134f760df81c2bb34b390941885c05d1f6fb4`  
		Last Modified: Tue, 08 Aug 2023 21:45:59 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a286705ba78a06ae4aa55d3cf24d8967921e74d162718164a954b4a6d3bd0a`  
		Last Modified: Tue, 08 Aug 2023 21:51:50 GMT  
		Size: 11.3 MB (11349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9070fc4ecd50e6ee53c5a7b446dbf3482e34714e142ec073edb545f22b7eaac`  
		Last Modified: Tue, 08 Aug 2023 21:51:49 GMT  
		Size: 486.9 KB (486877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b8d64082f36c396a5763bdd729dd28a205deff92b5e73c9daedb2af56da36`  
		Last Modified: Tue, 08 Aug 2023 21:51:49 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
