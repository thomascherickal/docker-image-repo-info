## `tomcat:9-jre11-temurin-jammy`

```console
$ docker pull tomcat@sha256:71662ebecbb7fab1c9c299a910c00a613a84fe7059fc736a1fb77c5859b365a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:9-jre11-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:dd18a54fd7a10c177adcc75316f622dd2dab80654a143d9366f0191ee8108ed0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102167788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bf1a336c6c837988ae00fe9ab5c01f5998d626cd0deffba796c30657d4c33e8`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:01:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:01:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:01:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:01:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:02:42 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 04:03:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:03:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 10:46:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 10:46:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:47:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 10:47:00 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 10:47:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:47:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:49:42 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 10:49:42 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 10:49:42 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 10:49:42 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 10:49:43 GMT
COPY dir:cc994c361b6606d436cb5b6a6d18f02d79333bbedec62fd309c328d3a6110831 in /usr/local/tomcat 
# Thu, 02 Mar 2023 10:49:47 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 10:49:48 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 10:49:48 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 10:49:48 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3e3d5d30a242b64d6ee4089176f1459cdfe9d3aeb58e2114cc14b420ad71e5`  
		Last Modified: Thu, 02 Mar 2023 04:07:58 GMT  
		Size: 12.4 MB (12432173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1afd9b3f07bf59f1db11ac95908fa4840bb36ea5ca2e38380ceb99feadec711`  
		Last Modified: Thu, 02 Mar 2023 04:10:00 GMT  
		Size: 46.6 MB (46635570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c021f0294c1a9786718db8f4082e50bb41ec03fdc866e6fdb1e624b899367f`  
		Last Modified: Thu, 02 Mar 2023 04:09:54 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c0466cd5772f2dc1cc3012e581ad983c38a42dc0b4150a2aaf64f22cc586ce`  
		Last Modified: Thu, 02 Mar 2023 11:03:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f08ce71bec2902df5010c44023c247c581ac0d5555966c393261a959130b2d`  
		Last Modified: Thu, 02 Mar 2023 11:06:02 GMT  
		Size: 12.2 MB (12215391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38409d4fe39a448b6539b72b9639415d7b2ae0270790e9b7f61be763c36ade1`  
		Last Modified: Thu, 02 Mar 2023 11:06:01 GMT  
		Size: 454.2 KB (454193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69660b09776f21fed3dec1480b6a38c21fe100110fa28b0a22fb20a9a628a75d`  
		Last Modified: Thu, 02 Mar 2023 11:06:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:bf4f5114a6510825f5fee491dea99050340960bb72e56881866545eb6baf6910
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.4 MB (96435796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842bf4aab53d04615b39b66aa27fcaac911da3c722bca2b3e1187ad923297c12`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 10:59:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 10:59:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:59:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 11:00:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:01:30 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 11:02:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 11:02:02 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 12:58:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 12:58:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 12:58:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 12:58:59 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 12:59:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 12:59:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 13:01:27 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 13:01:27 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 13:01:27 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 13:01:27 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 13:01:28 GMT
COPY dir:9ef57444c347aa1bfc8516325ca27717bc09ba00f5d93f08a6059b34855901d3 in /usr/local/tomcat 
# Thu, 02 Mar 2023 13:01:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 13:01:33 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 13:01:33 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 13:01:33 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7f8907def135ff9e4431f5006bfdfd54de1a11b40a6400a2ba91bc407d9d89`  
		Last Modified: Thu, 02 Mar 2023 11:07:07 GMT  
		Size: 12.0 MB (11993099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630c356e01a041e4fef009a25372c90857973a54f5830ecc1d788d93f70fcf67`  
		Last Modified: Thu, 02 Mar 2023 11:09:15 GMT  
		Size: 44.8 MB (44842666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b8af2b190da6223f5b59d3fac2fae61cf3363fb0f3f7743daec5121683c392`  
		Last Modified: Thu, 02 Mar 2023 11:09:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350673df038efb2a2a1211c837b784c32efb05720415df6f68a312c18a4d9428`  
		Last Modified: Thu, 02 Mar 2023 13:21:07 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26df53119cc11b13784d9d6d72fe8d7fa08f8ad9f56126c8e7415af0fae8545c`  
		Last Modified: Thu, 02 Mar 2023 13:24:06 GMT  
		Size: 12.1 MB (12147402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4a1a08aeadb19e4e72f667b56f9f8253618c5fdbde56bb374c2c4d9c8475b0`  
		Last Modified: Thu, 02 Mar 2023 13:24:05 GMT  
		Size: 427.7 KB (427677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3436611b750ec4977c4b2504b448146eee9650d1eb71391ec33dea9a1bd0705`  
		Last Modified: Thu, 02 Mar 2023 13:24:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:e8ffea53d0f2867d76521a189eaa7af9786f6ae9f13c16613cc7e3bd2fbe0b82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.4 MB (98431651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42100b97912abc4ab8ba6bbbb556a1871289843963d01e2657a7120fdd8994c7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:27:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:27:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:27:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:27:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:28:47 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 04:29:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:29:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 07:44:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 07:44:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:44:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 07:44:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 07:44:27 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:44:27 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:46:39 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 07:46:39 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 07:46:40 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 07:46:40 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 07:46:40 GMT
COPY dir:ac9f2356480994f9e8ff7dcf59fcdf5db26394f5bc3c173f9ddc409d23b6f2bd in /usr/local/tomcat 
# Thu, 02 Mar 2023 07:46:43 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:46:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 07:46:44 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 07:46:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ba20309dcd99cff3a43c2f3c01df9170ee1fe02df71ead98cfcef30b9c450`  
		Last Modified: Thu, 02 Mar 2023 04:33:24 GMT  
		Size: 12.4 MB (12390219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d5722bd69e931b1cf3e955e992893a8ea2e124b586c19b553fbe8a2d94f988`  
		Last Modified: Thu, 02 Mar 2023 04:35:11 GMT  
		Size: 45.0 MB (44977970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d1016d6ffd5bed4cc6724687b1659787f8e3d1c112f02173b5efcb5425180`  
		Last Modified: Thu, 02 Mar 2023 04:35:06 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f31cf77054a813fd2027944ece84d43497ed9c07608a3226933ae3158c327`  
		Last Modified: Thu, 02 Mar 2023 07:59:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aa1db7703a378aa73b2665bea1c65ba960c7fc3cf5bf8129b30b4f64b6b1a7`  
		Last Modified: Thu, 02 Mar 2023 08:01:43 GMT  
		Size: 12.2 MB (12221376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad1864467dddc9c44bb49ea6cbb7d4e46e8d69b6545ebd4435ec4f747f57de`  
		Last Modified: Thu, 02 Mar 2023 08:01:42 GMT  
		Size: 453.7 KB (453705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8389739cfcc6c3d2c94138cff5238142ff63934cd5f4c8a659749b62664c2efa`  
		Last Modified: Thu, 02 Mar 2023 08:01:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:afa4342e91c8a24054aa6b62474382ccdda14341826efaccfb4abfcb81801a58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.8 MB (103753369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8bb5e0515f171d367b0e854c69015e69b2d0e3d8c6b643dadef70459fae18a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:04:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:04:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:04:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:05:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:07:30 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 04:08:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:08:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 06:36:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 06:36:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 06:37:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 06:37:02 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 06:37:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:37:04 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:46:15 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 06:46:15 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 06:46:16 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 06:46:16 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 06:46:17 GMT
COPY dir:572e6f533b8ca5b03103bd7d036f0b3dbd8f86cca1334ee5f1a3f0aab3993e73 in /usr/local/tomcat 
# Thu, 02 Mar 2023 06:46:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 06:46:34 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 06:46:35 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 06:46:35 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121eddcd73312db262a7816616eb5c5d347769495ce897aef3f86e63aa00c644`  
		Last Modified: Thu, 02 Mar 2023 04:18:05 GMT  
		Size: 13.2 MB (13246165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da86c679cbca743536591fcdae611bf818c79bd370a112424b49c2710ed5727`  
		Last Modified: Thu, 02 Mar 2023 04:20:56 GMT  
		Size: 42.1 MB (42064908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eea8d62076b3ca37042a51c336ecdde73f2309cdd7449fb46c9ba377a2a351`  
		Last Modified: Thu, 02 Mar 2023 04:20:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1d4a073f6163dbeda08ef02e8091e9f7e75026206ba0932f384f8556c8845d`  
		Last Modified: Thu, 02 Mar 2023 07:22:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c64eeeef657da2913ef10089575b258327ca3455924a5374f5a578606ed035`  
		Last Modified: Thu, 02 Mar 2023 07:25:54 GMT  
		Size: 12.2 MB (12244616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e156f5085089c1a05c49fd353f4ab191f37ecbfb684ffc90d54072907957ce5c`  
		Last Modified: Thu, 02 Mar 2023 07:25:53 GMT  
		Size: 485.6 KB (485629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6216ac4bc7e24e3caa265250314650966f6afbfdbb50898070783046012156cf`  
		Last Modified: Thu, 02 Mar 2023 07:25:52 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:40b722d2595370c63ba05ffface4fb116398e3ec77f577f147ca18b6e750cfb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.5 MB (96520692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2513383c8cf57ada9e177a3e6c4da6a2fc8fdb498854ba8a1deb1667e8deae95`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:59:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:59:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:59:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 17:59:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:15 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 31 Jan 2023 17:59:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 18:00:00 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 19:54:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Jan 2023 19:54:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 19:54:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Jan 2023 19:54:37 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Jan 2023 19:54:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 19:54:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 19:58:15 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 31 Jan 2023 19:58:15 GMT
ENV TOMCAT_MAJOR=9
# Sat, 25 Feb 2023 00:08:09 GMT
ENV TOMCAT_VERSION=9.0.72
# Sat, 25 Feb 2023 00:08:09 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Sat, 25 Feb 2023 00:08:09 GMT
COPY dir:ad5bee10310077f6e510fc20f3ae597be25c7aaad53d9a681d57c174571f5a18 in /usr/local/tomcat 
# Sat, 25 Feb 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Feb 2023 00:08:16 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 25 Feb 2023 00:08:16 GMT
EXPOSE 8080
# Sat, 25 Feb 2023 00:08:17 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e61b13b86195413895b2e2ae4499c0123469558bfd3409aeb3edaada381f0a`  
		Last Modified: Tue, 31 Jan 2023 18:05:26 GMT  
		Size: 12.5 MB (12479720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abde70ae404bb211010de2b02e3ce57dd40af0f4f2d0f5d543c0d3e57c726fa`  
		Last Modified: Tue, 31 Jan 2023 18:06:07 GMT  
		Size: 40.5 MB (40535939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d1a40ebfac29aba7f7d31c33d9ea71ada590a146b3530de588beb2c60d5460`  
		Last Modified: Tue, 31 Jan 2023 18:06:01 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ee99ef021fa47648b0e8d4e711cf1266fd5d741c85050e0819907c3c5316f4`  
		Last Modified: Tue, 31 Jan 2023 20:09:05 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc21413c5043d99b5a74aa29f0faeb071f3d344263e4ad01a75d33229b468c`  
		Last Modified: Sat, 25 Feb 2023 00:21:44 GMT  
		Size: 12.2 MB (12212529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d335b8079f77b1fa5a46f60ed07c85bae8391946a1c977abb625f91ba3a632`  
		Last Modified: Sat, 25 Feb 2023 00:21:43 GMT  
		Size: 2.7 MB (2650115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c5f4ebbc454c6263152fac338167d2d11e9647e9db021c0256c224331e0aac`  
		Last Modified: Sat, 25 Feb 2023 00:21:43 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
