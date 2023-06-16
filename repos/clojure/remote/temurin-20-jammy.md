## `clojure:temurin-20-jammy`

```console
$ docker pull clojure@sha256:a749775c0fedacd5a8077092fbe4e6f0ff54f874c138497ab0161d30721e5e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-20-jammy` - linux; amd64

```console
$ docker pull clojure@sha256:a18e76cc946481f7e42df32537689206716c8453f08d6eb65df6c2f8edca9114
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.1 MB (307147851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ef0f260afba9b59a44be660bdec0668f4020fba2d8ac574644ae1b0f45d3fc`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:42:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Jun 2023 01:42:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 01:42:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Jun 2023 01:44:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:45:17 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Fri, 02 Jun 2023 01:45:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b16c0271899de1f0e277dc0398bfff11b54511765f104fa938929ac484dc926d';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_aarch64_linux_hotspot_20.0.1_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43ad054f135a7894dc87ad5d10ad45d8e82846186515892acdbc17c2c5cd27e4';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_x64_linux_hotspot_20.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 02 Jun 2023 01:45:30 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 02 Jun 2023 01:45:30 GMT
CMD ["jshell"]
# Mon, 05 Jun 2023 21:05:32 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Mon, 05 Jun 2023 21:05:32 GMT
WORKDIR /tmp
# Mon, 05 Jun 2023 21:05:47 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Mon, 05 Jun 2023 21:05:47 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Mon, 05 Jun 2023 21:05:47 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Mon, 05 Jun 2023 21:05:47 GMT
ENTRYPOINT ["entrypoint"]
# Mon, 05 Jun 2023 21:05:47 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec73b48ae406646223453ca41d5d6b7cb739853fb7a44f15d35a31c238271d2`  
		Last Modified: Fri, 02 Jun 2023 01:48:00 GMT  
		Size: 17.0 MB (17038759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b9bf172390f0282ae3bd50b03af0e2024a6db94896fde260eb482512b137ea`  
		Last Modified: Fri, 02 Jun 2023 01:48:54 GMT  
		Size: 202.8 MB (202822845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d6d89e7f4c8b47896ba91795280fa03669ff6b6a92ebfb71f9b9d536103320`  
		Last Modified: Fri, 02 Jun 2023 01:48:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4792780c7ac0eaf915a143754f2122cf2aedc3eb3dc1f171441d6ba4836dc01a`  
		Last Modified: Mon, 05 Jun 2023 21:13:14 GMT  
		Size: 56.9 MB (56854778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433f37d0b1bcfa388845774211efae97694c80f155400d3b1fef9a480351b92b`  
		Last Modified: Mon, 05 Jun 2023 21:13:07 GMT  
		Size: 618.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e714f66a1066b3412c4f7b91f5db83d50fa398bf6c157caffa4b72525afa712b`  
		Last Modified: Mon, 05 Jun 2023 21:13:07 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-20-jammy` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:012dd2a211df22d490f7cd04932380996c2c49712222b3d46619315d3243cdf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.5 MB (302531155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b939767ff2a741a6b35dd5630e1aefdf27d3a9a33b503a00d02c5d926c6728dd`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:47:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:48:31 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Fri, 16 Jun 2023 02:48:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b16c0271899de1f0e277dc0398bfff11b54511765f104fa938929ac484dc926d';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_aarch64_linux_hotspot_20.0.1_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43ad054f135a7894dc87ad5d10ad45d8e82846186515892acdbc17c2c5cd27e4';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20.0.1%2B9/OpenJDK20U-jdk_x64_linux_hotspot_20.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:48:45 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 02:48:45 GMT
CMD ["jshell"]
# Fri, 16 Jun 2023 04:50:48 GMT
ENV CLOJURE_VERSION=1.11.1.1347
# Fri, 16 Jun 2023 04:50:48 GMT
WORKDIR /tmp
# Fri, 16 Jun 2023 04:50:59 GMT
RUN apt-get update && apt-get install -y make git rlwrap wget && rm -rf /var/lib/apt/lists/* && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "d9158bf3a1d92fbf8551656e47a86f42e93d10f1db9defa2124bfee206ce8c8f *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apt-get purge -y --auto-remove wget
# Fri, 16 Jun 2023 04:51:00 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Fri, 16 Jun 2023 04:51:00 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Fri, 16 Jun 2023 04:51:00 GMT
ENTRYPOINT ["entrypoint"]
# Fri, 16 Jun 2023 04:51:00 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168066327b37e44f2a0ef7f788219bdbcd9013e4320cf4b9229ea9dfb73b561`  
		Last Modified: Fri, 16 Jun 2023 02:52:08 GMT  
		Size: 18.5 MB (18465563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a70544ab7e663fb70e44bb56b5a0e812bdccf31d918e20a55be862f970fd40`  
		Last Modified: Fri, 16 Jun 2023 02:53:07 GMT  
		Size: 201.2 MB (201166434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6eb21fe540057f6a516455d71b9d751ff5ce3e18e099ff32b7f3be8a52330f`  
		Last Modified: Fri, 16 Jun 2023 02:52:55 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633d0abecc0e1ce171bf6376ff77d637b28ee65f40fa574e5c66ce341749c719`  
		Last Modified: Fri, 16 Jun 2023 05:00:43 GMT  
		Size: 54.5 MB (54508767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359757c3ae61ac9cd994c8189f97245087375cc03c558e25cd3b6114cabb7c78`  
		Last Modified: Fri, 16 Jun 2023 05:00:38 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfac6a80b855536118e8db1bfd5cdee319ac4c0879f6b7145e68332de56cf04`  
		Last Modified: Fri, 16 Jun 2023 05:00:38 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
