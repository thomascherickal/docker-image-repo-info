## `tomcat:8-jre17-temurin`

```console
$ docker pull tomcat@sha256:b87136d1b1385eb4cd19cf5b335279e68f46ec0609895f8724fa45d407e0e9f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre17-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:cdb6a67c4f100965d85bad2d54e92a04a41635e7e4d6bd01c9d17c55d632dead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.9 MB (105879317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6138c05c2a968f059860fc5dc63463169cd58935d8ca2bb48f920eff1ae3fe`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:03:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:03:02 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 17:03:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:03:38 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 05:17:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 05:17:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:17:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 05:17:41 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 05:17:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:17:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:28:58 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 06 Oct 2022 05:28:58 GMT
ENV TOMCAT_MAJOR=8
# Thu, 06 Oct 2022 05:28:58 GMT
ENV TOMCAT_VERSION=8.5.82
# Thu, 06 Oct 2022 05:28:59 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Thu, 06 Oct 2022 05:28:59 GMT
COPY dir:49c8f2a5ef933872fa064d7ba523d8254a7d13e3e9cf11e23fbeaf82bc4af7fd in /usr/local/tomcat 
# Thu, 06 Oct 2022 05:29:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 05:29:04 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 06 Oct 2022 05:29:04 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 05:29:04 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b295fc69f17be5773c7d5e868ebc3c55b8e7789141f3aa47363fa69a7a446c7a`  
		Last Modified: Wed, 05 Oct 2022 17:10:08 GMT  
		Size: 17.0 MB (16985789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a10c28b8897d0f71a9ac7980bacef2a2114ec865656d6b649a368ea6a2442cd`  
		Last Modified: Wed, 05 Oct 2022 17:10:58 GMT  
		Size: 46.8 MB (46806033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c5e2ea3700c0093714576c85d5cfda263673d3226441bdf70a90f41abe84a1`  
		Last Modified: Wed, 05 Oct 2022 17:10:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0e938c320315adc6aba77d6b6810574c78548e0829fdf5be1bf75729c0bb60`  
		Last Modified: Thu, 06 Oct 2022 05:38:16 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe87399e6b564ec85784105df71d42dd46c41ac4e78903ff95af516a9d442d93`  
		Last Modified: Thu, 06 Oct 2022 05:48:43 GMT  
		Size: 11.2 MB (11202434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717bf56bfba1ed29e408d911915bd0690e11e32efbcedb1f832fbf67ac2072cb`  
		Last Modified: Thu, 06 Oct 2022 05:48:42 GMT  
		Size: 455.7 KB (455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8211288c22f61c77d7220592691f1419fbd17de5234c10aabba04e40e1f33`  
		Last Modified: Thu, 06 Oct 2022 05:48:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:9ebdad0284a094aa333e9b392d39a3210950972b0f4cbf063973363512647ae0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (100029133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4535c4a7f8e7b203ef41b9096ef170d36150cdc34373451f42615733b4860f89`
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
# Fri, 07 Oct 2022 06:28:06 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 07 Oct 2022 06:28:06 GMT
ENV TOMCAT_MAJOR=8
# Fri, 07 Oct 2022 06:28:06 GMT
ENV TOMCAT_VERSION=8.5.82
# Fri, 07 Oct 2022 06:28:06 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Fri, 07 Oct 2022 06:28:08 GMT
COPY dir:e8d4307f0a31ae9a50224050937a832ddfcb561e23dd91420d4706b00861bf5a in /usr/local/tomcat 
# Fri, 07 Oct 2022 06:28:17 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Oct 2022 06:28:19 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 07 Oct 2022 06:28:20 GMT
EXPOSE 8080
# Fri, 07 Oct 2022 06:28:20 GMT
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
	-	`sha256:ece13840476a03a481a5cb16941d978f26e0cfc37af7dadeff304509a4140af6`  
		Last Modified: Fri, 07 Oct 2022 07:02:03 GMT  
		Size: 11.1 MB (11135467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da939cefe6f8f6fd6013b32ea8fba6b21673996b4a2d6107148760dd2bf8b42`  
		Last Modified: Fri, 07 Oct 2022 07:02:01 GMT  
		Size: 428.3 KB (428270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bd4f0faa065c0d09a7ecf832f78bda41b07cdf9eb268e6282a53479a0c04d`  
		Last Modified: Fri, 07 Oct 2022 07:02:01 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:303b562be0e4a64ad643fbfa7e9e16b82189e25431ae4e49e7e9b8e1c79b0097
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104471709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6eec68e67c7e08879a8c9e7fca12807c3ae3ba43664229991290d129e16d83`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:44:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 15:44:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 15:44:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 15:47:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:47:25 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 15:48:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 15:48:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 04:21:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 04:21:28 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 04:21:29 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 04:21:30 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 04:21:31 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 04:21:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 04:39:52 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 06 Oct 2022 04:39:53 GMT
ENV TOMCAT_MAJOR=8
# Thu, 06 Oct 2022 04:39:54 GMT
ENV TOMCAT_VERSION=8.5.82
# Thu, 06 Oct 2022 04:39:55 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Thu, 06 Oct 2022 04:39:57 GMT
COPY dir:534f0c9c2a7e3c05f641d7e5400687a04cb55364da212098650ef49a21f69d5e in /usr/local/tomcat 
# Thu, 06 Oct 2022 04:40:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 04:40:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 06 Oct 2022 04:40:06 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 04:40:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2306aaa12630b303ecdc2ba04820df277229a5f73a0aae69b54a606863c98ae`  
		Last Modified: Wed, 05 Oct 2022 15:55:24 GMT  
		Size: 18.4 MB (18418115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218e026bfcb12b8ddca62e4360eb84f7a324aede6f4ae29b7f4b103b7740225`  
		Last Modified: Wed, 05 Oct 2022 15:56:21 GMT  
		Size: 46.2 MB (46246844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001ee99a030d80784840c741848f01198b025655d16268546b0668e82f979380`  
		Last Modified: Wed, 05 Oct 2022 15:56:14 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e40ccb1423bc1a0da272df01337d6ab4b68d1d895c19e665044553b7e431701`  
		Last Modified: Thu, 06 Oct 2022 04:56:23 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4febc574c4a36773a837af400626c7c439490176e651172de772e903f835358`  
		Last Modified: Thu, 06 Oct 2022 05:08:55 GMT  
		Size: 11.2 MB (11207281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e842cb0b1633ecfa83cdad503a95a1d5615f69579cf9ad063a55f83f3e3f5e7`  
		Last Modified: Thu, 06 Oct 2022 05:08:54 GMT  
		Size: 216.9 KB (216916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:46cf790bc320561d9a40bbc9c52bbb9045bfdfcff800eb23c4a51214844e740c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112314528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385e4338a846d7b15eec96980a7d24f63f6ca24a7078dcaf50f7689df068e6a6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 05 Oct 2022 10:52:24 GMT
ADD file:5f3953a21754ce756642c9ddcf521f2cfe220a5fe988ccec51085bd074fbe46e in / 
# Wed, 05 Oct 2022 10:52:26 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 19:58:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 19:58:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 19:58:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 20:04:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 20:04:01 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 20:05:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 20:05:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 01:52:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 01:52:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 01:52:07 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 01:52:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 01:52:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 01:52:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 02:14:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 06 Oct 2022 02:14:58 GMT
ENV TOMCAT_MAJOR=8
# Thu, 06 Oct 2022 02:14:58 GMT
ENV TOMCAT_VERSION=8.5.82
# Thu, 06 Oct 2022 02:14:59 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Thu, 06 Oct 2022 02:15:00 GMT
COPY dir:dd0bedf0f1f30b3fa8d9320fa66fb6a8e07d3be6e5bcb1d9103a5cf95e73b4d4 in /usr/local/tomcat 
# Thu, 06 Oct 2022 02:15:10 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 02:15:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 06 Oct 2022 02:15:13 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 02:15:14 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5053ecffedc109608feacf4836ad15e0f7b2f6a411250a41574342de479c4760`  
		Last Modified: Wed, 05 Oct 2022 10:54:49 GMT  
		Size: 35.7 MB (35709341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec5805d4537b892bc58f304ab88bf426910b3553a64a310062ff835310bbe1d`  
		Last Modified: Wed, 05 Oct 2022 20:14:40 GMT  
		Size: 18.3 MB (18267799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8234db927a11aad0b445ee658a29f6a0ed42436159ffea73a0ca5e16328552fb`  
		Last Modified: Wed, 05 Oct 2022 20:15:54 GMT  
		Size: 46.6 MB (46620361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89ec71430e631e456faad0970fa76dad3624d03fa36d26c3e0ea8880252b445`  
		Last Modified: Wed, 05 Oct 2022 20:15:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96847528fe23f5ade7b0e62a1b48ac8fe98e8846269dd0c37963428c451a95f`  
		Last Modified: Thu, 06 Oct 2022 02:33:27 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731eb9c3e92696cd7146a746163da3a9f16308ac51ef02a29014e17ff350038f`  
		Last Modified: Thu, 06 Oct 2022 02:47:06 GMT  
		Size: 11.2 MB (11229985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ec4d9ed1499957665dfd239a0ab78544a9222517b9304f5e025996b0a5d830`  
		Last Modified: Thu, 06 Oct 2022 02:47:04 GMT  
		Size: 486.6 KB (486577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddbafef604ab68938860b98ab61d983ace819074628a921bbf0b74b9a2975d`  
		Last Modified: Thu, 06 Oct 2022 02:47:04 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:f9f4624c067feaefaa762f060dea83b04d475c6f4890b8c7d4e719905f4ec0f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.8 MB (100775347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a999e7f68370ce47ec23373edc4f038dbd78d8d4e3550ddb48c7aec3a67a8c7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:57 GMT
ADD file:b1fcc8690fce8195995c8eab6b853225d65017d69692537273760bf84bfb72ec in / 
# Tue, 04 Oct 2022 23:52:59 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:55:38 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 07:55:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 07:55:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 07:57:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:57:57 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 07:59:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2e4137529319cd7935f74e1289025b7b4c794c0fb47a3d138adffbd1bbc0ea58';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b63f532cb8b30e4d0bd18d52f08c1933e3cf66aeb373180d002274b6d94b4a25';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='02947997297742ac5a7064fc5414042071fb96d0260d3756100abb281eff3cde';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f594458bbf42d1d43f7fb5880d0b09d5f9ac11e8eea0de8756419228a823d21c';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e96814ee145a599397d91e16831d2dddc3c6b8e8517a8527e28e727649aaa2d1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jre_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 07:59:19 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 18:06:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Oct 2022 18:06:55 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 18:06:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Oct 2022 18:06:55 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Oct 2022 18:06:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Oct 2022 18:06:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Oct 2022 18:14:40 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 05 Oct 2022 18:14:40 GMT
ENV TOMCAT_MAJOR=8
# Tue, 11 Oct 2022 20:28:16 GMT
ENV TOMCAT_VERSION=8.5.83
# Tue, 11 Oct 2022 20:28:16 GMT
ENV TOMCAT_SHA512=57cbe9608a9c4e88135e5f5480812e8d57690d5f3f6c43a7c05fe647bddb7c3b684bf0fc0efebad399d05e80c6d20c43d5ecdf38ec58f123e6653e443f9054e3
# Tue, 11 Oct 2022 20:28:16 GMT
COPY dir:9b05c08e51ab3dc9f3dddf4b3ff25af78a1f181e9e510ebf966c6803f476e229 in /usr/local/tomcat 
# Tue, 11 Oct 2022 20:28:19 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 11 Oct 2022 20:28:20 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 11 Oct 2022 20:28:20 GMT
EXPOSE 8080
# Tue, 11 Oct 2022 20:28:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:29c30188ad5f0c76a8b336bfa488a1bdf199dc8127ed81e4051c1c71d4da8f87`  
		Last Modified: Tue, 04 Oct 2022 23:54:34 GMT  
		Size: 28.6 MB (28643466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52739390b60a09956a7447b4a5e03687f23ee651c092732ffdc1b69a0764dd8`  
		Last Modified: Wed, 05 Oct 2022 08:04:28 GMT  
		Size: 16.8 MB (16766125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9991fc19bb3c35655b342ac496229e68c7d56ad3790ea0e51d556505d1c7c`  
		Last Modified: Wed, 05 Oct 2022 08:05:07 GMT  
		Size: 43.7 MB (43693934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b96185e649756765f3b8af58d879adc6ccc38533cea5cb868b47a00ff8b2eea`  
		Last Modified: Wed, 05 Oct 2022 08:05:01 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69345bc0c9e822f306533a3d4030409a94caa0005dcae359f6b8c94d27d4272d`  
		Last Modified: Wed, 05 Oct 2022 18:23:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c39b8325dc0c79af12fcbe3b6e1833c3941546de8625f31617a27f9544fb1f`  
		Last Modified: Tue, 11 Oct 2022 20:39:36 GMT  
		Size: 11.2 MB (11214403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d7e3f9217930e0d606d3238547cba6792e33a7b9ecaf74bf86d4b4803d2c57`  
		Last Modified: Tue, 11 Oct 2022 20:39:35 GMT  
		Size: 457.0 KB (456958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4b493cde1287df5bc3e81e83c19f38d80678fafa5ec1769eee79416daa7d83`  
		Last Modified: Tue, 11 Oct 2022 20:39:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
