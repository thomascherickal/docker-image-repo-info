## `jruby:9-jdk8`

```console
$ docker pull jruby@sha256:1469ded7dbfb152846c8d872576d825fe2d3de1e29c34815911fbcbff11918fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:5474395f34331faa9339a1d4c30e99b9396d64285fa580f61cdad801deb49634
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137255564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ad4a0b1505256637e774bd7b98bb5442694e6e7a09d005cba6ef5255efd81b4`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:42:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 00:42:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 00:42:52 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 00:43:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:43:23 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 00:43:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:29 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:45 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:45 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:45 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:47 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:47 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:48 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:55 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:56 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:56 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7affba4c9a33ed5dd050532c0d53e38b2c35c2fe490db721d943658feee4c914`  
		Last Modified: Tue, 18 Apr 2023 00:46:23 GMT  
		Size: 16.3 MB (16347011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8107f6f9dfff8b155dc1a3eccd114e03005d9829897b75c3e4bca3f105cc4ad7`  
		Last Modified: Tue, 18 Apr 2023 00:46:27 GMT  
		Size: 54.6 MB (54635739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6ceef65c5b42e1bea0bf7ea3d1194b4c8e6252673bbf2c17812e120e8c51c6`  
		Last Modified: Tue, 18 Apr 2023 00:46:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f147e3503b2d223a1adb8b742ee6df0c88208169fb62c2390d0d4deea22f20b8`  
		Last Modified: Tue, 18 Apr 2023 05:12:02 GMT  
		Size: 7.1 MB (7066011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f9a8b57d075eeb925943ac2800b6d7e28150ad6b82a9f83a4577ea5c155c52`  
		Last Modified: Tue, 18 Apr 2023 05:12:02 GMT  
		Size: 29.5 MB (29529464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1e23319c43c37ed7ae8a89e2995249383db8d4d1d4dfa1908d4a5112d3030e`  
		Last Modified: Tue, 18 Apr 2023 05:12:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4b31e33a84b7b402a654b97c718822a5c0ca3ef428c4aeb4d23c69998d8356`  
		Last Modified: Tue, 18 Apr 2023 05:12:00 GMT  
		Size: 1.1 MB (1098217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0bc9478c64cdab63e2d2e95bbf085b4eb70ad5d670a26bc8eafde6fcdeab1d`  
		Last Modified: Tue, 18 Apr 2023 05:12:00 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:e638a3eb5b3f022cb6ff628fcf46cc1a285918692daf0794744312649b005e48
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133805220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e68cc8f3d5ae77c79fd13c3f21b4fd5db21d25c51ab3b37a6c251958d32dc3`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:40:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 18 Apr 2023 01:40:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:40:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:41:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:39:26 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 26 Apr 2023 19:39:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='195808eb42ab73535c84de05188914a52a47c1ac784e4bf66de95fe1fd315a5a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bb85303848fe402d4f1004f748f80ccb39cb11f356f50a513555d1083c3913b8';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='78a0b3547d6f3d46227f2ad8c774248425f20f1cd63f399b713f0cdde2cc376c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:34 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:19 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:11:19 GMT
ENV JRUBY_VERSION=9.4.2.0
# Wed, 26 Apr 2023 21:11:19 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Wed, 26 Apr 2023 21:11:21 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:11:21 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:11:22 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:11:28 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:11:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:11:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:11:29 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:11:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:11:29 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269336393c4662b72ac4a2be29473801366e79f4db6c8b9944509f1903ee3fe6`  
		Last Modified: Tue, 18 Apr 2023 01:43:30 GMT  
		Size: 16.2 MB (16213349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce798d5065b28a7b72ef136a86a11606e6ac727d9d05ebbba91bb64b23dbf9eb`  
		Last Modified: Wed, 26 Apr 2023 19:44:28 GMT  
		Size: 53.7 MB (53744562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398467c409835a760dbc962b3b4b35e2a478483559a0b2f9b39e827569fed32c`  
		Last Modified: Wed, 26 Apr 2023 19:44:23 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d459d82b1348e2ea4a2cfffb3783ad741bc781f28e15361bda5d2bc3d8034c09`  
		Last Modified: Wed, 26 Apr 2023 21:14:06 GMT  
		Size: 6.0 MB (6022751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3351b635b49c4b40e3c79d360385f7ca321a9e1ca3f64836821bb23f559617d`  
		Last Modified: Wed, 26 Apr 2023 21:14:07 GMT  
		Size: 29.5 MB (29529387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effe6b132c0854858d1dbd64983dcba2f3fa043e2d501dba7dba99eea7f0a5ff`  
		Last Modified: Wed, 26 Apr 2023 21:14:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a26b7c679935762b5691a14423e5633c3cf48d0a3ebc18eee36779d7af7b14`  
		Last Modified: Wed, 26 Apr 2023 21:14:05 GMT  
		Size: 1.1 MB (1098211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e583cbf2d227ef5e0001f4aa6e403b6206068c11b2bbfd04cff6a28dfd815e6`  
		Last Modified: Wed, 26 Apr 2023 21:14:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
