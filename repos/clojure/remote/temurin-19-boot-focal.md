## `clojure:temurin-19-boot-focal`

```console
$ docker pull clojure@sha256:9119ec1d34fdb96513d9c84b84fb7c16c5e4fca2f5250b74678956dcd879e002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-focal` - linux; amd64

```console
$ docker pull clojure@sha256:66eebeccaf0f8d48096bdc8c1e5c49572851d2f234d670762c72c88128a221ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308939601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d970e619af25c60aaaf63809e5bd42a325f2777a890be586ce3323fdd9cecac5`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:10 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:45:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:46:43 GMT
ENV JAVA_VERSION=jdk-19.0.1+10
# Fri, 09 Dec 2022 01:47:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5e8d7b3189364afd78d936bad140dbe1e7025d4b96d530ed5536d035c21afb7c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='5f404ae08d7c49f22fe04c04ec39d7e7b17cae2007b9513ad1a7a1164174898b';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_arm_linux_hotspot_19.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79320712bbef13825a0aa308621006f32e54f503142737fb21ff085185a61a96';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0b4168e5a98d89b0a24fb2357b3544980d8c88a639024cde18b119b27d7583ae';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='163da7ea140210bae97c6a4590c757858ab4520a78af0e3e33129863d4087552';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_x64_linux_hotspot_19.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 01:47:06 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 01:47:06 GMT
CMD ["jshell"]
# Fri, 09 Dec 2022 06:46:17 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 06:46:17 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 06:46:17 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 06:46:22 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 06:46:22 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 06:46:23 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 06:46:43 GMT
RUN boot
# Fri, 09 Dec 2022 06:46:43 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 06:46:43 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 06:46:43 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b0873b98ac8f32b151346adbb3bebb71422b7f4d491cef4fe8fa08d19bf076`  
		Last Modified: Fri, 09 Dec 2022 01:52:23 GMT  
		Size: 20.1 MB (20086897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c466cc2c6833f53eb7e931ca25fc817ca2bd8baca6cc8e8a0037b9bcfb4c36e`  
		Last Modified: Fri, 09 Dec 2022 01:54:04 GMT  
		Size: 201.1 MB (201114405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d508d2b7eae1c1041383906f4ee9f4774b91fa6f731e31a7e18bc9a3e9b7b08a`  
		Last Modified: Fri, 09 Dec 2022 01:53:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8566437b033ab65499e0aad811db98b6338c11c56edae0bc37e419d7d32f8c`  
		Last Modified: Fri, 09 Dec 2022 07:00:28 GMT  
		Size: 340.3 KB (340291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678ecfe48dd8dbeb832967823d540cc3e04832dbc0bcf03ec8a7cd70527455ff`  
		Last Modified: Fri, 09 Dec 2022 07:00:30 GMT  
		Size: 58.8 MB (58820551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f496e9f97b592b29a626a79f7ab1cd2923ce066277c84b17b946139e698d002`  
		Last Modified: Fri, 09 Dec 2022 07:00:27 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:62175323c0365efdcf05628f81b61bf402e44896b5fdf87825b1cbc2646e4113
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (307017511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d27f0d8997b20194e56959926a177abdf657eff21bbc6fed1ba49bb9743540`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:38:47 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:38:47 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:38:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:41:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:42:37 GMT
ENV JAVA_VERSION=jdk-19.0.1+10
# Fri, 09 Dec 2022 03:42:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5e8d7b3189364afd78d936bad140dbe1e7025d4b96d530ed5536d035c21afb7c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='5f404ae08d7c49f22fe04c04ec39d7e7b17cae2007b9513ad1a7a1164174898b';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_arm_linux_hotspot_19.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='79320712bbef13825a0aa308621006f32e54f503142737fb21ff085185a61a96';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0b4168e5a98d89b0a24fb2357b3544980d8c88a639024cde18b119b27d7583ae';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='163da7ea140210bae97c6a4590c757858ab4520a78af0e3e33129863d4087552';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.1%2B10/OpenJDK19U-jdk_x64_linux_hotspot_19.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:42:56 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 03:42:56 GMT
CMD ["jshell"]
# Fri, 09 Dec 2022 05:11:51 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 09 Dec 2022 05:11:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 09 Dec 2022 05:11:51 GMT
WORKDIR /tmp
# Fri, 09 Dec 2022 05:11:54 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Fri, 09 Dec 2022 05:11:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 09 Dec 2022 05:11:54 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 09 Dec 2022 05:12:12 GMT
RUN boot
# Fri, 09 Dec 2022 05:12:12 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Fri, 09 Dec 2022 05:12:12 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 09 Dec 2022 05:12:12 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e6255f1d9634acbb611b17bafa5b0ec522018281353d85d93ff022b2cb8d08`  
		Last Modified: Fri, 09 Dec 2022 03:47:43 GMT  
		Size: 20.8 MB (20800924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8256e2f01bdcbb5424d066fed7e8efb6bec4e78db26bc1ad440f35b5daf8314`  
		Last Modified: Fri, 09 Dec 2022 03:49:10 GMT  
		Size: 199.9 MB (199862457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7aded17e52e983602a97a3373ae635e0383ff613796ce739f76130382f6d48`  
		Last Modified: Fri, 09 Dec 2022 03:48:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d50fe68e53d2c9cac1e0544f2bf32a33539c8aa707131543043418c8960242`  
		Last Modified: Fri, 09 Dec 2022 05:24:39 GMT  
		Size: 340.1 KB (340105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e2b7166c88c39db697d3cb88366ca1cdce3118807023ccda87ac537ed7c9e`  
		Last Modified: Fri, 09 Dec 2022 05:24:42 GMT  
		Size: 58.8 MB (58820282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00e9302f5ac4a814d79ec85d473cc1b24ecb0cfda880f3a07f00cf9b43f6c28`  
		Last Modified: Fri, 09 Dec 2022 05:24:39 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
