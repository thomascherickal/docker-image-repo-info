## `clojure:lein`

```console
$ docker pull clojure@sha256:608287882ae75005386eb6cf6619d3ad2d0d2b2908a23114f89d12d749ca6125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:lein` - linux; amd64

```console
$ docker pull clojure@sha256:d18afa4e91fa0fe972779440a803e8cd82364fa1e7ebdfdc41e6ceadd3321ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256340160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4869a76ea825e14551ee04d96f8f98170951a2d5ce2a2ef5111d4d0329e2448a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Thu, 06 Oct 2022 03:58:54 GMT
ENV LEIN_VERSION=2.9.10
# Thu, 06 Oct 2022 03:58:54 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 06 Oct 2022 03:58:54 GMT
WORKDIR /tmp
# Thu, 06 Oct 2022 03:59:08 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Thu, 06 Oct 2022 03:59:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 06 Oct 2022 03:59:08 GMT
ENV LEIN_ROOT=1
# Thu, 06 Oct 2022 03:59:11 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 06 Oct 2022 03:59:11 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Thu, 06 Oct 2022 03:59:11 GMT
ENTRYPOINT ["entrypoint"]
# Thu, 06 Oct 2022 03:59:11 GMT
CMD ["repl"]
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
	-	`sha256:9e9bdc644d4ac630bf4309ee7eead6163338ff0743c7e4419dd8764da4b5168f`  
		Last Modified: Thu, 06 Oct 2022 04:14:04 GMT  
		Size: 12.4 MB (12380607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f6012190046bf287eb10d045488270499917d56c8a50fe6ef26f364e8b71b1`  
		Last Modified: Thu, 06 Oct 2022 04:14:04 GMT  
		Size: 4.4 MB (4398664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3bbec27d1c953ab7783b90b065580b72752799b3908fc10e07ccd1eb8fb79f`  
		Last Modified: Thu, 06 Oct 2022 04:14:03 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:lein` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:ee69ca7c3cb347ee522bd5d2532f001656b1f30530d23e9ad34cfd424225d072
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254490458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75610af244cfcaf9a8c1628e29970e1626a2540984debdf9851543cc86b0ef12`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

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
# Wed, 26 Oct 2022 15:47:25 GMT
ENV LEIN_VERSION=2.9.10
# Wed, 26 Oct 2022 15:47:25 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 26 Oct 2022 15:47:25 GMT
WORKDIR /tmp
# Wed, 26 Oct 2022 15:47:38 GMT
RUN set -eux; apt-get update && apt-get install -y make gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://codeberg.org/leiningen/leiningen/raw/tag/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "dbb84d13d6df5b85bbf7f89a39daeed103133c24a4686d037fe6bd65e38e7f32 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && export GNUPGHOME="$(mktemp -d)" && export FILENAME_EXT=jar && if printf '%s\n%s\n' "2.9.7" "$LEIN_VERSION" | sort -cV; then               gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 6A2D483DB59437EBB97D09B1040193357D0606ED;             else               gpg --batch --keyserver hkps://keyserver.ubuntu.com --recv-keys 20242BACBBE95ADA22D0AFD7808A33D379C806C3;               FILENAME_EXT=zip;             fi && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && wget -q https://codeberg.org/leiningen/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT && gpgconf --kill all && rm -rf "$GNUPGHOME" leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.$FILENAME_EXT /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Wed, 26 Oct 2022 15:47:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 26 Oct 2022 15:47:38 GMT
ENV LEIN_ROOT=1
# Wed, 26 Oct 2022 15:47:41 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.11.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 26 Oct 2022 15:47:41 GMT
COPY file:cf90f595e38d932dff3bdcd4221efe7c65fb3432787490053b55b6917f06e4cd in /usr/local/bin/entrypoint 
# Wed, 26 Oct 2022 15:47:41 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 26 Oct 2022 15:47:41 GMT
CMD ["repl"]
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
	-	`sha256:9d396b041176d4a1dc57f95ce1a22d3304ff01ba095e43f35fc7824878750f9c`  
		Last Modified: Wed, 26 Oct 2022 16:02:56 GMT  
		Size: 12.4 MB (12379192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea4d506ed98ea2c612d6d133bcadb1cb893fab7ac4c89d453dee9c07bba8a67`  
		Last Modified: Wed, 26 Oct 2022 16:02:55 GMT  
		Size: 4.4 MB (4398639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ab4f8e07f7195644ec417974844734c9f3b87f36536e8fc25ecdad029ad929`  
		Last Modified: Wed, 26 Oct 2022 16:02:55 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
