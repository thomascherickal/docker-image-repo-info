## `clojure:tools-deps-1.11.1.1208`

```console
$ docker pull clojure@sha256:c15648f2a2fda2d26bfd7035adea957c2a32b59a992b7bfad50268b10dc530bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:tools-deps-1.11.1.1208` - linux; amd64

```console
$ docker pull clojure@sha256:bd90fefb51fcfafe288c3ba25297cbcab5cdee2c86000290653398374db9eb75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.3 MB (294270846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:323d3e46d6c76e1c77b6bce6725a1b994300bda7d5fa2c17d1ed8d2d02909988`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:45:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:45:54 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 01:46:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c26c0e09f1641a666d6740d802beb81e12180abaea07b47c409d30c7f368109';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='e7c81596f67b6325036e9182d012f2266ced5663c5d4b0de0540ce62dcc67718';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a426a4e2cbc29f46fa686bea8b26613f7b7a9a772a77fed0d40dfe05295be883';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6fc21601d3cf08584e698d676249a91b6a9e790c8fc7c4d9f294628562e16273';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='482180725ceca472e12a8e6d1a4af23d608d78287a77d963335e2a0156a020af';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 01:46:05 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 01:46:05 GMT
CMD ["jshell"]
# Wed, 14 Dec 2022 00:23:44 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:23:44 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:23:58 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 14 Dec 2022 00:23:59 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:23:59 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 14 Dec 2022 00:23:59 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 14 Dec 2022 00:23:59 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8d923227d8dc300e1ddab1b65c83c0eff7f4a7105d958420872f7138b79735`  
		Last Modified: Fri, 09 Dec 2022 01:52:47 GMT  
		Size: 17.0 MB (16973851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda8241fd25fe52c584da502f21cef5b5067551f7bcfcca58e9a630238f7f558`  
		Last Modified: Fri, 09 Dec 2022 01:52:59 GMT  
		Size: 192.4 MB (192440274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dccabde73de58115ed8db691bd335b82d91b6961c0d1af77691b368b0a8253`  
		Last Modified: Fri, 09 Dec 2022 01:52:45 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f82a6e8fda3d6035c7aa73a4503f5cc37db39af4523594cd2b4643a987eb3fc`  
		Last Modified: Wed, 14 Dec 2022 00:31:08 GMT  
		Size: 54.4 MB (54426821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70d92799882284c5e81ab27a7e2274df1b491e2c1383139ba12d96e9207b8f`  
		Last Modified: Wed, 14 Dec 2022 00:31:02 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb89ff34b21007602b9a5ea3987fbacfa2bd39cb30bf70a1d04e92bae926df3`  
		Last Modified: Wed, 14 Dec 2022 00:31:02 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:tools-deps-1.11.1.1208` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:4f2dcdde2b4b32ba3b6e1fe949d1d9a161316b767b71c603854e5e868debf8e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.4 MB (292400764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0bc73bd573e1aa4ba4e6b921671a1544261a2c5765301fa172d194ba26bdf7d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:39:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:39:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:39:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:42:00 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:42:00 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Fri, 09 Dec 2022 03:42:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c26c0e09f1641a666d6740d802beb81e12180abaea07b47c409d30c7f368109';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.5_8.tar.gz';          ;;        armhf|arm)          ESUM='e7c81596f67b6325036e9182d012f2266ced5663c5d4b0de0540ce62dcc67718';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.5_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a426a4e2cbc29f46fa686bea8b26613f7b7a9a772a77fed0d40dfe05295be883';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.5_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6fc21601d3cf08584e698d676249a91b6a9e790c8fc7c4d9f294628562e16273';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.5_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='482180725ceca472e12a8e6d1a4af23d608d78287a77d963335e2a0156a020af';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.5%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.5_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:42:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 03:42:10 GMT
CMD ["jshell"]
# Wed, 14 Dec 2022 00:42:31 GMT
ENV CLOJURE_VERSION=1.11.1.1208
# Wed, 14 Dec 2022 00:42:31 GMT
WORKDIR /tmp
# Wed, 14 Dec 2022 00:42:42 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "4a3b1200c4d633202648dc3db6ed0a1311e75cc4baeee8fce32208c1eaa07537 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 14 Dec 2022 00:42:43 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 14 Dec 2022 00:42:43 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 14 Dec 2022 00:42:43 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 14 Dec 2022 00:42:43 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f2e5e37e706412c1481b71d2240df4fe659ef83ae4d2932a8ddfe42b0d3d20`  
		Last Modified: Fri, 09 Dec 2022 03:48:04 GMT  
		Size: 18.4 MB (18400373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8f048f32cc8c2c10e668e5de4da2c2fb6f21410107ed5a233a7c25cc6994ed`  
		Last Modified: Fri, 09 Dec 2022 03:48:14 GMT  
		Size: 191.2 MB (191223696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3effab4d2ab2ce23b6966dd48f71c31d3bb34d4a41170bdbff42e9ce9b49bc4`  
		Last Modified: Fri, 09 Dec 2022 03:48:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9a5de3191fbc6ece01337726ca0708d248ab0af4fff3fd159cb5baa580fc58`  
		Last Modified: Wed, 14 Dec 2022 00:48:45 GMT  
		Size: 54.4 MB (54391027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1850654f67fb6cac62b0fa4b935c31392376fccfde303fc4dbb2847cf927e1`  
		Last Modified: Wed, 14 Dec 2022 00:48:39 GMT  
		Size: 619.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17223705de15e2cb5242f989beae3a95665ea52e93db46f6b2b0fc1509c2c16a`  
		Last Modified: Wed, 14 Dec 2022 00:48:39 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
