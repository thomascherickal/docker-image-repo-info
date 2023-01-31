## `clojure:temurin-19-boot-focal`

```console
$ docker pull clojure@sha256:5e5efc8a29a0d05c188e1bb0a0ac100d83cd5bea2dc3a59cef516df2ff1fd089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-focal` - linux; amd64

```console
$ docker pull clojure@sha256:e1159cc8eb472d62ea5a84e7933b3e7a6bb1c14d7e92a0877445725145f08db3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308942653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c54eb7d42eb66d709dba1a513fb4630851f26b87d74869cc9818258665f27eda`
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
# Wed, 25 Jan 2023 19:22:14 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 25 Jan 2023 19:22:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c4be9aa173cb0deb0d215643d9509c8900e5497290b29eee4bee335fa57984f';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='6a51cb3868b5a3b81848a0d276267230ff3f8639f20ba9ae9ef1d386440bf1fd';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_arm_linux_hotspot_19.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='173d1256dfb9d13d309b5390e6bdf72d143b512201b0868f9d349d5ed3d64072';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f2512f9a8e9847dd5d3557c39b485a8e7a1ef37b601dcbcb748d22e49f44815c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3a3ba7a3f8c3a5999e2c91ea1dca843435a0d1c43737bd2f6822b2f02fc52165';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_linux_hotspot_19.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 25 Jan 2023 19:22:35 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 25 Jan 2023 19:22:35 GMT
CMD ["jshell"]
# Wed, 25 Jan 2023 19:56:46 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 25 Jan 2023 19:56:46 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 25 Jan 2023 19:56:46 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 19:56:52 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 19:56:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 25 Jan 2023 19:56:52 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 25 Jan 2023 19:57:10 GMT
RUN boot
# Wed, 25 Jan 2023 19:57:11 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 19:57:11 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 19:57:11 GMT
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
	-	`sha256:462c3448f7dfaba11276b88575088e00672ba935a35000bce5739b42c052fed6`  
		Last Modified: Wed, 25 Jan 2023 19:29:25 GMT  
		Size: 201.1 MB (201117683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195cfff8e4e563530e325239c9c36a0bc5df36d4f4e9b3a32f82fa3fab64e000`  
		Last Modified: Wed, 25 Jan 2023 19:29:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ab454785da89ffe023da117a843630f7b16416f5c1af0cec725a6e5d450f7`  
		Last Modified: Wed, 25 Jan 2023 20:08:49 GMT  
		Size: 340.3 KB (340312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926268f71bcc0cd947e32fc5f5437d3ab62dd417db0f21d5b103aa4b3bbbdbd3`  
		Last Modified: Wed, 25 Jan 2023 20:08:52 GMT  
		Size: 58.8 MB (58820302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141721f473a0743ac1a63935678c231ab975cc56d2cccb37f711b9f866dfdfa4`  
		Last Modified: Wed, 25 Jan 2023 20:08:49 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:774223bb6f333c6aeed6147d2a2f5ad1fc9fda57154f01ebc5dcc127daa0b3c3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (307024097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d150776387c8fd8a294cb70924673453592753d10fc093c3597fadb8c0c1fa`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Thu, 26 Jan 2023 13:50:26 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:50:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:50:33 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Thu, 26 Jan 2023 13:50:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:43:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:43:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:43:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 17:46:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:47:38 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Tue, 31 Jan 2023 17:47:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c4be9aa173cb0deb0d215643d9509c8900e5497290b29eee4bee335fa57984f';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='6a51cb3868b5a3b81848a0d276267230ff3f8639f20ba9ae9ef1d386440bf1fd';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_arm_linux_hotspot_19.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='173d1256dfb9d13d309b5390e6bdf72d143b512201b0868f9d349d5ed3d64072';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f2512f9a8e9847dd5d3557c39b485a8e7a1ef37b601dcbcb748d22e49f44815c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3a3ba7a3f8c3a5999e2c91ea1dca843435a0d1c43737bd2f6822b2f02fc52165';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_linux_hotspot_19.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 17:47:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 17:47:55 GMT
CMD ["jshell"]
# Tue, 31 Jan 2023 20:57:59 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 31 Jan 2023 20:57:59 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 31 Jan 2023 20:57:59 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:58:03 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Tue, 31 Jan 2023 20:58:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 31 Jan 2023 20:58:03 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 31 Jan 2023 20:58:19 GMT
RUN boot
# Tue, 31 Jan 2023 20:58:19 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Tue, 31 Jan 2023 20:58:19 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 31 Jan 2023 20:58:20 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0d033864bdd7e6f8ce77794561b894a3182f3ad98291a8fbb57cfa287b05fc`  
		Last Modified: Tue, 31 Jan 2023 17:52:30 GMT  
		Size: 20.8 MB (20801392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3607e5b5a89a0fd061eba535fce08fc33730246f597beced59d1031f8919d337`  
		Last Modified: Tue, 31 Jan 2023 17:53:58 GMT  
		Size: 199.9 MB (199868031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e793bbb7723895ce4b9aebd5f0ef415cdb26069846abecb768296d67291b8b9d`  
		Last Modified: Tue, 31 Jan 2023 17:53:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707a478363ace175275d441229dd253d8a209b251a3257e9a4923161e5c3a039`  
		Last Modified: Tue, 31 Jan 2023 21:10:40 GMT  
		Size: 340.0 KB (340034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9e0d6301b68b567fca220b37fc93632b33f8d73b0f371c809c1d686a88e2c`  
		Last Modified: Tue, 31 Jan 2023 21:10:43 GMT  
		Size: 58.8 MB (58820329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a80144158b0dafe1e2151883deb51fe40736f707eb19db299457986da4db088`  
		Last Modified: Tue, 31 Jan 2023 21:10:40 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
