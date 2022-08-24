## `clojure:temurin-17-tools-deps`

```console
$ docker pull clojure@sha256:1da3ab5bb1da82ba69891fa92edf9995507800939335eb55fb6aff54a61ab619
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-17-tools-deps` - linux; amd64

```console
$ docker pull clojure@sha256:8ca1eca1146b1875082d37630cb39a5b4208cd726b9893cd002d580cf5b6c4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (293982991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3281bce3a809548758ffd1ae3b40e00f40498e9073d546a3bce07be401cd8038`
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
# Wed, 24 Aug 2022 21:54:31 GMT
ENV CLOJURE_VERSION=1.11.1.1155
# Wed, 24 Aug 2022 21:54:32 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 21:54:44 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7eb9aa2ecc6c0abfdb1578d4b99ca7c2055111aafa38524a12a6fb76fe01f30b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 21:54:45 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 Aug 2022 21:54:45 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 21:54:45 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 21:54:45 GMT
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
	-	`sha256:4b82c943fef7c831a974a36f35806b7d36c1821a600d6a62a8c19fc4983d0c3d`  
		Last Modified: Wed, 24 Aug 2022 22:02:51 GMT  
		Size: 54.4 MB (54408510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c7721c90a5eeb82b57890cdb8039131acbf665a01d709e5d23e906e966a6a4`  
		Last Modified: Wed, 24 Aug 2022 22:02:45 GMT  
		Size: 620.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a841d95c9a986b93f115b4cda93aa2ba675f1bc0acc27ea3911b38de6038251`  
		Last Modified: Wed, 24 Aug 2022 22:02:45 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-17-tools-deps` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:be9d6b2643e31308fdae3a6fe7759b63b073c34c66e7a4e159198240bb582489
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291864789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dc91818fdec5b611e8adc3278d47189adc13ff7ec8a401b3e8501c019c7e24d`
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
# Wed, 24 Aug 2022 20:18:16 GMT
ENV CLOJURE_VERSION=1.11.1.1155
# Wed, 24 Aug 2022 20:18:17 GMT
WORKDIR /tmp
# Wed, 24 Aug 2022 20:18:37 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7eb9aa2ecc6c0abfdb1578d4b99ca7c2055111aafa38524a12a6fb76fe01f30b *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 24 Aug 2022 20:18:38 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 24 Aug 2022 20:18:39 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 24 Aug 2022 20:18:39 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 24 Aug 2022 20:18:40 GMT
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
	-	`sha256:aae681d8956c8cc001ac5f453b7052fd9c8b6fab3474ddc55bddf00c62bd4546`  
		Last Modified: Wed, 24 Aug 2022 20:27:08 GMT  
		Size: 54.1 MB (54137028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e77434cfd2a4ab540f88477154f80820c2d7e818d583b510439878176e38f6`  
		Last Modified: Wed, 24 Aug 2022 20:27:00 GMT  
		Size: 621.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39d7f0a2db39dbbce9c49baa664bcdfffaa642d29e0ce9f28ceeb8b69b669f4`  
		Last Modified: Wed, 24 Aug 2022 20:27:00 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
