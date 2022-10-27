## `tomcat:jre17-temurin-jammy`

```console
$ docker pull tomcat@sha256:97e5ef00ffe469ec8b3134ea01a8e844accebb23350955e265242d462be7db29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre17-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:6a640838eb0deb26708954071891077fede0585952474439e61349fc953b52a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106653347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7979b6bb99bea8e8ca3785179622d08d1629126afa87b32bfff72f07258f79`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:41 GMT
ADD file:ba96f963bbfd429a0839c40603fdd7829eaca58f20adfa0d15e6beae8244bc08 in / 
# Tue, 25 Oct 2022 01:53:41 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:27:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 17:27:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 17:27:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 17:30:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 17:30:25 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Tue, 25 Oct 2022 17:30:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 25 Oct 2022 17:31:00 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 23:43:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 23:43:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 23:43:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 23:43:28 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 23:43:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:43:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 23:43:28 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Oct 2022 23:43:29 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Oct 2022 23:43:29 GMT
ENV TOMCAT_VERSION=10.1.1
# Wed, 26 Oct 2022 23:43:29 GMT
ENV TOMCAT_SHA512=5718b877eb2d3fb05ec0c11d0af8a2bb34766e14b915ecda8d61e92670a7a911ff08c3cb03dafe8f28f10df19172ca0681ade953ccda5363fc5b57468a47476c
# Wed, 26 Oct 2022 23:43:29 GMT
COPY dir:c5820cf594f63c63f958c06b25b760b350f580afd47ca3c6c98e041fac9ca630 in /usr/local/tomcat 
# Wed, 26 Oct 2022 23:43:34 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 23:43:36 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 23:43:36 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 23:43:36 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:301a8b74f71f85f3a31e9c7e7fedd5b001ead5bcf895bc2911c1d260e06bd987`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 30.4 MB (30426374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c735a83dbd58e1c83f8d52abdc51068e27c00405f53d59802d4954a6b5398a`  
		Last Modified: Wed, 26 Oct 2022 16:46:13 GMT  
		Size: 17.0 MB (16988718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb350608a356dc75407035af5f5902a4f24e0383b5b143fa952276746d837f5`  
		Last Modified: Wed, 26 Oct 2022 16:47:02 GMT  
		Size: 46.8 MB (46806002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e2f77c71f18a74f8fee99211d10a82647b8c21ceb669c1d21764bd8240746d`  
		Last Modified: Wed, 26 Oct 2022 16:46:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e910be9949ff71ea2087be78dcdf6e63601e6712c12e482afbd6d4375a2b102e`  
		Last Modified: Thu, 27 Oct 2022 00:05:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e95f4f874c192e8e7f15584a90c37bcc28b0e14c3f142c8b841a9a30c57953`  
		Last Modified: Thu, 27 Oct 2022 00:05:05 GMT  
		Size: 12.0 MB (11976138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94fa47e8115e9c85bee22e6f25282197e70d2e76b3b030db56f6710b3718cd57`  
		Last Modified: Thu, 27 Oct 2022 00:05:04 GMT  
		Size: 455.7 KB (455652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f16ea04b1a495d5b6bb8aa9d2e15975015d9b40f7152f76cab80ee871a4512`  
		Last Modified: Thu, 27 Oct 2022 00:05:03 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:b3d98a4b5c97045171c59cd7e6f462e44c012bf2fd9d4b38006a448d0a128a9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100841693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc41bc3756d5ec96236c6f6d66a702d774081fa516773324b379e22800cb3f7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:57 GMT
ADD file:11e25fc4812528219464289700bb0495bf9298918899103c33d7ef9022690eb0 in / 
# Wed, 05 Oct 2022 00:13:57 GMT
CMD ["bash"]
# Thu, 06 Oct 2022 06:30:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 06 Oct 2022 06:30:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 06:30:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 06 Oct 2022 06:34:20 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 06:34:20 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Thu, 06 Oct 2022 06:35:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 06 Oct 2022 06:35:46 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 07 Oct 2022 06:07:28 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 07 Oct 2022 06:07:28 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 06:07:29 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 07 Oct 2022 06:07:29 GMT
WORKDIR /usr/local/tomcat
# Fri, 07 Oct 2022 06:07:29 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:07:29 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 07 Oct 2022 06:07:30 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 07 Oct 2022 06:07:30 GMT
ENV TOMCAT_MAJOR=10
# Fri, 14 Oct 2022 11:33:53 GMT
ENV TOMCAT_VERSION=10.1.1
# Fri, 14 Oct 2022 11:33:53 GMT
ENV TOMCAT_SHA512=5718b877eb2d3fb05ec0c11d0af8a2bb34766e14b915ecda8d61e92670a7a911ff08c3cb03dafe8f28f10df19172ca0681ade953ccda5363fc5b57468a47476c
# Fri, 14 Oct 2022 11:33:55 GMT
COPY dir:c780754084c36cfe40584632e87bcb574e9cc0579220e7f58305f998e13d4498 in /usr/local/tomcat 
# Fri, 14 Oct 2022 11:34:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 14 Oct 2022 11:34:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 14 Oct 2022 11:34:06 GMT
EXPOSE 8080
# Fri, 14 Oct 2022 11:34:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:99b9c73338a7c0dbe41f9fc543fae706650a616453e1e330f870e20916c18a11`  
		Last Modified: Wed, 05 Oct 2022 00:16:02 GMT  
		Size: 27.0 MB (27018632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef04b7f991520bc7a47731dace44051d5a194dafd5da570405d58ec4729acd2e`  
		Last Modified: Thu, 06 Oct 2022 06:42:55 GMT  
		Size: 17.1 MB (17105130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b39d668ad60486faa2c12674c151674b5959995e6d18393b9bde02573f8d79`  
		Last Modified: Thu, 06 Oct 2022 06:43:48 GMT  
		Size: 44.3 MB (44341171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e9242cdb5165313e943f4655684124b4b115282604725e8f8849db88eb8c8`  
		Last Modified: Thu, 06 Oct 2022 06:43:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b285cab1d120ecaf340c1034432ac8f4b11fa2be892b0e1428da6c3838c0122f`  
		Last Modified: Fri, 07 Oct 2022 06:47:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c71e194946fdbe02e864dd86c52ccba1e2f8011477cbd5a13ac9f27edf4757`  
		Last Modified: Fri, 14 Oct 2022 11:51:49 GMT  
		Size: 11.9 MB (11947998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c5284e3d54dad08e995e4a15120d9d8ccef4d44cd6dbc84e211a8547366f0`  
		Last Modified: Fri, 14 Oct 2022 11:51:48 GMT  
		Size: 428.3 KB (428300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142eee1601a8243565447c28564c5259d5acc431f1f16d61a3c5c2aaabf90cd6`  
		Last Modified: Fri, 14 Oct 2022 11:51:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:37289cee2799f3108b130510cbd18a863056881c62405f07b0e7f81287b3b6bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105479691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bac3d07a10992b64faf80681038f6ae634e25c1a055aac5c903d6917a705cd1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:08:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:08:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:12:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:12:19 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 26 Oct 2022 01:13:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Oct 2022 01:13:19 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 17:10:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 17:10:21 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 17:10:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 17:10:21 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 17:10:21 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:10:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:10:22 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Oct 2022 17:10:22 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Oct 2022 17:10:22 GMT
ENV TOMCAT_VERSION=10.1.1
# Wed, 26 Oct 2022 17:10:22 GMT
ENV TOMCAT_SHA512=5718b877eb2d3fb05ec0c11d0af8a2bb34766e14b915ecda8d61e92670a7a911ff08c3cb03dafe8f28f10df19172ca0681ade953ccda5363fc5b57468a47476c
# Wed, 26 Oct 2022 17:10:22 GMT
COPY dir:6dc021b133b3928ec7c350559032068548aeadd15c2b4ebcfd57932282254464 in /usr/local/tomcat 
# Wed, 26 Oct 2022 17:10:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 17:10:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 17:10:26 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 17:10:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbcda71286ccda82b38ebdb092380175412af668b5afa39d175cd3cdefd14e4`  
		Last Modified: Wed, 26 Oct 2022 01:20:19 GMT  
		Size: 18.4 MB (18418404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838c47d4ccd4c9637ebc935de9583aab3f0b4719e112424c11da1f5f56755933`  
		Last Modified: Wed, 26 Oct 2022 01:21:30 GMT  
		Size: 46.2 MB (46246685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b495c3c13700e6e9dd6bf6ac30bf068feff8fe32db726f7ee1578338d9e0fd`  
		Last Modified: Wed, 26 Oct 2022 01:21:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7429951a4e43a58e6daf1fa6ca3f5737008e0664bf4d375cb3b2100726eaa753`  
		Last Modified: Wed, 26 Oct 2022 17:34:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f80a5a57ca34df95ce7e1d3869341462c7203f47ea5e5526416feec890afdba`  
		Last Modified: Wed, 26 Oct 2022 17:34:23 GMT  
		Size: 12.0 MB (11977071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d931695eb6519bdc43bab132de21e8692e5026359b468b4168467d375b8a670`  
		Last Modified: Wed, 26 Oct 2022 17:34:22 GMT  
		Size: 454.6 KB (454579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe150c9d5cdfe45e6eac59530f5481b317b0dcb5c1cf137155f194b1aca33b7`  
		Last Modified: Wed, 26 Oct 2022 17:34:22 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:c5a6b60e0a226a7c28bbf613b2ce4dfef1e17b339ad449dc71e9fa1811b66d52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113077886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd062f98e3939d2a6dc9bd559ad8497a664c6d9520975c380c09297d88dd1f22`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:00 GMT
ADD file:766b7743de4ed1a194fc749b7649d245b0cd545b03cc2c81f16a6c15e91c87e7 in / 
# Tue, 25 Oct 2022 03:26:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:47:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 13:47:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 13:47:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 13:52:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 13:52:28 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Tue, 25 Oct 2022 13:53:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 25 Oct 2022 13:53:36 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 01:58:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 01:58:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:58:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 01:58:51 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 01:58:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 01:58:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 01:58:52 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Oct 2022 01:58:53 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Oct 2022 01:58:53 GMT
ENV TOMCAT_VERSION=10.1.1
# Wed, 26 Oct 2022 01:58:54 GMT
ENV TOMCAT_SHA512=5718b877eb2d3fb05ec0c11d0af8a2bb34766e14b915ecda8d61e92670a7a911ff08c3cb03dafe8f28f10df19172ca0681ade953ccda5363fc5b57468a47476c
# Wed, 26 Oct 2022 01:58:55 GMT
COPY dir:cd2c31ae7f3aec4f9ff4f6d70beee38f7c52e3f02537174177fd5c3cf18a3613 in /usr/local/tomcat 
# Wed, 26 Oct 2022 01:59:04 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:59:08 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 01:59:09 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 01:59:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aa33126e789290559dc146af02cbf168119ed23be1e30fd99fe8572956e50616`  
		Last Modified: Tue, 25 Oct 2022 03:28:08 GMT  
		Size: 35.7 MB (35709401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7706378e88f22b868f467afb7f92be779183ac279b698a8ec90dc640193294`  
		Last Modified: Tue, 25 Oct 2022 14:03:02 GMT  
		Size: 18.3 MB (18269422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22cf96acbbb0c7a6b494e3558625ecd86e4a9472e076d0b6a43479a3cc4ca51`  
		Last Modified: Tue, 25 Oct 2022 14:04:18 GMT  
		Size: 46.6 MB (46620361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f1f5950d18761ee75b1ea80e79434480d99312f3f04acc182d8bc35d216440`  
		Last Modified: Tue, 25 Oct 2022 14:04:06 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10e2268041666f65a0762f04e3bde80447811241c766c7df2f90862228308b6`  
		Last Modified: Wed, 26 Oct 2022 02:39:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68113b98658199e275e19971a6bff1278d5982856fac742d04566b66c70ef44d`  
		Last Modified: Wed, 26 Oct 2022 02:39:55 GMT  
		Size: 12.0 MB (11991606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8075cff8c3c5baa897660067f407f450e6c3e623b216168a7b60cd67bc2a318`  
		Last Modified: Wed, 26 Oct 2022 02:39:54 GMT  
		Size: 486.6 KB (486632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663022428673651671e36d4d2b278351e96ff6db64a678f1eafd45644a16f3d4`  
		Last Modified: Wed, 26 Oct 2022 02:39:54 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:3f2c2f438963883b399b67eda306b5efbdf7b9076ca61ba3a4b125672e33cbfd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101537647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ca9dcb0746fcecb0fc3bddc7ebc01dd2fa8e570918aca0d1fb7d82eed55056`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:21 GMT
ADD file:d9af7670f58e9478e400dac85a0fcb07a4209846dbd1ea560fdc6de6e2cb5e4e in / 
# Tue, 25 Oct 2022 01:23:22 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:00:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 09:00:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 09:00:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 09:04:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:04:28 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Tue, 25 Oct 2022 09:05:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 25 Oct 2022 09:06:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 25 Oct 2022 19:56:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 25 Oct 2022 19:56:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 19:56:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 25 Oct 2022 19:56:37 GMT
WORKDIR /usr/local/tomcat
# Tue, 25 Oct 2022 19:56:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 25 Oct 2022 19:56:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 25 Oct 2022 19:56:39 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 25 Oct 2022 19:56:39 GMT
ENV TOMCAT_MAJOR=10
# Tue, 25 Oct 2022 19:56:40 GMT
ENV TOMCAT_VERSION=10.1.1
# Tue, 25 Oct 2022 19:56:41 GMT
ENV TOMCAT_SHA512=5718b877eb2d3fb05ec0c11d0af8a2bb34766e14b915ecda8d61e92670a7a911ff08c3cb03dafe8f28f10df19172ca0681ade953ccda5363fc5b57468a47476c
# Tue, 25 Oct 2022 19:56:42 GMT
COPY dir:3ef6fc8672dbf2761482e4ac79a64c64aa6f230376c0b833bcf1fa8bd556c2c5 in /usr/local/tomcat 
# Tue, 25 Oct 2022 19:56:51 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 19:56:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 25 Oct 2022 19:56:57 GMT
EXPOSE 8080
# Tue, 25 Oct 2022 19:56:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9aed974aece14dd3aed00810d58a89e87eb5be9ad1c6fbb1ed077dc3f145dccc`  
		Last Modified: Tue, 25 Oct 2022 01:24:48 GMT  
		Size: 28.6 MB (28641668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5ef382f9cd7650f02bff84c04acf5fc944f0eca28369ddaee049c51d4700a7`  
		Last Modified: Tue, 25 Oct 2022 09:12:25 GMT  
		Size: 16.8 MB (16766701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970748761c44ed40f9a254e6eaa64b11e5e2a6bae1cb3e1e017e71c9516f8570`  
		Last Modified: Tue, 25 Oct 2022 09:13:07 GMT  
		Size: 43.7 MB (43693895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3ae0e17e3f60ed8a385e9f0c2cbabbfb2dddfae5583191161882ee85e6139a`  
		Last Modified: Tue, 25 Oct 2022 09:13:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085075141eb60b4a0213a8c2a295813c47da017f3d93ded14bc301c4d5216bd7`  
		Last Modified: Tue, 25 Oct 2022 20:25:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6646684d81e827bde9e13d6a6951083d364bae28dc5ecaa7e64b96c5c0c70a`  
		Last Modified: Tue, 25 Oct 2022 20:25:36 GMT  
		Size: 12.0 MB (11977864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63db740caf6be53c527444f31744b377fa7d124c92f3ab4a4d4a513e045b0a3`  
		Last Modified: Tue, 25 Oct 2022 20:25:36 GMT  
		Size: 457.1 KB (457056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039478186b4ebe9f90d4f92da43e181d1f182a28fbc603a8fcc348936cc93247`  
		Last Modified: Tue, 25 Oct 2022 20:25:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
