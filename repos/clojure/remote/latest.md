## `clojure:latest`

```console
$ docker pull clojure@sha256:cea42536833180cf6651ae40651e28afb1fe6873f6d9a01d68eb10a41453390f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:latest` - linux; amd64

```console
$ docker pull clojure@sha256:2c6ffebb941251f08fb53d789c398e3a91b41d7e1ca7d6edbdf2f23e94a428db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.5 MB (365485626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d5260fc5514b4a259250500c0e18ece5e3d489a97a3949486e99082ad5cd27d`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:20:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:20:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:20:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:23:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:22:35 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:22:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:22:47 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:22:47 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 21:46:59 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 21:47:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:47:00 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:47:05 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 21:47:06 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 21:47:06 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 21:47:38 GMT
RUN boot
# Wed, 24 Aug 2022 21:47:39 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 24 Aug 2022 21:47:39 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 21:47:39 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:47:58 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 24 Aug 2022 21:47:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Wed, 24 Aug 2022 21:47:59 GMT
ENV LEIN_ROOT=1
# Wed, 24 Aug 2022 21:48:01 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 Aug 2022 21:48:01 GMT
ENV CLOJURE_VERSION=1.11.1.1155
# Wed, 24 Aug 2022 21:48:01 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:48:23 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7eb9aa2ecc6c0abfdb1578d4b99ca7c2055111aafa38524a12a6fb76fe01f30b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 21:48:24 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 Aug 2022 21:48:24 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 21:48:24 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 21:48:24 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ffabbc7d493a0023d83d0a6b1e82866abef587a22c60708a4f07dda563de6a`  
		Last Modified: Fri, 12 Aug 2022 17:32:48 GMT  
		Size: 17.0 MB (17001621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccfedeac8a2a9fca5cf85459e4d8ab26541dd8c95ced8d1805079f8b85b57d5`  
		Last Modified: Wed, 24 Aug 2022 19:29:43 GMT  
		Size: 192.1 MB (192145526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ae17c2165b6ecce719bf8712cc3d4856f1a7ed64282129177e222e9ae9e21d`  
		Last Modified: Wed, 24 Aug 2022 19:29:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e0d5f86d172b9968b5881e56ccabea7e754a002a059696288ec30b4c025b1`  
		Last Modified: Wed, 24 Aug 2022 21:57:06 GMT  
		Size: 338.1 KB (338090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a824406c35182145957cf1f607d0387b4307208956fe087c38ed0724d622cb`  
		Last Modified: Wed, 24 Aug 2022 21:57:10 GMT  
		Size: 58.8 MB (58820798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089f9afd7520a7188f9169fd4da62472dde4b12b6267706e85b3caf14404e4f4`  
		Last Modified: Wed, 24 Aug 2022 21:57:05 GMT  
		Size: 12.4 MB (12380019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:febb99bee666734af23dadd787629ec7ba143866aa886a973ed3df2a6f1e1728`  
		Last Modified: Wed, 24 Aug 2022 21:57:04 GMT  
		Size: 4.4 MB (4398845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c444d4056a926754edc047b3c61272f93739d9db9ff990cb12278bd1487b2084`  
		Last Modified: Wed, 24 Aug 2022 21:57:10 GMT  
		Size: 50.0 MB (49973392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1997af74a64ceb05bb253d73f2ddceac075152df81c69886126814f62073e58f`  
		Last Modified: Wed, 24 Aug 2022 21:57:04 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9078a4ea362f78d3824668f898b6e7795cb77866585dcab6787410ef09e7b7`  
		Last Modified: Wed, 24 Aug 2022 21:57:04 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:latest` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ed998afceec9b0462b122bdd90a0f7fc31fbca9173e8e9df9b69d9b0f5f92414
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.9 MB (362877216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b768b334e2570cd852094611056db57001c8dfa8fbf58675ffa28eb87136dfb`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:40:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:40:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:40:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:45:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:42:41 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 24 Aug 2022 19:42:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:42:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 19:42:52 GMT
CMD ["jshell"]
# Wed, 24 Aug 2022 20:10:21 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 24 Aug 2022 20:10:21 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 20:10:22 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 20:10:29 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 20:10:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 24 Aug 2022 20:10:31 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 24 Aug 2022 20:11:04 GMT
RUN boot
# Wed, 24 Aug 2022 20:11:04 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 24 Aug 2022 20:11:05 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 24 Aug 2022 20:11:06 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 20:11:34 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 24 Aug 2022 20:11:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/:/usr/local/bin/
# Wed, 24 Aug 2022 20:11:35 GMT
ENV LEIN_ROOT=1
# Wed, 24 Aug 2022 20:11:39 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 Aug 2022 20:11:39 GMT
ENV CLOJURE_VERSION=1.11.1.1155
# Wed, 24 Aug 2022 20:11:40 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 20:11:59 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7eb9aa2ecc6c0abfdb1578d4b99ca7c2055111aafa38524a12a6fb76fe01f30b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 20:12:00 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 Aug 2022 20:12:01 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 20:12:01 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 20:12:02 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3daf49bfff4711ea3e9c4de6d7bb8d1733d4b962c4d277384d83f2d8d98f367`  
		Last Modified: Fri, 12 Aug 2022 17:56:05 GMT  
		Size: 18.4 MB (18434264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca022bbec64d92dd58c0246cd5520942fd998a3277546294d650b0373c0cde`  
		Last Modified: Wed, 24 Aug 2022 19:50:04 GMT  
		Size: 190.9 MB (190911160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bd1319327319d407c465329e74dc805345b562186efe01bc77764df1111612`  
		Last Modified: Wed, 24 Aug 2022 19:49:44 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7874c2f86ffbae21d2747eeba62d9e3709cdc3b695790ffb09642c05e03aff`  
		Last Modified: Wed, 24 Aug 2022 20:22:10 GMT  
		Size: 101.2 KB (101203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee3da76eaab384809ef3bb671d13ac65a9d188c61b2a5852af9480a3a72fcf`  
		Last Modified: Wed, 24 Aug 2022 20:22:13 GMT  
		Size: 58.8 MB (58816470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201bbbdf0cca256706f36b38ea305e66ba2f9696c1c62a1aa03fef732711bbde`  
		Last Modified: Wed, 24 Aug 2022 20:22:08 GMT  
		Size: 12.1 MB (12140712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ac5f0dba8b4074c8a9ba133374ca60dc7580b042721ae9a21ac0beed7ad824`  
		Last Modified: Wed, 24 Aug 2022 20:22:07 GMT  
		Size: 4.4 MB (4398579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15c61de068d37c9f6ae77387290d55fa1329ca82d3dd98e0b2da5264484cd60`  
		Last Modified: Wed, 24 Aug 2022 20:22:14 GMT  
		Size: 49.7 MB (49692490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dea6fd305e9a6ff441959d569c3ac5f77cbe19144f5a951a224cb44990fea8`  
		Last Modified: Wed, 24 Aug 2022 20:22:07 GMT  
		Size: 622.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec91dd6e8f3898c75a415d9cdd9c3fe9dee2545394e49126f4333f03577ad36`  
		Last Modified: Wed, 24 Aug 2022 20:22:07 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
