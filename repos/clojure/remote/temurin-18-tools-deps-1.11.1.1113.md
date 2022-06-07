## `clojure:temurin-18-tools-deps-1.11.1.1113`

```console
$ docker pull clojure@sha256:ab9053b91204d31c98c9f75b20cf3d8282f9eb94a0658106c8568dbe894b86fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-18-tools-deps-1.11.1.1113` - linux; amd64

```console
$ docker pull clojure@sha256:6d3c01764b0cf0a770968625ab0a18e7877ee59f7b932b162336439b0889c7e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304645395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:688f50eabf95b6145cfb5eb0a6e795a9cd183d40958d08394a5be375a3b26a12`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:15:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:16:35 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 07 Jun 2022 00:16:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37ceaf232a85cce46bcccfd71839854e8b14bf3160e7ef72a676b9cae45ee8af';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='0ddec3c165ab0b662a57a845db3fdaeb840660b493f164696b03df76aadf61c8';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7c3376b4eb14a58d27816776e965f1b214c17c4c2e918dc9e996a0f30e76550e';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='236dc78e698c21f258078661ab5c74b8cc7d38a1febb7aa7a6598bd3b999c0dc';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='16b1d9d75f22c157af04a1fd9c664324c7f4b5163c022b382a2f2e8897c1b0a2';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 00:16:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 00:16:49 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 00:16:49 GMT
CMD ["jshell"]
# Tue, 07 Jun 2022 04:46:28 GMT
ENV CLOJURE_VERSION=1.11.1.1113
# Tue, 07 Jun 2022 04:46:28 GMT
WORKDIR /tmp
# Tue, 07 Jun 2022 04:46:44 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7677bb1179ebb15ebf954a87bd1078f1c547673d946dadafd23ece8cd61f5a9f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Tue, 07 Jun 2022 04:46:44 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 07 Jun 2022 04:46:44 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 07 Jun 2022 04:46:45 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 07 Jun 2022 04:46:45 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32598539a8f0b55be77078c6637866fc4128a4213ea59e9993662a310a2b711`  
		Last Modified: Tue, 07 Jun 2022 00:22:05 GMT  
		Size: 19.8 MB (19773881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab1e3bdf3dcc14af31e9535f736da5c91bb9add2ad5a162cd3e86d867ab634a`  
		Last Modified: Tue, 07 Jun 2022 00:23:46 GMT  
		Size: 193.5 MB (193544180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59651909abe6d6a31a9aa05a896765e01e80010d983522cbbce07891da8c499f`  
		Last Modified: Tue, 07 Jun 2022 00:23:32 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6628d5629679bc2b0a3361eaf154bc85f70a980fc28ae66be16dca93b9bbc23`  
		Last Modified: Tue, 07 Jun 2022 04:50:39 GMT  
		Size: 62.8 MB (62753520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ed068a2410a891ba671d997ffd1c279c2a84c31bba45cfafe3e4552880ea2d`  
		Last Modified: Tue, 07 Jun 2022 04:50:30 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901f5cc83cddc9a23dad14cffffbaac26a2cdb846fc165541806e856dfb40df4`  
		Last Modified: Tue, 07 Jun 2022 04:50:30 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-18-tools-deps-1.11.1.1113` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:b9eace5f53c69a88c28493b745c74ef5baa78b32dde5e8abc8e8e45038a958d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302680435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ae898b0b66aee2e403e15982869a9ce89c52c32da880bae6d62d85f476483a`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 04 May 2022 17:42:24 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 17:42:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37ceaf232a85cce46bcccfd71839854e8b14bf3160e7ef72a676b9cae45ee8af';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='0ddec3c165ab0b662a57a845db3fdaeb840660b493f164696b03df76aadf61c8';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7c3376b4eb14a58d27816776e965f1b214c17c4c2e918dc9e996a0f30e76550e';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='236dc78e698c21f258078661ab5c74b8cc7d38a1febb7aa7a6598bd3b999c0dc';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='16b1d9d75f22c157af04a1fd9c664324c7f4b5163c022b382a2f2e8897c1b0a2';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 04 May 2022 17:42:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 May 2022 17:42:39 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 04 May 2022 17:42:39 GMT
CMD ["jshell"]
# Wed, 04 May 2022 18:53:30 GMT
ENV CLOJURE_VERSION=1.11.1.1113
# Wed, 04 May 2022 18:53:31 GMT
WORKDIR /tmp
# Wed, 04 May 2022 18:53:51 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "7677bb1179ebb15ebf954a87bd1078f1c547673d946dadafd23ece8cd61f5a9f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Wed, 04 May 2022 18:53:52 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Wed, 04 May 2022 18:53:53 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Wed, 04 May 2022 18:53:53 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 04 May 2022 18:53:54 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb838ee3b38b60e84012b6193ab83e74d7c63751ef15100b396edb10b02a5e0`  
		Last Modified: Wed, 04 May 2022 17:45:52 GMT  
		Size: 192.4 MB (192377858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922cda8184457eff7386c6bc438f49b8129a04bf49c06431b169dec7768effd6`  
		Last Modified: Wed, 04 May 2022 17:45:32 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872982ac9e9e91ac17f1e1f66f311177faecd20e96083ccee8597b013da0ecd2`  
		Last Modified: Wed, 04 May 2022 18:59:43 GMT  
		Size: 62.6 MB (62632690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4aa0460e66ab9ba7385aa462dc9ebd6e59bcbf3dc3be6660d70a590cf6385c`  
		Last Modified: Wed, 04 May 2022 18:59:35 GMT  
		Size: 617.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a6ee4ac2626f9e271adc6923c1f9f22f26e427d32567f86e86f47ee2bf00bd`  
		Last Modified: Wed, 04 May 2022 18:59:35 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
