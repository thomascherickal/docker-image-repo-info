## `clojure:temurin-19-tools-deps-1.11.1.1208-focal`

```console
$ docker pull clojure@sha256:b16dc0e543154e1033435c2593788f28b4a17db5a73223981d55c02b9b514300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-tools-deps-1.11.1.1208-focal` - linux; amd64

```console
$ docker pull clojure@sha256:2d85d440235fa18f952d05bb77b5c7fe925a34f84c942712972dd4b17a3fd94f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.8 MB (312786411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed180c0bab603965c1ba2ebb41646ff9d798ef0d84ba0639053643d40a47db09`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

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
# Wed, 25 Jan 2023 20:00:18 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 25 Jan 2023 20:00:19 GMT
WORKDIR /tmp
# Wed, 25 Jan 2023 20:00:33 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 25 Jan 2023 20:00:34 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 25 Jan 2023 20:00:34 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 25 Jan 2023 20:00:34 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 25 Jan 2023 20:00:34 GMT
CMD ["-M" "--repl"]
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
	-	`sha256:42f888d557d38fe2bdfcce4eb7f2bb4a568c06a3fe2eec3685284af0fc3345cd`  
		Last Modified: Wed, 25 Jan 2023 20:11:04 GMT  
		Size: 63.0 MB (63003756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c214b8eee086d797d476d37804b40846f95ae91e45dc9f7b8cc5176d28a4e69`  
		Last Modified: Wed, 25 Jan 2023 20:10:56 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82e970db7b805ecfc18a3ca16831f6b65b96bb75aced28b83630a98292646e8`  
		Last Modified: Wed, 25 Jan 2023 20:10:56 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-tools-deps-1.11.1.1208-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:321fd6d2940e72d995de9d13b993d4c4bc5b469e9c6e42c1d73e33e4291b6da3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.0 MB (310994703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9459ca02d4e87b12ef624f2435976a23595a8720835cbd5b5d6fd9bd164088`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

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
# Tue, 31 Jan 2023 20:59:30 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Tue, 31 Jan 2023 20:59:30 GMT
WORKDIR /tmp
# Tue, 31 Jan 2023 20:59:41 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Tue, 31 Jan 2023 20:59:42 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 31 Jan 2023 20:59:42 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 31 Jan 2023 20:59:42 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 31 Jan 2023 20:59:42 GMT
CMD ["-M" "--repl"]
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
	-	`sha256:f9da9c4c2d958e791dbcb6fe60cdbf07089cf79f7912878d31a6184ffe1eee59`  
		Last Modified: Tue, 31 Jan 2023 21:11:40 GMT  
		Size: 63.1 MB (63130353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6842487b55b4848c7083ec85acc4b37e66568acfecc9b101385b693e722f55e6`  
		Last Modified: Tue, 31 Jan 2023 21:11:34 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4161d47e8a77635c11f1cb77278d49f1d553ebc7300064903bed00471d61edc`  
		Last Modified: Tue, 31 Jan 2023 21:11:34 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
