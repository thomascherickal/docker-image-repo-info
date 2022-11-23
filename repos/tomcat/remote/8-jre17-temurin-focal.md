## `tomcat:8-jre17-temurin-focal`

```console
$ docker pull tomcat@sha256:f62537171841d2a436b00f50610b74e4220b35c5ceca035f2776dcefda7a7091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:594428a71154bf43a3a19585780439110553daf24941654bb8b556c148caf077
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107376051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2edd0e2173f700eba1616db2f3fbc2b57df78808c7db1d7048ac570e5fc4889a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 17:27:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 17:27:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 17:27:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 17:29:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:20:54 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:22:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:22:01 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:48:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:48:31 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:48:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:48:32 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:48:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:48:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:52:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 07 Nov 2022 21:52:57 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Nov 2022 22:49:19 GMT
ENV TOMCAT_VERSION=8.5.84
# Tue, 22 Nov 2022 22:49:19 GMT
ENV TOMCAT_SHA512=e595e906d62ff16545318108478aa101103181569dc6f4549dd0cdf8744147f7e9ba8a88cab6d33237b22981acb1085de86e7b2a4f1659efdbd4804df1303561
# Tue, 22 Nov 2022 22:49:19 GMT
COPY dir:3683e2a93339a54d4e441924643fd8d09daaf0eb5f9c9df5d85cc191c190ab6a in /usr/local/tomcat 
# Tue, 22 Nov 2022 22:49:24 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Nov 2022 22:49:25 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Nov 2022 22:49:25 GMT
EXPOSE 8080
# Tue, 22 Nov 2022 22:49:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5503608cd3ee42cbf7643a392e00ac707a3fd9a24b4cbe9dc6ee9ee6f92397f`  
		Last Modified: Wed, 26 Oct 2022 16:45:46 GMT  
		Size: 20.1 MB (20104549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e94dc7d947dd2b67ffb463efd050d22e845553634cf46e2243ceecffc1fd6a3`  
		Last Modified: Mon, 07 Nov 2022 20:26:41 GMT  
		Size: 47.0 MB (46956297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68588881139f73fdeee52c342a901b014d25e0866784938168bc64769ed9ec6e`  
		Last Modified: Mon, 07 Nov 2022 20:26:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50e50e8f1ce0ae38585a2bde3626f30783ca7e63b49925d733d5bdafbf3abf4`  
		Last Modified: Mon, 07 Nov 2022 22:00:04 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d8fe4d74fa627c9f914529b580dd6ad6396bc178455ead7438ebc7184e60c0`  
		Last Modified: Tue, 22 Nov 2022 23:01:58 GMT  
		Size: 11.3 MB (11285300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940ecb37221e8c9bcd325a98fa69e72826e837cc040a23cef396837557e9d77d`  
		Last Modified: Tue, 22 Nov 2022 23:01:57 GMT  
		Size: 451.6 KB (451608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d2c732fac74bf49ec0994b90293361ed96e014c858d2f603ab72238b301465`  
		Last Modified: Tue, 22 Nov 2022 23:01:56 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:8bf19a5f8f39f253961728690d3404c6d84343ed821f45bac3f7f5cb662e7409
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.2 MB (100237884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497b14cdf7d1d37f0c0f8c809e65296994e55fbadf97b39940b0b8fb332b1e53`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 03:07:00 GMT
ADD file:0e30b9fd980776c745b113ac234367069202f461c4d888acb3225ccc0aa75385 in / 
# Tue, 25 Oct 2022 03:07:02 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:34:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:34:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:34:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:38:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 19:58:33 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 19:59:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 19:59:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 20:47:09 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 20:47:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 20:47:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 20:47:10 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 20:47:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 20:47:10 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 20:53:22 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 07 Nov 2022 20:53:22 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Nov 2022 23:18:21 GMT
ENV TOMCAT_VERSION=8.5.84
# Tue, 22 Nov 2022 23:18:21 GMT
ENV TOMCAT_SHA512=e595e906d62ff16545318108478aa101103181569dc6f4549dd0cdf8744147f7e9ba8a88cab6d33237b22981acb1085de86e7b2a4f1659efdbd4804df1303561
# Tue, 22 Nov 2022 23:18:22 GMT
COPY dir:80578995f7f85b05ffe3821541c1758778ac4a9b6f3bdf3c59ecb6d40c6f8cd9 in /usr/local/tomcat 
# Tue, 22 Nov 2022 23:18:26 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Nov 2022 23:18:27 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Nov 2022 23:18:28 GMT
EXPOSE 8080
# Tue, 22 Nov 2022 23:18:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:88411d40226eb74e038e5d2cbedefbd7555c34298ed687d1073cf87740fab694`  
		Last Modified: Tue, 25 Oct 2022 03:09:28 GMT  
		Size: 24.6 MB (24588786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18de77b8e763c9de4a384b71099f699ea2d44f453526c13400cbb79e9e4dd9fe`  
		Last Modified: Wed, 02 Nov 2022 18:47:59 GMT  
		Size: 19.5 MB (19484984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e469b6991fa498ca41f27347b7cbc2553e0339f8902cb0dba885a5996ce85f9e`  
		Last Modified: Mon, 07 Nov 2022 20:04:25 GMT  
		Size: 44.5 MB (44500841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac22d422fde00842232b34944efa8d43a11dc37abdedc7bdcb962c2caec6ea5`  
		Last Modified: Mon, 07 Nov 2022 20:04:17 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd3e3417c41d3857c62a77111a00f13207917f8351fe226400094f40927585c`  
		Last Modified: Mon, 07 Nov 2022 21:08:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1677ff3626b77ad52eca1d915f9477a6fb9c0b9397ea1c715ff7ae262959a3e6`  
		Last Modified: Tue, 22 Nov 2022 23:37:09 GMT  
		Size: 11.2 MB (11234693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c865a00331f11245938e9f5ce3a10b57911254bf87acb9b5ed15f06f8cdb58db`  
		Last Modified: Tue, 22 Nov 2022 23:37:08 GMT  
		Size: 428.1 KB (428150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b23c28c9a0dd5170093171e0e2e082b9c722b2cadf79aee3a5a62983f592e73`  
		Last Modified: Tue, 22 Nov 2022 23:37:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:fd0c5275187eb8106ac4579fa8ecdc5677775ee024ad99194f79753de9902f35
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.2 MB (106178044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52dbbb86c89c97f00847a0cf6927f097472b7a5068fe13857ee51ae49443f11a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:07:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:07:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:07:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:11:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:40:01 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:41:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:41:08 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:55:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:55:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:55:07 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:55:07 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:55:07 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:55:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:58:39 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 07 Nov 2022 21:58:39 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Nov 2022 23:03:51 GMT
ENV TOMCAT_VERSION=8.5.84
# Tue, 22 Nov 2022 23:03:52 GMT
ENV TOMCAT_SHA512=e595e906d62ff16545318108478aa101103181569dc6f4549dd0cdf8744147f7e9ba8a88cab6d33237b22981acb1085de86e7b2a4f1659efdbd4804df1303561
# Tue, 22 Nov 2022 23:03:52 GMT
COPY dir:60fc7e26cba5063e49a4e9d3d4817ae9a1dd602d195c5c957a316f0d68fdc557 in /usr/local/tomcat 
# Tue, 22 Nov 2022 23:03:56 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Nov 2022 23:03:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Nov 2022 23:03:58 GMT
EXPOSE 8080
# Tue, 22 Nov 2022 23:03:58 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b12f4cab5d71e49b20ff7f15fb01ffd2673806701a44a0e8d79d667d7c2ca4`  
		Last Modified: Wed, 26 Oct 2022 01:19:55 GMT  
		Size: 20.8 MB (20828559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640e1d5c7cb2fd15e07c8dbd80f0ba4a78e376a80ac1f4a93677c27c7f6a506d`  
		Last Modified: Mon, 07 Nov 2022 20:44:34 GMT  
		Size: 46.4 MB (46398682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e091c75a4fc06be4165bcfc4c2bbf210136b75b01a81c96e03a3f72ee33af1`  
		Last Modified: Mon, 07 Nov 2022 20:44:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba4779fb60820cadb73dca7659eaf019e66b4cf3bf157659c8c5df9fbe30007`  
		Last Modified: Mon, 07 Nov 2022 22:06:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106a5ea457b9e4c3eeaa328b61d9799b5d0b05a3666e7dbb1f55a2c46a037542`  
		Last Modified: Tue, 22 Nov 2022 23:15:49 GMT  
		Size: 11.3 MB (11302258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2484d3efac4d3c06254479131541bab2b8b538eddbbc832914128e4ec6a4f3ce`  
		Last Modified: Tue, 22 Nov 2022 23:15:48 GMT  
		Size: 452.1 KB (452083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a537a6953a2c7004b056bfa39a700575fedf0b8991256cdc0fbf4c503652bfd8`  
		Last Modified: Tue, 22 Nov 2022 23:15:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:9179ce2fac26b922c1ab8a0d9bdc38408b43d4278f276463e7527e690cb26ac5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113989899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb0ea96075fb31a3f10c32afbad092b9571fe389c4bd7e85176a5ed330648f77`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:47 GMT
ADD file:013ddcea49540903962069a03762fe471452e8cf00bafeb530724940405797e1 in / 
# Tue, 25 Oct 2022 03:25:49 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 13:45:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 13:45:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 13:45:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 13:51:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:17:36 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:19:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:19:42 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:09:44 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:09:44 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:09:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:09:46 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:09:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:09:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:17:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 07 Nov 2022 21:17:43 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Nov 2022 22:55:26 GMT
ENV TOMCAT_VERSION=8.5.84
# Tue, 22 Nov 2022 22:55:26 GMT
ENV TOMCAT_SHA512=e595e906d62ff16545318108478aa101103181569dc6f4549dd0cdf8744147f7e9ba8a88cab6d33237b22981acb1085de86e7b2a4f1659efdbd4804df1303561
# Tue, 22 Nov 2022 22:55:28 GMT
COPY dir:2edaee0051e813369dd445c825f6de8c1658b639fca70fe787b64d6f89573f8b in /usr/local/tomcat 
# Tue, 22 Nov 2022 22:55:36 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Nov 2022 22:55:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Nov 2022 22:55:40 GMT
EXPOSE 8080
# Tue, 22 Nov 2022 22:55:40 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:42e5f4d60d38e5070be91d6965be1cff1294e6dc275038002dc2ef1812233b0e`  
		Last Modified: Tue, 25 Oct 2022 03:27:44 GMT  
		Size: 33.3 MB (33300542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a64ad4bc2ecdf82e0999c7ea9f16fd927cf85d64f83821bf651ceec25f8908`  
		Last Modified: Tue, 25 Oct 2022 14:02:22 GMT  
		Size: 22.1 MB (22079033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d2e849faed71b798fa2378973f762c884d77709b716ae3a3dbf2769540667`  
		Last Modified: Mon, 07 Nov 2022 20:26:03 GMT  
		Size: 46.8 MB (46807807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ba05eedcaebfc5e07614b51e9937183ea3990e540753cb89f21fe09e9f856d`  
		Last Modified: Mon, 07 Nov 2022 20:25:51 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0530a17f69ea69b9c47a161c4d2128d788eea6d7f616acf6c796ced80d1bff71`  
		Last Modified: Mon, 07 Nov 2022 21:30:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667da6a75ae775524b9450b3b9af63b56458360c4b96885a7162a015eb9c6c13`  
		Last Modified: Tue, 22 Nov 2022 23:14:54 GMT  
		Size: 11.3 MB (11325227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98caf35992f5ae246ddebf9c44d8e8030bf1ba025f92172acfa87e73fe5a540b`  
		Last Modified: Tue, 22 Nov 2022 23:14:52 GMT  
		Size: 476.8 KB (476826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a650d04abd6c265e8950582cedde555f6f7c46b07711701446877264041180`  
		Last Modified: Tue, 22 Nov 2022 23:14:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:b042906ed362a4881152dfe68dd64c80fedd5b102a1606a75af5c719e5e607e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102051448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1155544f5c35fbe7dcd9766a8f125d168e8ae29699a2fe132279583a1f17fcd`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:11 GMT
ADD file:c657b467ecb15f1f4a49a5f04a525f38924750c8187c9ef9f0b886d0264e21f1 in / 
# Tue, 25 Oct 2022 01:23:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:58:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 25 Oct 2022 08:58:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 08:58:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 25 Oct 2022 09:03:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Nov 2022 20:42:23 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:44:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='34d6414710db27cd7760fe369135f3b9927ccc81410280606613166d4106d60a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='9e0d1745139fe502f22df1e261d2ed1ad807085dd75a8b333d481289b579870d';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='51dd491505bd2e096676b9dc8ecaf196d78993215af16c0f9dfddfe3dbc0205b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='eeb1e92b8267e7e015908f3e3b80e48f418b37a2b4491f65290bc5d25e5daf93';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='11326464a14b63e6328d1d2088a23fb559c0e36b3f380e4c1f8dcbe160a8b95e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jre_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 07 Nov 2022 20:44:56 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 21:36:08 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Nov 2022 21:36:08 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Nov 2022 21:36:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Nov 2022 21:36:11 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Nov 2022 21:36:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:36:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Nov 2022 21:45:51 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 07 Nov 2022 21:45:52 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Nov 2022 23:16:31 GMT
ENV TOMCAT_VERSION=8.5.84
# Tue, 22 Nov 2022 23:16:32 GMT
ENV TOMCAT_SHA512=e595e906d62ff16545318108478aa101103181569dc6f4549dd0cdf8744147f7e9ba8a88cab6d33237b22981acb1085de86e7b2a4f1659efdbd4804df1303561
# Tue, 22 Nov 2022 23:16:32 GMT
COPY dir:594ecce2d3d2481ea542c2507e96bf6008117c65a797a5fe04ae9fc322d67322 in /usr/local/tomcat 
# Tue, 22 Nov 2022 23:16:35 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 22 Nov 2022 23:16:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Nov 2022 23:16:37 GMT
EXPOSE 8080
# Tue, 22 Nov 2022 23:16:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a63328f08dbd14148b5ffe154c18846ead48e759779d007b78ec3fb19f5f43a5`  
		Last Modified: Tue, 25 Oct 2022 01:24:36 GMT  
		Size: 27.0 MB (27016028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9e8310c059ea81f37516c947b6ad2e266b5df4f83665270795602ff3e8d9f9`  
		Last Modified: Tue, 25 Oct 2022 09:12:03 GMT  
		Size: 19.5 MB (19546934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fc11cd6504e22032b3af54d0c0a12c9c0411cd2908af1cc4918584498e64cf`  
		Last Modified: Mon, 07 Nov 2022 20:49:11 GMT  
		Size: 43.7 MB (43737364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a82a57749d8ce09eccde22d98d89efaf16b52313fc744ebdfb09a3fc6965ff0`  
		Last Modified: Mon, 07 Nov 2022 20:49:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb9fab5726e83cb4f89418a789c88e3532b1f476c855945a3c4b9fd08c506ec`  
		Last Modified: Mon, 07 Nov 2022 21:56:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f5eab5ce7f80366fa8030aa6d9dceb80b54eb799408b477116354c3a67f61c`  
		Last Modified: Tue, 22 Nov 2022 23:26:38 GMT  
		Size: 11.3 MB (11297245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d86b523d87fd90246bf5cd573991ae66a60974d6b1ae6188276862b29f07bb2`  
		Last Modified: Tue, 22 Nov 2022 23:26:37 GMT  
		Size: 453.4 KB (453416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ac62a5fdf0e642835204cb4aecfba44c2c9de457f34a1af817c552043a884d`  
		Last Modified: Tue, 22 Nov 2022 23:26:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
