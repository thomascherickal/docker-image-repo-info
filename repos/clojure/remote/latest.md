## `clojure:latest`

```console
$ docker pull clojure@sha256:d0f1acfa9656f2dc5dc891f6e3bc3d69186e2f08c337e6508663ad9cbf51f4b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:latest` - linux; amd64

```console
$ docker pull clojure@sha256:63f5bb343f764029213d73c10bc764e3ea6a542cece2c77de1be220e8578eedb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.5 MB (365472263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8866cd9ad00214668ff6f16f79eb7b8facfffd6a7331f32dd24031157b49af9d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

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
# Wed, 05 Oct 2022 17:03:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:03:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 17:03:15 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 03:45:16 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 06 Oct 2022 03:45:16 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 06 Oct 2022 03:45:16 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:45:21 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 06 Oct 2022 03:45:21 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 06 Oct 2022 03:45:21 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 06 Oct 2022 03:46:01 GMT
RUN boot
# Thu, 06 Oct 2022 03:46:02 GMT
ENV LEIN_VERSION=2.9.10
# Thu, 06 Oct 2022 03:46:02 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 06 Oct 2022 03:46:02 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:46:25 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 06 Oct 2022 03:46:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Thu, 06 Oct 2022 03:46:25 GMT
ENV LEIN_ROOT=1
# Thu, 06 Oct 2022 03:46:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 06 Oct 2022 03:46:28 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Thu, 06 Oct 2022 03:46:28 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:46:46 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Thu, 06 Oct 2022 03:46:46 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Thu, 06 Oct 2022 03:46:46 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Thu, 06 Oct 2022 03:46:46 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 06 Oct 2022 03:46:47 GMT
CMD ["-M" "--repl"]
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
	-	`sha256:cdd77715f382e98938e79c50dd4e198e1ed0591a6e4d742c42ce76539de42b46`  
		Last Modified: Wed, 05 Oct 2022 17:10:20 GMT  
		Size: 192.1 MB (192145595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01940d6ad844857adae5eff7e87edb52b8913729617e44e0f36a7dab19831b2f`  
		Last Modified: Wed, 05 Oct 2022 17:10:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f19fe39b3b39c67b251a3af1eb9321b112e9082384830499dc62825fe61ad50`  
		Last Modified: Thu, 06 Oct 2022 04:06:09 GMT  
		Size: 338.5 KB (338532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e5961c5832b2a418ce52e097139d6d0de81760de6f083275820b36850421be`  
		Last Modified: Thu, 06 Oct 2022 04:06:13 GMT  
		Size: 58.8 MB (58820771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c2eb566c6e65fb28120d4d62a5ceec1e507ba8ea789df4788cac67fac87abd`  
		Last Modified: Thu, 06 Oct 2022 04:06:08 GMT  
		Size: 12.4 MB (12380509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb2785005188da95a08083a4c48b4da03dc02963aee28e3c5b6347f0383d0f`  
		Last Modified: Thu, 06 Oct 2022 04:06:07 GMT  
		Size: 4.4 MB (4398813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72a6ce013d947914ea2437c9272171a2d0e61f8e380a78eaa2ccbec8894485f`  
		Last Modified: Thu, 06 Oct 2022 04:06:14 GMT  
		Size: 50.0 MB (49972128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d9f27ebbf9a51a2c894a43662572ec388f621d9674e2329e14d0d3f90c601e`  
		Last Modified: Thu, 06 Oct 2022 04:06:07 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571d6aaf12e6f8614a7ad3c40f32116f9e06ec64beb41d8df06d3a1fd300fa40`  
		Last Modified: Thu, 06 Oct 2022 04:06:07 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:latest` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:6a63acbfb229a3e84275e08c5b7acbfccf28c8613522f0ca97aef08362ff798c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.6 MB (363574590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a633a675d5c8edcf542dc4ddb5820dd0119f919867d81845390fd8ca365c9f9d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

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
# Wed, 26 Oct 2022 01:12:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Oct 2022 01:12:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 01:12:29 GMT
CMD ["jshell"]
# Wed, 26 Oct 2022 15:33:35 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 26 Oct 2022 15:33:35 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:33:35 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:33:39 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:33:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:33:40 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 26 Oct 2022 15:34:20 GMT
RUN boot
# Wed, 26 Oct 2022 15:34:20 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 26 Oct 2022 15:34:20 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:34:20 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:34:39 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 26 Oct 2022 15:34:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Wed, 26 Oct 2022 15:34:40 GMT
ENV LEIN_ROOT=1
# Wed, 26 Oct 2022 15:34:42 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 26 Oct 2022 15:34:42 GMT
ENV CLOJURE_VERSION=1.11.1.1165
# Wed, 26 Oct 2022 15:34:42 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:34:56 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "72d662bdc99b79037f9e34996272384de35e01e0416d8eb79cc940ee0f0fc808 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 26 Oct 2022 15:34:56 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 26 Oct 2022 15:34:56 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 15:34:56 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 15:34:56 GMT
CMD ["-M" "--repl"]
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
	-	`sha256:57f760cd96c6aa0b1d070451e5f9d8f4ecefdf4172993c4e7183465f4ffd252a`  
		Last Modified: Wed, 26 Oct 2022 01:20:29 GMT  
		Size: 190.9 MB (190911164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fe3d0d60ddcdefddd94cc47a6dcd12ab9a1fd6c41d0e10ba3dc2a85484150`  
		Last Modified: Wed, 26 Oct 2022 01:20:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edb1db28e9bf5cc3c6758bda7470fd1445d05b00549ae61ce931e2168ce41cb`  
		Last Modified: Wed, 26 Oct 2022 15:55:34 GMT  
		Size: 338.6 KB (338648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b0b6c8f175c17cee3fff9259bc721085e46d7db9120301ec3d96e74f9d586a4`  
		Last Modified: Wed, 26 Oct 2022 15:55:37 GMT  
		Size: 58.8 MB (58821040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9c0d4fa6edd3e2b58ce6751ef7669ac5ccff57ceb40b5dd2f1ab3b782bbe23`  
		Last Modified: Wed, 26 Oct 2022 15:55:33 GMT  
		Size: 12.4 MB (12379091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe2d3f82d24265a78b4e6bc97d9e84b5f5b1a3ff163e973efb9ae72a76b0bc0`  
		Last Modified: Wed, 26 Oct 2022 15:55:32 GMT  
		Size: 4.4 MB (4398844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426ced6513ce7ecc6e3124dda04a95eaab0eb351cf9d2d9abf13e7c8b5ef47f2`  
		Last Modified: Wed, 26 Oct 2022 15:55:37 GMT  
		Size: 49.9 MB (49923718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6520fc8dfe498307279db33ea0fe148e7e630d90b828ed6873c1a32fa78d0d3e`  
		Last Modified: Wed, 26 Oct 2022 15:55:32 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfaf6a7a64010a234d0a69122df8ccbfd204c6270a8b475d827ff37a6528611`  
		Last Modified: Wed, 26 Oct 2022 15:55:32 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
