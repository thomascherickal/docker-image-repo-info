<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `jruby`

-	[`jruby:9`](#jruby9)
-	[`jruby:9-jdk`](#jruby9-jdk)
-	[`jruby:9-jdk8`](#jruby9-jdk8)
-	[`jruby:9.3`](#jruby93)
-	[`jruby:9.3-jdk`](#jruby93-jdk)
-	[`jruby:9.3-jdk11`](#jruby93-jdk11)
-	[`jruby:9.3-jdk17`](#jruby93-jdk17)
-	[`jruby:9.3-jdk8`](#jruby93-jdk8)
-	[`jruby:9.3-jre`](#jruby93-jre)
-	[`jruby:9.3-jre11`](#jruby93-jre11)
-	[`jruby:9.3-jre8`](#jruby93-jre8)
-	[`jruby:9.3.10`](#jruby9310)
-	[`jruby:9.3.10-jdk`](#jruby9310-jdk)
-	[`jruby:9.3.10-jdk11`](#jruby9310-jdk11)
-	[`jruby:9.3.10-jdk17`](#jruby9310-jdk17)
-	[`jruby:9.3.10-jdk8`](#jruby9310-jdk8)
-	[`jruby:9.3.10-jre`](#jruby9310-jre)
-	[`jruby:9.3.10-jre11`](#jruby9310-jre11)
-	[`jruby:9.3.10-jre8`](#jruby9310-jre8)
-	[`jruby:9.3.10.0`](#jruby93100)
-	[`jruby:9.3.10.0-jdk`](#jruby93100-jdk)
-	[`jruby:9.3.10.0-jdk11`](#jruby93100-jdk11)
-	[`jruby:9.3.10.0-jdk17`](#jruby93100-jdk17)
-	[`jruby:9.3.10.0-jdk8`](#jruby93100-jdk8)
-	[`jruby:9.3.10.0-jre`](#jruby93100-jre)
-	[`jruby:9.3.10.0-jre11`](#jruby93100-jre11)
-	[`jruby:9.3.10.0-jre8`](#jruby93100-jre8)
-	[`jruby:9.4`](#jruby94)
-	[`jruby:9.4-jdk`](#jruby94-jdk)
-	[`jruby:9.4-jdk11`](#jruby94-jdk11)
-	[`jruby:9.4-jdk17`](#jruby94-jdk17)
-	[`jruby:9.4-jdk8`](#jruby94-jdk8)
-	[`jruby:9.4-jre`](#jruby94-jre)
-	[`jruby:9.4-jre11`](#jruby94-jre11)
-	[`jruby:9.4-jre8`](#jruby94-jre8)
-	[`jruby:9.4.2`](#jruby942)
-	[`jruby:9.4.2-jdk`](#jruby942-jdk)
-	[`jruby:9.4.2-jdk11`](#jruby942-jdk11)
-	[`jruby:9.4.2-jdk17`](#jruby942-jdk17)
-	[`jruby:9.4.2-jdk8`](#jruby942-jdk8)
-	[`jruby:9.4.2-jre`](#jruby942-jre)
-	[`jruby:9.4.2-jre11`](#jruby942-jre11)
-	[`jruby:9.4.2-jre8`](#jruby942-jre8)
-	[`jruby:9.4.2.0`](#jruby9420)
-	[`jruby:9.4.2.0-jdk`](#jruby9420-jdk)
-	[`jruby:9.4.2.0-jdk11`](#jruby9420-jdk11)
-	[`jruby:9.4.2.0-jdk17`](#jruby9420-jdk17)
-	[`jruby:9.4.2.0-jdk8`](#jruby9420-jdk8)
-	[`jruby:9.4.2.0-jre`](#jruby9420-jre)
-	[`jruby:9.4.2.0-jre11`](#jruby9420-jre11)
-	[`jruby:9.4.2.0-jre8`](#jruby9420-jre8)
-	[`jruby:latest`](#jrubylatest)

## `jruby:9`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9-jdk`

```console
$ docker pull jruby@sha256:1469ded7dbfb152846c8d872576d825fe2d3de1e29c34815911fbcbff11918fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9-jdk` - linux; amd64

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

### `jruby:9-jdk` - linux; arm64 variant v8

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

## `jruby:9.3`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk`

```console
$ docker pull jruby@sha256:d37b51b897e82d483e7a013532dec71c144e1df57c5ad1e5cddb2f9af654d089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:b52e54daad1d0ddf7cc5720bd88da02a84c56f4159c2280588457f6c107ea1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136550087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1758c12db58cf794a075c563243beb970961ac4e2bd8e0a49882eac2ee9667b8`
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
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:14 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:22 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:23 GMT
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
	-	`sha256:13bd82f79d5a1a62a0eeb4bdb8a066d4e1a50668212cba0a444abdb7d3b2456c`  
		Last Modified: Tue, 18 Apr 2023 05:13:26 GMT  
		Size: 28.9 MB (28854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f4dce994ee128038d2145308632a06e9c60334080ef57d63688bfc3e4aad9`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f943e1e3ab27cbe48f31121fc18a7f13f89d99942b99709bfc38a436d7ffa`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 1.1 MB (1067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260efdb780214e7ad07ae619863a47142a5a51a1f804ae3ddb7a74fe9845857`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jdk` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:9b2bc521d74049439075993f655c3ed9a64926f328a82b710f4034dec2b4fec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133099794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9000ddce609d3db7e72bd994fa7c9fad87dc906bc1867e053bac204012cf1ea5`
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
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:31 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:31 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:32 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:39 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:39 GMT
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
	-	`sha256:bc99126de627cde0ce0d495e42d48986963f7064f652ba12f98d03421a09cca3`  
		Last Modified: Wed, 26 Apr 2023 21:15:28 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974a36338b571a9f29a9fe51aed3849d56f72ee959075d3474e5197dd162c30`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6d13ee8693152d2b057fbef22807cae24af97dca4ca5c68f168dfe5cea2f2`  
		Last Modified: Wed, 26 Apr 2023 21:15:27 GMT  
		Size: 1.1 MB (1067771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d31c7b477c926c1a10820b77dc20a69c09970ad57815c8879158f891c58656`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk11`

```console
$ docker pull jruby@sha256:610d3d7c88af591d4be546b68cdb132683223f1e9410e4df20b5f19814a04649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:3c200e1d084efdec62333fa0d84941fd8fb7c34b1987a0f4492ef58582ad1787
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280402518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1499dcbdf4747d1141d6ee7f6737be663911d3469b359bd82de6f69ee6ecaaa`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:04 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:24 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:40 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:40 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:42 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:42 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:50 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:50 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:51 GMT
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
	-	`sha256:92c807db9f3053b04e5e7309b190d1af31a410554295b83b7e42ebd37d795fbc`  
		Last Modified: Tue, 18 Apr 2023 00:47:07 GMT  
		Size: 198.5 MB (198488083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff7975ce69e8bb8b5432bab0d34d5de1e7798930490c9cc19d7121bdda9227`  
		Last Modified: Tue, 18 Apr 2023 00:46:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e486a90411bbeb5de2cdc83a866e2e92d3bacee895c402a91b84da503ecd6d1`  
		Last Modified: Tue, 18 Apr 2023 05:12:37 GMT  
		Size: 7.1 MB (7066139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce41fe69752bcd928957b8afc524331c882bd25803f285bc08751f64a69a64f`  
		Last Modified: Tue, 18 Apr 2023 05:13:58 GMT  
		Size: 28.9 MB (28854366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b25beafeb0cfed6e0439a393fb20af81ddc2b3862af8a62eff8a6522b81869`  
		Last Modified: Tue, 18 Apr 2023 05:13:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590c2f785f0e870999aff11d043e5bf4e7421e4c6eb3b12f6462b653ff1f0040`  
		Last Modified: Tue, 18 Apr 2023 05:13:56 GMT  
		Size: 1.1 MB (1067780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888704e582e054cf552e370fdd99db00d15b0c8c7ab8c19e100170a74ca3ffe2`  
		Last Modified: Tue, 18 Apr 2023 05:13:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jdk11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:8c88db1cb100623c1a8eeabb396bda194a4d95cc8f206bca313ee74cc1d627d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274685130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008a89533d32fcb9238b7234e26039d419a117312fb02bfeaeb20b8d08b5bf68`
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
# Wed, 26 Apr 2023 19:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:40:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0c7763a19b4af4ef5fbae831781b5184e988d6f131d264482399eeaf51b6e254';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='be07af349f0d2e1ffb7e01e1e8bac8bffd76e22f6cc1354e5b627222e3395f41';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1e3704c8e155f8f894953c2a6708a52e6f449bbf5a85450be6fbb2ec76581700';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a21e2c30e48df0b7238691833316c008167cbedd4e2f1e677bcb81638420d273';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f19fb28aea3e28fcc402b73ce72f62b602992d48769502effe81c52ca39a581';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:40:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:40:27 GMT
CMD ["jshell"]
# Wed, 26 Apr 2023 21:11:51 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:52 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:52 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:53 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:54 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:54 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:13:01 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:13:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:01 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:01 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:13:01 GMT
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
	-	`sha256:9999759029cca08e4ce40a4073366c9227d73a0dc73a4189707c47ba63614239`  
		Last Modified: Wed, 26 Apr 2023 19:46:24 GMT  
		Size: 195.3 MB (195329906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381a1f91095e95d49250dc06174f0a706bf1c1cef39bcf630a44291c6bb8d2f1`  
		Last Modified: Wed, 26 Apr 2023 19:46:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4304b09b2e14df7ab5f5399e7322776b41ab45d2212cb31a82143c28553a4345`  
		Last Modified: Wed, 26 Apr 2023 21:14:39 GMT  
		Size: 6.0 MB (6022734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f2384cb1ece4a1412929aeb7a5540ff43a6b9abfdb1532c1f4e9777b9e925`  
		Last Modified: Wed, 26 Apr 2023 21:15:58 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c3298269d59244d91c0a9e953678382b1dff381316322b50eb257a14d58159`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed69875dd90217f307de80246c652f48730bdaa2b0388eed1c6301035190e88`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 1.1 MB (1067766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0e89953f961d10b03b3aab459ae7c1c56c4d3ea757ef3dc082d29d509b2b6`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk17`

```console
$ docker pull jruby@sha256:ccdc5ab2c88a9160b3192f2453ac9c206c52ae1af374c9a3217cbc1458994406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:4c3b49c50b62035b5ab25682193f44f6957f290bc1c444ce2833a1bf2b8d8813
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.1 MB (278114916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9039a254bdc7d05e52f3cc54ca135cf438db5d660232bec0f9cba3b920fcc0f8`
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
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:58 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:44 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:54 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:54 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:55 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:56 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:56 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:11:03 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:11:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:11:04 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:11:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:11:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ebc9b7986f0210261b9474e28924822358a3e7811682aa6991dfdc2eed3ae`  
		Last Modified: Tue, 18 Apr 2023 00:47:49 GMT  
		Size: 192.4 MB (192448102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd987ac8d27cbef298907f5f282f9e895970ba27e01a15d63ac9131563958a`  
		Last Modified: Tue, 18 Apr 2023 00:47:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419e06a88be997f34d392d377eacd6ff8d1e44759a26af8e6348521015cfa83`  
		Last Modified: Tue, 18 Apr 2023 05:12:49 GMT  
		Size: 7.1 MB (7068634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67056faac3b2fc1bfd244bfb7567cf0ffdc1a813545cfafdcee6022fb652653`  
		Last Modified: Tue, 18 Apr 2023 05:14:10 GMT  
		Size: 28.9 MB (28854412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffafd6c6b82b150e9d28f97c806410d6aca154e70b293cd69e8ceeb03ccd4ee0`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b630b06c183344558b33d52eeddc4ebd5b714775253d35379fcc969c9b5a5`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 1.1 MB (1067791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36eb6c5faab521e347e0e433546d76a0b57945fa7953db9ce5ec4bb7897ece12`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jdk17` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:57fd853e9581896ed0001aa86de2590cd1e1bd0c81479f36510cd9c51ab6e1ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275363024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55207dc90975bb1c92aa41b4f9047076d660e435dc195ccfdf0af050578c090b`
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
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:41:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:44 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:41:44 GMT
CMD ["jshell"]
# Wed, 26 Apr 2023 21:12:07 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:13:03 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:13:03 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:13:05 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:13:05 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:05 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:13:12 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:13:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:12 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:13:13 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cfbead4ab6695e8e5082cf21969d8cddd4af6f02659c98db80315b6bc00b20`  
		Last Modified: Wed, 26 Apr 2023 19:48:47 GMT  
		Size: 191.4 MB (191403797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab5928b774148eca0fea966342b3695c4c7286fc929cff74ef4fca20bf40f1`  
		Last Modified: Wed, 26 Apr 2023 19:48:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4e0550462389ef34286af33d4ef72e8242b1e1f8852252cc044b4d20008fa`  
		Last Modified: Wed, 26 Apr 2023 21:14:51 GMT  
		Size: 6.0 MB (6024913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c964f7e85fa27454c24288bc2b7fa8a12e9fd9fab098cd5a30b10ea6371219c`  
		Last Modified: Wed, 26 Apr 2023 21:16:10 GMT  
		Size: 28.9 MB (28854360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfab3e27262aaae06fa315053c2a2549fdb9fc632aea8dc7a666f016a850577`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba76649e9e0f62efbc916a5f57134dabacceb42348461adb855118bfdbbe531`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 1.1 MB (1067782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506eaf359b5d3dcb4af226b3219e002d347c5870221297a1c956e55e0472b74`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jdk8`

```console
$ docker pull jruby@sha256:d37b51b897e82d483e7a013532dec71c144e1df57c5ad1e5cddb2f9af654d089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:b52e54daad1d0ddf7cc5720bd88da02a84c56f4159c2280588457f6c107ea1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136550087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1758c12db58cf794a075c563243beb970961ac4e2bd8e0a49882eac2ee9667b8`
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
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:14 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:22 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:23 GMT
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
	-	`sha256:13bd82f79d5a1a62a0eeb4bdb8a066d4e1a50668212cba0a444abdb7d3b2456c`  
		Last Modified: Tue, 18 Apr 2023 05:13:26 GMT  
		Size: 28.9 MB (28854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f4dce994ee128038d2145308632a06e9c60334080ef57d63688bfc3e4aad9`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f943e1e3ab27cbe48f31121fc18a7f13f89d99942b99709bfc38a436d7ffa`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 1.1 MB (1067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260efdb780214e7ad07ae619863a47142a5a51a1f804ae3ddb7a74fe9845857`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:9b2bc521d74049439075993f655c3ed9a64926f328a82b710f4034dec2b4fec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133099794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9000ddce609d3db7e72bd994fa7c9fad87dc906bc1867e053bac204012cf1ea5`
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
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:31 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:31 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:32 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:39 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:39 GMT
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
	-	`sha256:bc99126de627cde0ce0d495e42d48986963f7064f652ba12f98d03421a09cca3`  
		Last Modified: Wed, 26 Apr 2023 21:15:28 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974a36338b571a9f29a9fe51aed3849d56f72ee959075d3474e5197dd162c30`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6d13ee8693152d2b057fbef22807cae24af97dca4ca5c68f168dfe5cea2f2`  
		Last Modified: Wed, 26 Apr 2023 21:15:27 GMT  
		Size: 1.1 MB (1067771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d31c7b477c926c1a10820b77dc20a69c09970ad57815c8879158f891c58656`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jre`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jre` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jre` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jre11`

```console
$ docker pull jruby@sha256:5a9cb573eafa5a20ebd022b33291e61182a4dfa729104820dade9395f6a457f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:b7c2d675f503556571b36c62c1ac12ca7c9d0430be73e8b80e80c26695b2b3a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128546665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb2cba18afaa94ed6d20fd736d51308a6df9a84c047c6ad2b489f50ec8f3f2b`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:26 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:26 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:28 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:28 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:29 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:36 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:37 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:37 GMT
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
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109a326f4fabe4a7280054399df681dda4f0d9dedb8622400684c2a5a319299`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 7.1 MB (7066154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f570e217bb9dafe3ad550b1200be72785af3ba98cf7f5e58e6b7b4ab426945e2`  
		Last Modified: Tue, 18 Apr 2023 05:13:45 GMT  
		Size: 28.9 MB (28854379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641796f37ebfe0a7f67b1c7536d52b9faf6b45a2922cc72532a70361db365785`  
		Last Modified: Tue, 18 Apr 2023 05:13:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2c906851d2a07cb3be8bf4d023217226dfdf8172808d55763062345360ecff`  
		Last Modified: Tue, 18 Apr 2023 05:13:44 GMT  
		Size: 1.1 MB (1067794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9de7a96a0858d78dd5f2daff4bed648aab1e3f2493c18acd31a663c565a4d90`  
		Last Modified: Tue, 18 Apr 2023 05:13:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jre11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:e0c01a3cd7f52c3bf5cccaf4cf59a3ee490af459a529004d643b2d09702db854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124366576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06587625915692f950ff6595c6372daf971405ecb5960b93c4b761ed254dca85`
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
# Wed, 26 Apr 2023 19:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:41:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 21:11:35 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:41 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:41 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:43 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:50 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:50 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:50 GMT
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
	-	`sha256:0990e95b7d7488e9f0e1578de631d0bc2c5564a2e6f12a261dc7df50e8a03258`  
		Last Modified: Wed, 26 Apr 2023 19:47:43 GMT  
		Size: 45.0 MB (45011380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26513c24fc27c615b36ec4e6da60b5792eab52d2e8c6e5264df5fcc48d182186`  
		Last Modified: Wed, 26 Apr 2023 19:47:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777e5da470892748bf6df842c0bc3182882ac494a6eaf1b6ec5b914456fb4fd`  
		Last Modified: Wed, 26 Apr 2023 21:14:27 GMT  
		Size: 6.0 MB (6022740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4519a3199a3d27d9c3a67a08961b31bfa76dca7ae6b7c502d4dae6a29536e926`  
		Last Modified: Wed, 26 Apr 2023 21:15:46 GMT  
		Size: 28.9 MB (28854370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabd5398ccf373daf4a0700dcfb957097c18b4e5816245398740a7cbf5827a8`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f2482f05a43603bbc6dd42072d00b58e6e274f74fde2b4cb1da3f4fcec440`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 1.1 MB (1067778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2699d339fd0ab7eb9594a7ce5c61bd13f96a8f248a1e929261d7391e40f6f30d`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3-jre8`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3-jre8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jdk`

```console
$ docker pull jruby@sha256:d37b51b897e82d483e7a013532dec71c144e1df57c5ad1e5cddb2f9af654d089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:b52e54daad1d0ddf7cc5720bd88da02a84c56f4159c2280588457f6c107ea1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136550087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1758c12db58cf794a075c563243beb970961ac4e2bd8e0a49882eac2ee9667b8`
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
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:14 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:22 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:23 GMT
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
	-	`sha256:13bd82f79d5a1a62a0eeb4bdb8a066d4e1a50668212cba0a444abdb7d3b2456c`  
		Last Modified: Tue, 18 Apr 2023 05:13:26 GMT  
		Size: 28.9 MB (28854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f4dce994ee128038d2145308632a06e9c60334080ef57d63688bfc3e4aad9`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f943e1e3ab27cbe48f31121fc18a7f13f89d99942b99709bfc38a436d7ffa`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 1.1 MB (1067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260efdb780214e7ad07ae619863a47142a5a51a1f804ae3ddb7a74fe9845857`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jdk` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:9b2bc521d74049439075993f655c3ed9a64926f328a82b710f4034dec2b4fec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133099794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9000ddce609d3db7e72bd994fa7c9fad87dc906bc1867e053bac204012cf1ea5`
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
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:31 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:31 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:32 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:39 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:39 GMT
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
	-	`sha256:bc99126de627cde0ce0d495e42d48986963f7064f652ba12f98d03421a09cca3`  
		Last Modified: Wed, 26 Apr 2023 21:15:28 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974a36338b571a9f29a9fe51aed3849d56f72ee959075d3474e5197dd162c30`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6d13ee8693152d2b057fbef22807cae24af97dca4ca5c68f168dfe5cea2f2`  
		Last Modified: Wed, 26 Apr 2023 21:15:27 GMT  
		Size: 1.1 MB (1067771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d31c7b477c926c1a10820b77dc20a69c09970ad57815c8879158f891c58656`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jdk11`

```console
$ docker pull jruby@sha256:610d3d7c88af591d4be546b68cdb132683223f1e9410e4df20b5f19814a04649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:3c200e1d084efdec62333fa0d84941fd8fb7c34b1987a0f4492ef58582ad1787
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280402518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1499dcbdf4747d1141d6ee7f6737be663911d3469b359bd82de6f69ee6ecaaa`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:04 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:24 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:40 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:40 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:42 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:42 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:50 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:50 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:51 GMT
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
	-	`sha256:92c807db9f3053b04e5e7309b190d1af31a410554295b83b7e42ebd37d795fbc`  
		Last Modified: Tue, 18 Apr 2023 00:47:07 GMT  
		Size: 198.5 MB (198488083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff7975ce69e8bb8b5432bab0d34d5de1e7798930490c9cc19d7121bdda9227`  
		Last Modified: Tue, 18 Apr 2023 00:46:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e486a90411bbeb5de2cdc83a866e2e92d3bacee895c402a91b84da503ecd6d1`  
		Last Modified: Tue, 18 Apr 2023 05:12:37 GMT  
		Size: 7.1 MB (7066139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce41fe69752bcd928957b8afc524331c882bd25803f285bc08751f64a69a64f`  
		Last Modified: Tue, 18 Apr 2023 05:13:58 GMT  
		Size: 28.9 MB (28854366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b25beafeb0cfed6e0439a393fb20af81ddc2b3862af8a62eff8a6522b81869`  
		Last Modified: Tue, 18 Apr 2023 05:13:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590c2f785f0e870999aff11d043e5bf4e7421e4c6eb3b12f6462b653ff1f0040`  
		Last Modified: Tue, 18 Apr 2023 05:13:56 GMT  
		Size: 1.1 MB (1067780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888704e582e054cf552e370fdd99db00d15b0c8c7ab8c19e100170a74ca3ffe2`  
		Last Modified: Tue, 18 Apr 2023 05:13:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jdk11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:8c88db1cb100623c1a8eeabb396bda194a4d95cc8f206bca313ee74cc1d627d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274685130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008a89533d32fcb9238b7234e26039d419a117312fb02bfeaeb20b8d08b5bf68`
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
# Wed, 26 Apr 2023 19:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:40:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0c7763a19b4af4ef5fbae831781b5184e988d6f131d264482399eeaf51b6e254';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='be07af349f0d2e1ffb7e01e1e8bac8bffd76e22f6cc1354e5b627222e3395f41';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1e3704c8e155f8f894953c2a6708a52e6f449bbf5a85450be6fbb2ec76581700';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a21e2c30e48df0b7238691833316c008167cbedd4e2f1e677bcb81638420d273';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f19fb28aea3e28fcc402b73ce72f62b602992d48769502effe81c52ca39a581';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:40:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:40:27 GMT
CMD ["jshell"]
# Wed, 26 Apr 2023 21:11:51 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:52 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:52 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:53 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:54 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:54 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:13:01 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:13:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:01 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:01 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:13:01 GMT
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
	-	`sha256:9999759029cca08e4ce40a4073366c9227d73a0dc73a4189707c47ba63614239`  
		Last Modified: Wed, 26 Apr 2023 19:46:24 GMT  
		Size: 195.3 MB (195329906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381a1f91095e95d49250dc06174f0a706bf1c1cef39bcf630a44291c6bb8d2f1`  
		Last Modified: Wed, 26 Apr 2023 19:46:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4304b09b2e14df7ab5f5399e7322776b41ab45d2212cb31a82143c28553a4345`  
		Last Modified: Wed, 26 Apr 2023 21:14:39 GMT  
		Size: 6.0 MB (6022734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f2384cb1ece4a1412929aeb7a5540ff43a6b9abfdb1532c1f4e9777b9e925`  
		Last Modified: Wed, 26 Apr 2023 21:15:58 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c3298269d59244d91c0a9e953678382b1dff381316322b50eb257a14d58159`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed69875dd90217f307de80246c652f48730bdaa2b0388eed1c6301035190e88`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 1.1 MB (1067766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0e89953f961d10b03b3aab459ae7c1c56c4d3ea757ef3dc082d29d509b2b6`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jdk17`

```console
$ docker pull jruby@sha256:ccdc5ab2c88a9160b3192f2453ac9c206c52ae1af374c9a3217cbc1458994406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:4c3b49c50b62035b5ab25682193f44f6957f290bc1c444ce2833a1bf2b8d8813
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.1 MB (278114916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9039a254bdc7d05e52f3cc54ca135cf438db5d660232bec0f9cba3b920fcc0f8`
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
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:58 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:44 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:54 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:54 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:55 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:56 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:56 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:11:03 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:11:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:11:04 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:11:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:11:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ebc9b7986f0210261b9474e28924822358a3e7811682aa6991dfdc2eed3ae`  
		Last Modified: Tue, 18 Apr 2023 00:47:49 GMT  
		Size: 192.4 MB (192448102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd987ac8d27cbef298907f5f282f9e895970ba27e01a15d63ac9131563958a`  
		Last Modified: Tue, 18 Apr 2023 00:47:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419e06a88be997f34d392d377eacd6ff8d1e44759a26af8e6348521015cfa83`  
		Last Modified: Tue, 18 Apr 2023 05:12:49 GMT  
		Size: 7.1 MB (7068634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67056faac3b2fc1bfd244bfb7567cf0ffdc1a813545cfafdcee6022fb652653`  
		Last Modified: Tue, 18 Apr 2023 05:14:10 GMT  
		Size: 28.9 MB (28854412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffafd6c6b82b150e9d28f97c806410d6aca154e70b293cd69e8ceeb03ccd4ee0`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b630b06c183344558b33d52eeddc4ebd5b714775253d35379fcc969c9b5a5`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 1.1 MB (1067791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36eb6c5faab521e347e0e433546d76a0b57945fa7953db9ce5ec4bb7897ece12`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jdk17` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:57fd853e9581896ed0001aa86de2590cd1e1bd0c81479f36510cd9c51ab6e1ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275363024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55207dc90975bb1c92aa41b4f9047076d660e435dc195ccfdf0af050578c090b`
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
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:41:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:44 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:41:44 GMT
CMD ["jshell"]
# Wed, 26 Apr 2023 21:12:07 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:13:03 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:13:03 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:13:05 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:13:05 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:05 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:13:12 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:13:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:12 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:13:13 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cfbead4ab6695e8e5082cf21969d8cddd4af6f02659c98db80315b6bc00b20`  
		Last Modified: Wed, 26 Apr 2023 19:48:47 GMT  
		Size: 191.4 MB (191403797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab5928b774148eca0fea966342b3695c4c7286fc929cff74ef4fca20bf40f1`  
		Last Modified: Wed, 26 Apr 2023 19:48:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4e0550462389ef34286af33d4ef72e8242b1e1f8852252cc044b4d20008fa`  
		Last Modified: Wed, 26 Apr 2023 21:14:51 GMT  
		Size: 6.0 MB (6024913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c964f7e85fa27454c24288bc2b7fa8a12e9fd9fab098cd5a30b10ea6371219c`  
		Last Modified: Wed, 26 Apr 2023 21:16:10 GMT  
		Size: 28.9 MB (28854360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfab3e27262aaae06fa315053c2a2549fdb9fc632aea8dc7a666f016a850577`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba76649e9e0f62efbc916a5f57134dabacceb42348461adb855118bfdbbe531`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 1.1 MB (1067782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506eaf359b5d3dcb4af226b3219e002d347c5870221297a1c956e55e0472b74`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jdk8`

```console
$ docker pull jruby@sha256:d37b51b897e82d483e7a013532dec71c144e1df57c5ad1e5cddb2f9af654d089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:b52e54daad1d0ddf7cc5720bd88da02a84c56f4159c2280588457f6c107ea1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136550087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1758c12db58cf794a075c563243beb970961ac4e2bd8e0a49882eac2ee9667b8`
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
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:14 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:22 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:23 GMT
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
	-	`sha256:13bd82f79d5a1a62a0eeb4bdb8a066d4e1a50668212cba0a444abdb7d3b2456c`  
		Last Modified: Tue, 18 Apr 2023 05:13:26 GMT  
		Size: 28.9 MB (28854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f4dce994ee128038d2145308632a06e9c60334080ef57d63688bfc3e4aad9`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f943e1e3ab27cbe48f31121fc18a7f13f89d99942b99709bfc38a436d7ffa`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 1.1 MB (1067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260efdb780214e7ad07ae619863a47142a5a51a1f804ae3ddb7a74fe9845857`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:9b2bc521d74049439075993f655c3ed9a64926f328a82b710f4034dec2b4fec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133099794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9000ddce609d3db7e72bd994fa7c9fad87dc906bc1867e053bac204012cf1ea5`
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
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:31 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:31 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:32 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:39 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:39 GMT
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
	-	`sha256:bc99126de627cde0ce0d495e42d48986963f7064f652ba12f98d03421a09cca3`  
		Last Modified: Wed, 26 Apr 2023 21:15:28 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974a36338b571a9f29a9fe51aed3849d56f72ee959075d3474e5197dd162c30`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6d13ee8693152d2b057fbef22807cae24af97dca4ca5c68f168dfe5cea2f2`  
		Last Modified: Wed, 26 Apr 2023 21:15:27 GMT  
		Size: 1.1 MB (1067771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d31c7b477c926c1a10820b77dc20a69c09970ad57815c8879158f891c58656`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jre`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jre` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jre` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jre11`

```console
$ docker pull jruby@sha256:5a9cb573eafa5a20ebd022b33291e61182a4dfa729104820dade9395f6a457f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:b7c2d675f503556571b36c62c1ac12ca7c9d0430be73e8b80e80c26695b2b3a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128546665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb2cba18afaa94ed6d20fd736d51308a6df9a84c047c6ad2b489f50ec8f3f2b`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:26 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:26 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:28 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:28 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:29 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:36 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:37 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:37 GMT
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
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109a326f4fabe4a7280054399df681dda4f0d9dedb8622400684c2a5a319299`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 7.1 MB (7066154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f570e217bb9dafe3ad550b1200be72785af3ba98cf7f5e58e6b7b4ab426945e2`  
		Last Modified: Tue, 18 Apr 2023 05:13:45 GMT  
		Size: 28.9 MB (28854379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641796f37ebfe0a7f67b1c7536d52b9faf6b45a2922cc72532a70361db365785`  
		Last Modified: Tue, 18 Apr 2023 05:13:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2c906851d2a07cb3be8bf4d023217226dfdf8172808d55763062345360ecff`  
		Last Modified: Tue, 18 Apr 2023 05:13:44 GMT  
		Size: 1.1 MB (1067794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9de7a96a0858d78dd5f2daff4bed648aab1e3f2493c18acd31a663c565a4d90`  
		Last Modified: Tue, 18 Apr 2023 05:13:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jre11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:e0c01a3cd7f52c3bf5cccaf4cf59a3ee490af459a529004d643b2d09702db854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124366576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06587625915692f950ff6595c6372daf971405ecb5960b93c4b761ed254dca85`
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
# Wed, 26 Apr 2023 19:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:41:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 21:11:35 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:41 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:41 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:43 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:50 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:50 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:50 GMT
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
	-	`sha256:0990e95b7d7488e9f0e1578de631d0bc2c5564a2e6f12a261dc7df50e8a03258`  
		Last Modified: Wed, 26 Apr 2023 19:47:43 GMT  
		Size: 45.0 MB (45011380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26513c24fc27c615b36ec4e6da60b5792eab52d2e8c6e5264df5fcc48d182186`  
		Last Modified: Wed, 26 Apr 2023 19:47:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777e5da470892748bf6df842c0bc3182882ac494a6eaf1b6ec5b914456fb4fd`  
		Last Modified: Wed, 26 Apr 2023 21:14:27 GMT  
		Size: 6.0 MB (6022740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4519a3199a3d27d9c3a67a08961b31bfa76dca7ae6b7c502d4dae6a29536e926`  
		Last Modified: Wed, 26 Apr 2023 21:15:46 GMT  
		Size: 28.9 MB (28854370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabd5398ccf373daf4a0700dcfb957097c18b4e5816245398740a7cbf5827a8`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f2482f05a43603bbc6dd42072d00b58e6e274f74fde2b4cb1da3f4fcec440`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 1.1 MB (1067778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2699d339fd0ab7eb9594a7ce5c61bd13f96a8f248a1e929261d7391e40f6f30d`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10-jre8`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10-jre8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jdk`

```console
$ docker pull jruby@sha256:d37b51b897e82d483e7a013532dec71c144e1df57c5ad1e5cddb2f9af654d089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jdk` - linux; amd64

```console
$ docker pull jruby@sha256:b52e54daad1d0ddf7cc5720bd88da02a84c56f4159c2280588457f6c107ea1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136550087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1758c12db58cf794a075c563243beb970961ac4e2bd8e0a49882eac2ee9667b8`
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
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:14 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:22 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:23 GMT
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
	-	`sha256:13bd82f79d5a1a62a0eeb4bdb8a066d4e1a50668212cba0a444abdb7d3b2456c`  
		Last Modified: Tue, 18 Apr 2023 05:13:26 GMT  
		Size: 28.9 MB (28854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f4dce994ee128038d2145308632a06e9c60334080ef57d63688bfc3e4aad9`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f943e1e3ab27cbe48f31121fc18a7f13f89d99942b99709bfc38a436d7ffa`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 1.1 MB (1067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260efdb780214e7ad07ae619863a47142a5a51a1f804ae3ddb7a74fe9845857`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jdk` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:9b2bc521d74049439075993f655c3ed9a64926f328a82b710f4034dec2b4fec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133099794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9000ddce609d3db7e72bd994fa7c9fad87dc906bc1867e053bac204012cf1ea5`
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
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:31 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:31 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:32 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:39 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:39 GMT
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
	-	`sha256:bc99126de627cde0ce0d495e42d48986963f7064f652ba12f98d03421a09cca3`  
		Last Modified: Wed, 26 Apr 2023 21:15:28 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974a36338b571a9f29a9fe51aed3849d56f72ee959075d3474e5197dd162c30`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6d13ee8693152d2b057fbef22807cae24af97dca4ca5c68f168dfe5cea2f2`  
		Last Modified: Wed, 26 Apr 2023 21:15:27 GMT  
		Size: 1.1 MB (1067771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d31c7b477c926c1a10820b77dc20a69c09970ad57815c8879158f891c58656`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jdk11`

```console
$ docker pull jruby@sha256:610d3d7c88af591d4be546b68cdb132683223f1e9410e4df20b5f19814a04649
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:3c200e1d084efdec62333fa0d84941fd8fb7c34b1987a0f4492ef58582ad1787
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.4 MB (280402518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1499dcbdf4747d1141d6ee7f6737be663911d3469b359bd82de6f69ee6ecaaa`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:04 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:24 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:40 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:40 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:42 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:42 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:50 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:50 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:51 GMT
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
	-	`sha256:92c807db9f3053b04e5e7309b190d1af31a410554295b83b7e42ebd37d795fbc`  
		Last Modified: Tue, 18 Apr 2023 00:47:07 GMT  
		Size: 198.5 MB (198488083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff7975ce69e8bb8b5432bab0d34d5de1e7798930490c9cc19d7121bdda9227`  
		Last Modified: Tue, 18 Apr 2023 00:46:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e486a90411bbeb5de2cdc83a866e2e92d3bacee895c402a91b84da503ecd6d1`  
		Last Modified: Tue, 18 Apr 2023 05:12:37 GMT  
		Size: 7.1 MB (7066139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce41fe69752bcd928957b8afc524331c882bd25803f285bc08751f64a69a64f`  
		Last Modified: Tue, 18 Apr 2023 05:13:58 GMT  
		Size: 28.9 MB (28854366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b25beafeb0cfed6e0439a393fb20af81ddc2b3862af8a62eff8a6522b81869`  
		Last Modified: Tue, 18 Apr 2023 05:13:55 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590c2f785f0e870999aff11d043e5bf4e7421e4c6eb3b12f6462b653ff1f0040`  
		Last Modified: Tue, 18 Apr 2023 05:13:56 GMT  
		Size: 1.1 MB (1067780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888704e582e054cf552e370fdd99db00d15b0c8c7ab8c19e100170a74ca3ffe2`  
		Last Modified: Tue, 18 Apr 2023 05:13:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jdk11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:8c88db1cb100623c1a8eeabb396bda194a4d95cc8f206bca313ee74cc1d627d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274685130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008a89533d32fcb9238b7234e26039d419a117312fb02bfeaeb20b8d08b5bf68`
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
# Wed, 26 Apr 2023 19:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:40:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0c7763a19b4af4ef5fbae831781b5184e988d6f131d264482399eeaf51b6e254';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='be07af349f0d2e1ffb7e01e1e8bac8bffd76e22f6cc1354e5b627222e3395f41';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1e3704c8e155f8f894953c2a6708a52e6f449bbf5a85450be6fbb2ec76581700';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a21e2c30e48df0b7238691833316c008167cbedd4e2f1e677bcb81638420d273';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5f19fb28aea3e28fcc402b73ce72f62b602992d48769502effe81c52ca39a581';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jdk_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:40:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:40:27 GMT
CMD ["jshell"]
# Wed, 26 Apr 2023 21:11:51 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:52 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:52 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:53 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:54 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:54 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:13:01 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:13:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:01 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:01 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:13:01 GMT
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
	-	`sha256:9999759029cca08e4ce40a4073366c9227d73a0dc73a4189707c47ba63614239`  
		Last Modified: Wed, 26 Apr 2023 19:46:24 GMT  
		Size: 195.3 MB (195329906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381a1f91095e95d49250dc06174f0a706bf1c1cef39bcf630a44291c6bb8d2f1`  
		Last Modified: Wed, 26 Apr 2023 19:46:13 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4304b09b2e14df7ab5f5399e7322776b41ab45d2212cb31a82143c28553a4345`  
		Last Modified: Wed, 26 Apr 2023 21:14:39 GMT  
		Size: 6.0 MB (6022734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f2384cb1ece4a1412929aeb7a5540ff43a6b9abfdb1532c1f4e9777b9e925`  
		Last Modified: Wed, 26 Apr 2023 21:15:58 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c3298269d59244d91c0a9e953678382b1dff381316322b50eb257a14d58159`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed69875dd90217f307de80246c652f48730bdaa2b0388eed1c6301035190e88`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 1.1 MB (1067766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0e89953f961d10b03b3aab459ae7c1c56c4d3ea757ef3dc082d29d509b2b6`  
		Last Modified: Wed, 26 Apr 2023 21:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jdk17`

```console
$ docker pull jruby@sha256:ccdc5ab2c88a9160b3192f2453ac9c206c52ae1af374c9a3217cbc1458994406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:4c3b49c50b62035b5ab25682193f44f6957f290bc1c444ce2833a1bf2b8d8813
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.1 MB (278114916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9039a254bdc7d05e52f3cc54ca135cf438db5d660232bec0f9cba3b920fcc0f8`
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
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:58 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:44 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:54 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:54 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:55 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:56 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:56 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:11:03 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:11:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:11:04 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:11:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:11:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ebc9b7986f0210261b9474e28924822358a3e7811682aa6991dfdc2eed3ae`  
		Last Modified: Tue, 18 Apr 2023 00:47:49 GMT  
		Size: 192.4 MB (192448102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd987ac8d27cbef298907f5f282f9e895970ba27e01a15d63ac9131563958a`  
		Last Modified: Tue, 18 Apr 2023 00:47:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419e06a88be997f34d392d377eacd6ff8d1e44759a26af8e6348521015cfa83`  
		Last Modified: Tue, 18 Apr 2023 05:12:49 GMT  
		Size: 7.1 MB (7068634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67056faac3b2fc1bfd244bfb7567cf0ffdc1a813545cfafdcee6022fb652653`  
		Last Modified: Tue, 18 Apr 2023 05:14:10 GMT  
		Size: 28.9 MB (28854412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffafd6c6b82b150e9d28f97c806410d6aca154e70b293cd69e8ceeb03ccd4ee0`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b630b06c183344558b33d52eeddc4ebd5b714775253d35379fcc969c9b5a5`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 1.1 MB (1067791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36eb6c5faab521e347e0e433546d76a0b57945fa7953db9ce5ec4bb7897ece12`  
		Last Modified: Tue, 18 Apr 2023 05:14:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jdk17` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:57fd853e9581896ed0001aa86de2590cd1e1bd0c81479f36510cd9c51ab6e1ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.4 MB (275363024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55207dc90975bb1c92aa41b4f9047076d660e435dc195ccfdf0af050578c090b`
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
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:41:32 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:41:41 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0084272404b89442871e0a1f112779844090532978ad4d4191b8d03fc6adfade';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='e7a84c3e59704588510d7e6cce1f732f397b54a3b558c521912a18a1b4d0abdc';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8f4366ff1eddb548b1744cd82a1a56ceee60abebbcbad446bfb3ead7ac0f0f85';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='2d75540ae922d0c4162729267a8c741e2414881a468fd2ce4140b4069ba47ca9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='e9458b38e97358850902c2936a1bb5f35f6cffc59da9fcd28c63eab8dbbfbc3b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jdk_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:44 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:41:44 GMT
CMD ["jshell"]
# Wed, 26 Apr 2023 21:12:07 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:13:03 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:13:03 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:13:05 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:13:05 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:05 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:13:12 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:13:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:13:12 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:13:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:13:13 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cfbead4ab6695e8e5082cf21969d8cddd4af6f02659c98db80315b6bc00b20`  
		Last Modified: Wed, 26 Apr 2023 19:48:47 GMT  
		Size: 191.4 MB (191403797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ab5928b774148eca0fea966342b3695c4c7286fc929cff74ef4fca20bf40f1`  
		Last Modified: Wed, 26 Apr 2023 19:48:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4e0550462389ef34286af33d4ef72e8242b1e1f8852252cc044b4d20008fa`  
		Last Modified: Wed, 26 Apr 2023 21:14:51 GMT  
		Size: 6.0 MB (6024913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c964f7e85fa27454c24288bc2b7fa8a12e9fd9fab098cd5a30b10ea6371219c`  
		Last Modified: Wed, 26 Apr 2023 21:16:10 GMT  
		Size: 28.9 MB (28854360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfab3e27262aaae06fa315053c2a2549fdb9fc632aea8dc7a666f016a850577`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba76649e9e0f62efbc916a5f57134dabacceb42348461adb855118bfdbbe531`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 1.1 MB (1067782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506eaf359b5d3dcb4af226b3219e002d347c5870221297a1c956e55e0472b74`  
		Last Modified: Wed, 26 Apr 2023 21:16:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jdk8`

```console
$ docker pull jruby@sha256:d37b51b897e82d483e7a013532dec71c144e1df57c5ad1e5cddb2f9af654d089
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jdk8` - linux; amd64

```console
$ docker pull jruby@sha256:b52e54daad1d0ddf7cc5720bd88da02a84c56f4159c2280588457f6c107ea1b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136550087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1758c12db58cf794a075c563243beb970961ac4e2bd8e0a49882eac2ee9667b8`
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
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:12 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:14 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:14 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:15 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:22 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:23 GMT
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
	-	`sha256:13bd82f79d5a1a62a0eeb4bdb8a066d4e1a50668212cba0a444abdb7d3b2456c`  
		Last Modified: Tue, 18 Apr 2023 05:13:26 GMT  
		Size: 28.9 MB (28854408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8f4dce994ee128038d2145308632a06e9c60334080ef57d63688bfc3e4aad9`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537f943e1e3ab27cbe48f31121fc18a7f13f89d99942b99709bfc38a436d7ffa`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 1.1 MB (1067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2260efdb780214e7ad07ae619863a47142a5a51a1f804ae3ddb7a74fe9845857`  
		Last Modified: Tue, 18 Apr 2023 05:13:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:9b2bc521d74049439075993f655c3ed9a64926f328a82b710f4034dec2b4fec8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133099794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9000ddce609d3db7e72bd994fa7c9fad87dc906bc1867e053bac204012cf1ea5`
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
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:30 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:31 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:31 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:32 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:39 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:39 GMT
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
	-	`sha256:bc99126de627cde0ce0d495e42d48986963f7064f652ba12f98d03421a09cca3`  
		Last Modified: Wed, 26 Apr 2023 21:15:28 GMT  
		Size: 28.9 MB (28854403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974a36338b571a9f29a9fe51aed3849d56f72ee959075d3474e5197dd162c30`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf6d13ee8693152d2b057fbef22807cae24af97dca4ca5c68f168dfe5cea2f2`  
		Last Modified: Wed, 26 Apr 2023 21:15:27 GMT  
		Size: 1.1 MB (1067771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d31c7b477c926c1a10820b77dc20a69c09970ad57815c8879158f891c58656`  
		Last Modified: Wed, 26 Apr 2023 21:15:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jre`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jre` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jre` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jre11`

```console
$ docker pull jruby@sha256:5a9cb573eafa5a20ebd022b33291e61182a4dfa729104820dade9395f6a457f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:b7c2d675f503556571b36c62c1ac12ca7c9d0430be73e8b80e80c26695b2b3a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128546665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb2cba18afaa94ed6d20fd736d51308a6df9a84c047c6ad2b489f50ec8f3f2b`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:10:26 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:10:26 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:28 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:28 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:29 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:36 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:37 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:37 GMT
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
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109a326f4fabe4a7280054399df681dda4f0d9dedb8622400684c2a5a319299`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 7.1 MB (7066154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f570e217bb9dafe3ad550b1200be72785af3ba98cf7f5e58e6b7b4ab426945e2`  
		Last Modified: Tue, 18 Apr 2023 05:13:45 GMT  
		Size: 28.9 MB (28854379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641796f37ebfe0a7f67b1c7536d52b9faf6b45a2922cc72532a70361db365785`  
		Last Modified: Tue, 18 Apr 2023 05:13:43 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2c906851d2a07cb3be8bf4d023217226dfdf8172808d55763062345360ecff`  
		Last Modified: Tue, 18 Apr 2023 05:13:44 GMT  
		Size: 1.1 MB (1067794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9de7a96a0858d78dd5f2daff4bed648aab1e3f2493c18acd31a663c565a4d90`  
		Last Modified: Tue, 18 Apr 2023 05:13:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jre11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:e0c01a3cd7f52c3bf5cccaf4cf59a3ee490af459a529004d643b2d09702db854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124366576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06587625915692f950ff6595c6372daf971405ecb5960b93c4b761ed254dca85`
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
# Wed, 26 Apr 2023 19:40:14 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:41:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 21:11:35 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:41 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:41 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:42 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:43 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:43 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:50 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:50 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:50 GMT
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
	-	`sha256:0990e95b7d7488e9f0e1578de631d0bc2c5564a2e6f12a261dc7df50e8a03258`  
		Last Modified: Wed, 26 Apr 2023 19:47:43 GMT  
		Size: 45.0 MB (45011380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26513c24fc27c615b36ec4e6da60b5792eab52d2e8c6e5264df5fcc48d182186`  
		Last Modified: Wed, 26 Apr 2023 19:47:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777e5da470892748bf6df842c0bc3182882ac494a6eaf1b6ec5b914456fb4fd`  
		Last Modified: Wed, 26 Apr 2023 21:14:27 GMT  
		Size: 6.0 MB (6022740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4519a3199a3d27d9c3a67a08961b31bfa76dca7ae6b7c502d4dae6a29536e926`  
		Last Modified: Wed, 26 Apr 2023 21:15:46 GMT  
		Size: 28.9 MB (28854370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efabd5398ccf373daf4a0700dcfb957097c18b4e5816245398740a7cbf5827a8`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8f2482f05a43603bbc6dd42072d00b58e6e274f74fde2b4cb1da3f4fcec440`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 1.1 MB (1067778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2699d339fd0ab7eb9594a7ce5c61bd13f96a8f248a1e929261d7391e40f6f30d`  
		Last Modified: Wed, 26 Apr 2023 21:15:44 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.3.10.0-jre8`

```console
$ docker pull jruby@sha256:2499bf7158cf45c3bd4df16afaf19509646ea6724c3d33962f054d43372d3827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.3.10.0-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:748daa12b929361e3da2db16262acbeefb15807aa203f31828805893f2d32ef9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.7 MB (123738521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2fcf888b9594c5b3ae28e36f8d03baebf4ae29057885cdda697f1d531737ea`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:58 GMT
ENV JRUBY_VERSION=9.3.10.0
# Tue, 18 Apr 2023 05:09:59 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Tue, 18 Apr 2023 05:10:00 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:10:00 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:01 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:10:08 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:10:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:10:08 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:10:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:10:09 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c9b4a6198565011f354e295f03dd27335712c4c5ddbf2c7d10903b579fc9f`  
		Last Modified: Tue, 18 Apr 2023 05:13:03 GMT  
		Size: 28.9 MB (28854384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822aa40732fbe1241b891fa8d9f6ade7eb3142461949b503d8373dc1c58bec71`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c21cddc4dfe7ac8abe92f672bde241e4e13cbd6a61c8ed69fa541c524c22b8d`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 1.1 MB (1067775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c17716fc4ac347afb683d0038562dbb7066e31929ec07b81f8a3e4c9e0ba46`  
		Last Modified: Tue, 18 Apr 2023 05:13:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.3.10.0-jre8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c9fadc27fdeee82c742b35799507daad3126a476afb8775cc4461c97f6445ed3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120176658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb0416030ebdbf62cb251b2895f2717897e993b7e9df39bbf3b5b6d062be143`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_VERSION=9.3.10.0
# Wed, 26 Apr 2023 21:12:19 GMT
ENV JRUBY_SHA256=c78c127e0aa166f257eeab03c4733ba3d96a445314eff7e5dc1f8154d2b5ae45
# Wed, 26 Apr 2023 21:12:20 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:12:20 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:21 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:12:27 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:12:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:12:28 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:12:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:12:28 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8129fae16a14e1a9ec13070b1613fd03fb8a74b79db9f8bcff3f2ca6d268eb3`  
		Last Modified: Wed, 26 Apr 2023 21:15:05 GMT  
		Size: 28.9 MB (28854399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df412ed8511eee091aeb3f4331368a5f1568f411e36a5b9eee3de297edfee11d`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea556162445553434b6b6b0276660cb9f07c85fc05ff140d8ff7f42061f6d6b`  
		Last Modified: Wed, 26 Apr 2023 21:15:04 GMT  
		Size: 1.1 MB (1067804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49327c48b937283f82c84427c4895aab43f366683ddad93d0b3a23d05e6ce051`  
		Last Modified: Wed, 26 Apr 2023 21:15:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4`

```console
$ docker pull jruby@sha256:288d1353a7229e3537dcba4c672a34eacf678a1a405592d954ca269a4ad17e6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:fe1aac15d7410d1f0dc0d7ea856479440e5a9a08e2aff02290fae1780145af96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120882188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0877ed827fb1d899bfd76301e4d720f034ee125572f8da6ebf12e62cda34548`
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
# Wed, 26 Apr 2023 19:39:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 26 Apr 2023 19:39:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 26 Apr 2023 21:11:02 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:11:02 GMT
ENV JRUBY_VERSION=9.4.2.0
# Wed, 26 Apr 2023 21:11:02 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Wed, 26 Apr 2023 21:11:04 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Wed, 26 Apr 2023 21:11:04 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:11:05 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Wed, 26 Apr 2023 21:11:12 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Wed, 26 Apr 2023 21:11:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Apr 2023 21:11:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Apr 2023 21:11:12 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:11:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Apr 2023 21:11:13 GMT
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
	-	`sha256:39e513f8f881a0cc7a3cac24b4a0cd510fb03659886e8579a7f00a50eaef0b6d`  
		Last Modified: Wed, 26 Apr 2023 19:45:28 GMT  
		Size: 40.8 MB (40821399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53254470097a46feb44d8d38699f6a2fa13cf3da75e4cfe7059fad4d5f76773`  
		Last Modified: Wed, 26 Apr 2023 19:45:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043bcdc346efe9e3d1f18343d5315aa4420208a08eaf61546cff41eac6bd4b2e`  
		Last Modified: Wed, 26 Apr 2023 21:13:39 GMT  
		Size: 6.0 MB (6022750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad973beaf0991dd10896bc11fb3ef197b1f2c0a404e2251624437aebc0eb8939`  
		Last Modified: Wed, 26 Apr 2023 21:13:40 GMT  
		Size: 29.5 MB (29529494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dec0bc3cfe301b453ed82b835871753bfae04a37234fc09f0149922b3192149`  
		Last Modified: Wed, 26 Apr 2023 21:13:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855af765163b2662754c72d3a1a6785ce15ccbb286bf9100f107e48a4926ac26`  
		Last Modified: Wed, 26 Apr 2023 21:13:38 GMT  
		Size: 1.1 MB (1098240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2184f8e01fa068eada5dcf86bf0dee73bdba5c116cb46bb23689732d90eb8286`  
		Last Modified: Wed, 26 Apr 2023 21:13:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4-jdk`

```console
$ docker pull jruby@sha256:1469ded7dbfb152846c8d872576d825fe2d3de1e29c34815911fbcbff11918fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jdk` - linux; amd64

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

### `jruby:9.4-jdk` - linux; arm64 variant v8

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

## `jruby:9.4-jdk11`

```console
$ docker pull jruby@sha256:0184904adf78f1c1f6e66b96a74c08083aa3b5e621472c6d82b80d319408d872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:0d502abb8ef3c71e13fb87b3566f5fee2453759b1daad845a4c20fc8fe8a2c8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281108014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f51efd6f253395ba99b1599bfb34a834ceca3c16c0c38d53136db02fe40b214e`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:04 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:24 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:24 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:24 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:26 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:26 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:27 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:35 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:36 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:36 GMT
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
	-	`sha256:92c807db9f3053b04e5e7309b190d1af31a410554295b83b7e42ebd37d795fbc`  
		Last Modified: Tue, 18 Apr 2023 00:47:07 GMT  
		Size: 198.5 MB (198488083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff7975ce69e8bb8b5432bab0d34d5de1e7798930490c9cc19d7121bdda9227`  
		Last Modified: Tue, 18 Apr 2023 00:46:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e486a90411bbeb5de2cdc83a866e2e92d3bacee895c402a91b84da503ecd6d1`  
		Last Modified: Tue, 18 Apr 2023 05:12:37 GMT  
		Size: 7.1 MB (7066139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586cbc609ca5384d34f9faee0f6cebdf82b9191e83a6790cb5812da99d35f9`  
		Last Modified: Tue, 18 Apr 2023 05:12:38 GMT  
		Size: 29.5 MB (29529441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38083fce0e66808ff07678dba7e1a2f0c9cefa87bfc5f9c8ca9023da2dd95d8a`  
		Last Modified: Tue, 18 Apr 2023 05:12:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c084193dabbcc18ebf0cc5500676ae05d181d3732b25c692a277d68712271a`  
		Last Modified: Tue, 18 Apr 2023 05:12:35 GMT  
		Size: 1.1 MB (1098202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4726e1e20661483fa043d8afd86f4c6eaca955646357437fea0f06436297455`  
		Last Modified: Tue, 18 Apr 2023 05:12:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4-jdk11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:17c78c33aa15e22e5267d9e16b13c3bc1f219f73fe6581bfcac8d2caebb1d1da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275316058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92f651c6af7ba81922bbbab07e1a934674b21b0f305db05761b24320822bc76`
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
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 01:41:43 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 03:14:48 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:48 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:48 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:50 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:50 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:50 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:57 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:57 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:58 GMT
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
	-	`sha256:73bc3d968f2da6a6fe292e47c2c89c7441de812edd76a4ff3427b36273c34e1e`  
		Last Modified: Tue, 18 Apr 2023 01:44:09 GMT  
		Size: 195.2 MB (195247232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fa06f508956a3c52e6ab6c8de1aa5c430e059d9869f1b7bac4bdd55ec9d385`  
		Last Modified: Tue, 18 Apr 2023 01:43:58 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c56105999f385265f58ed429f24ff002c54a933f627b1fdd54141c0836db5f`  
		Last Modified: Tue, 18 Apr 2023 03:17:41 GMT  
		Size: 6.0 MB (6030832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9814a9eacdc7026ca0123660f7984e73e270a66dc53f5569fa8f449631caec22`  
		Last Modified: Tue, 18 Apr 2023 03:17:42 GMT  
		Size: 29.5 MB (29529459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac549d8e656c1f9178905ffe5d890d1752b1935c55c71ebb0967aedbbdaf0c`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481d21b229013161de0195fba897b7c0805a86e9902e175cd556da561a53c2ef`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252ec4a31c209a4dd9dbd1ddc90897d93780310b4564f55d2d3afb32291f1c7f`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4-jdk17`

```console
$ docker pull jruby@sha256:4938d2e1528308a7239eaa26eebe245d306894e05a95fa35804e60cf97b7b1fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:b48a46eae0a24bd392d80998a0f91c2070e3edb2dd7ca2b3d7b7b5a79d7d5394
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.8 MB (278820337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2020c2643b40eeea4f6addf069ae91cf76a452a82643e5d002a41752b4174a40`
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
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:58 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:44 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:44 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:44 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:46 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:46 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:47 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:55 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:55 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:55 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ebc9b7986f0210261b9474e28924822358a3e7811682aa6991dfdc2eed3ae`  
		Last Modified: Tue, 18 Apr 2023 00:47:49 GMT  
		Size: 192.4 MB (192448102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd987ac8d27cbef298907f5f282f9e895970ba27e01a15d63ac9131563958a`  
		Last Modified: Tue, 18 Apr 2023 00:47:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419e06a88be997f34d392d377eacd6ff8d1e44759a26af8e6348521015cfa83`  
		Last Modified: Tue, 18 Apr 2023 05:12:49 GMT  
		Size: 7.1 MB (7068634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef705ef14e7a1e229b3a5570eacd4d03495ba06289b989f059d3a4672e675311`  
		Last Modified: Tue, 18 Apr 2023 05:12:50 GMT  
		Size: 29.5 MB (29529422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d16ec92b8a476e710c531b79f1e1f8ad63aced53f1f76c5f98eb24d5c94417`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e417fd2440cc796efc47cd6567c93335b95ad69fdfaadf4df7c0e878a841a3e`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 1.1 MB (1098203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f89cb8f1bcc34d0d83a28c56181268896c9e64ffb957e33282c8a89539dd5f`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4-jdk17` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:37253098b53560eeb6b88c54ba73ff7e33e1a5ca04564b6e40ac2d1ff18d2692
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.9 MB (275939626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2abe7a0445986f6e1647343735a42d9eaf0c6c1469706ff47824021951086e`
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
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 01:42:31 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 03:15:05 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:15:05 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:15:05 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:15:07 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:15:07 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:15:07 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:15:14 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:15:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:15:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:15:15 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:15:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:15:15 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc3b28649d32ea96d611a7bedb76863b3b800ee2bcd2235adf9fb7300a2f8`  
		Last Modified: Tue, 18 Apr 2023 01:44:46 GMT  
		Size: 191.3 MB (191267093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400034484de605c0d52622a38b90a4fafcd53115f266ffe3d002dc453135c14b`  
		Last Modified: Tue, 18 Apr 2023 01:44:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0518bf339cdf9c7ecf25bd86ac1c8d34922c66bb80b9444811b8b2f2bc155bb`  
		Last Modified: Tue, 18 Apr 2023 03:17:53 GMT  
		Size: 6.0 MB (6032687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d379dfb0979d7dd5c9bf90ecfa8ef42c2d0d47adb3098c95c30b270861f9ee`  
		Last Modified: Tue, 18 Apr 2023 03:17:53 GMT  
		Size: 29.5 MB (29529475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8549c3e3016698b772ffeb10df7eceea56ba8c6bcd99dcdcd51c550e0639f3`  
		Last Modified: Tue, 18 Apr 2023 03:17:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0775450c6c74be44739c5ba526182c73d5c8981e3c654926911f1b9f7ce24035`  
		Last Modified: Tue, 18 Apr 2023 03:17:52 GMT  
		Size: 1.1 MB (1098198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce9c082433ebb40b70642e6f6649aef9f4d7ce100ed3e503e02a48e4ad3034`  
		Last Modified: Tue, 18 Apr 2023 03:17:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4-jdk8`

```console
$ docker pull jruby@sha256:b519152224ca75417c7447244fca57e3209558bf6bbe46c6e90bd8900855b59c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jdk8` - linux; amd64

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

### `jruby:9.4-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:5cf8bcc8593e073fcab0a1214111f6eab500f46cd24a708edadcea6a40d916eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133800690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b5c86414bbd2e81b0347f5f4de65c2217d88471addae46456e44b70e5b0007`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:16 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:16 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:18 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:18 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:19 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:26 GMT
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
	-	`sha256:555e98cd5715a0c03df0b6570efc8e34e5eaf64959b4f25c32600201dd304c75`  
		Last Modified: Tue, 18 Apr 2023 01:43:33 GMT  
		Size: 53.7 MB (53731774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fbc060ab7aea2bac49b1d333c9f16148a551e3c54e6e974af800da8ebded00`  
		Last Modified: Tue, 18 Apr 2023 01:43:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86e1918500d49d0684daaebb68671c814c2dc1602a2215fb3f8c1a90c30a70b`  
		Last Modified: Tue, 18 Apr 2023 03:17:06 GMT  
		Size: 6.0 MB (6030871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8a71c44ec9d8582bcf4eed8c149905ea76685a99fd3c83a0240fa9f1dcc2e3`  
		Last Modified: Tue, 18 Apr 2023 03:17:07 GMT  
		Size: 29.5 MB (29529525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9baf37653df1d43b84ae7ba0e0cbe1adf7706ac8a604a275afaee07e4fcd42`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a532d09bd65e1113c21013e197f12acbb5f0e0a5cfe3a91fa913221cfb74f6`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2d669edfbce042dcb28a426fa45336db48806d2d5623b73ddf6f8f31b03f5`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4-jre`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jre` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4-jre` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4-jre11`

```console
$ docker pull jruby@sha256:2f96df61030f5d5d741dbbf2bf37af248bb8dd97a1fe89cd1c9d059ae08ba024
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:7105ac6d73723e47610b81c3dee1a9bb0f14ca9d9a13e523b6efd43d2a518ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129252180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2efc9b19c25aeb7b5dbab194ca9d90438970d3307017daf168e2a16ecc5918`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:05 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:05 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:06 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:07 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:07 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:16 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:16 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:17 GMT
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
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109a326f4fabe4a7280054399df681dda4f0d9dedb8622400684c2a5a319299`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 7.1 MB (7066154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50f846640c718edf425de6bd612bde9089dcd36c592f901204cc387cbdba360`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 29.5 MB (29529469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c43f16c3a59380af076169d20874389df0bb673e7826cd93fe2f008ca746edf`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aae8efd09fc04eb749bd8b1b0a910e55af24c300355143baa5a890d0bb49a1d`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 1.1 MB (1098218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abd999047f08223d572bff36ecf8dcbab2bebe8bfc90f04c2f5ff2be4ba01a`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4-jre11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:847f6c1717a8602731692caf81da91f2766ed627099f529474a506cd417cd7b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125048285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee5a85fb427b81885dc837811668acac608eb9816f333c6bf73f13090aaf23`
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
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:14:32 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:32 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:32 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:34 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:34 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:34 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:41 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:42 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:42 GMT
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
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886bf5eff32cf1af790d0dc271b18c64579fbe05c0a2a845c478fe6ff1fd84ae`  
		Last Modified: Tue, 18 Apr 2023 03:17:27 GMT  
		Size: 6.0 MB (6030846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1e742173261482f7ae1dcbc0415de78147d5f50e084bf2c7a58fd15acf741`  
		Last Modified: Tue, 18 Apr 2023 03:17:28 GMT  
		Size: 29.5 MB (29529479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b1330611b193e5722056732324feca67913b1fb0e63fb2bda6a010cbd5e05c`  
		Last Modified: Tue, 18 Apr 2023 03:17:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea50f6821eee8593fc43b3e61f85ed25898146c5067f2e3e3c72f82127577a`  
		Last Modified: Tue, 18 Apr 2023 03:17:27 GMT  
		Size: 1.1 MB (1098195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2bd9f6b6e72dc254b9f036f39b77da4e7bc6ef1604270d2048941f2fcd6ab`  
		Last Modified: Tue, 18 Apr 2023 03:17:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4-jre8`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4-jre8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jdk`

```console
$ docker pull jruby@sha256:b519152224ca75417c7447244fca57e3209558bf6bbe46c6e90bd8900855b59c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jdk` - linux; amd64

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

### `jruby:9.4.2-jdk` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:5cf8bcc8593e073fcab0a1214111f6eab500f46cd24a708edadcea6a40d916eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133800690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b5c86414bbd2e81b0347f5f4de65c2217d88471addae46456e44b70e5b0007`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:16 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:16 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:18 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:18 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:19 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:26 GMT
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
	-	`sha256:555e98cd5715a0c03df0b6570efc8e34e5eaf64959b4f25c32600201dd304c75`  
		Last Modified: Tue, 18 Apr 2023 01:43:33 GMT  
		Size: 53.7 MB (53731774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fbc060ab7aea2bac49b1d333c9f16148a551e3c54e6e974af800da8ebded00`  
		Last Modified: Tue, 18 Apr 2023 01:43:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86e1918500d49d0684daaebb68671c814c2dc1602a2215fb3f8c1a90c30a70b`  
		Last Modified: Tue, 18 Apr 2023 03:17:06 GMT  
		Size: 6.0 MB (6030871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8a71c44ec9d8582bcf4eed8c149905ea76685a99fd3c83a0240fa9f1dcc2e3`  
		Last Modified: Tue, 18 Apr 2023 03:17:07 GMT  
		Size: 29.5 MB (29529525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9baf37653df1d43b84ae7ba0e0cbe1adf7706ac8a604a275afaee07e4fcd42`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a532d09bd65e1113c21013e197f12acbb5f0e0a5cfe3a91fa913221cfb74f6`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2d669edfbce042dcb28a426fa45336db48806d2d5623b73ddf6f8f31b03f5`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jdk11`

```console
$ docker pull jruby@sha256:0184904adf78f1c1f6e66b96a74c08083aa3b5e621472c6d82b80d319408d872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:0d502abb8ef3c71e13fb87b3566f5fee2453759b1daad845a4c20fc8fe8a2c8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281108014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f51efd6f253395ba99b1599bfb34a834ceca3c16c0c38d53136db02fe40b214e`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:04 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:24 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:24 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:24 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:26 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:26 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:27 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:35 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:36 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:36 GMT
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
	-	`sha256:92c807db9f3053b04e5e7309b190d1af31a410554295b83b7e42ebd37d795fbc`  
		Last Modified: Tue, 18 Apr 2023 00:47:07 GMT  
		Size: 198.5 MB (198488083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff7975ce69e8bb8b5432bab0d34d5de1e7798930490c9cc19d7121bdda9227`  
		Last Modified: Tue, 18 Apr 2023 00:46:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e486a90411bbeb5de2cdc83a866e2e92d3bacee895c402a91b84da503ecd6d1`  
		Last Modified: Tue, 18 Apr 2023 05:12:37 GMT  
		Size: 7.1 MB (7066139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586cbc609ca5384d34f9faee0f6cebdf82b9191e83a6790cb5812da99d35f9`  
		Last Modified: Tue, 18 Apr 2023 05:12:38 GMT  
		Size: 29.5 MB (29529441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38083fce0e66808ff07678dba7e1a2f0c9cefa87bfc5f9c8ca9023da2dd95d8a`  
		Last Modified: Tue, 18 Apr 2023 05:12:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c084193dabbcc18ebf0cc5500676ae05d181d3732b25c692a277d68712271a`  
		Last Modified: Tue, 18 Apr 2023 05:12:35 GMT  
		Size: 1.1 MB (1098202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4726e1e20661483fa043d8afd86f4c6eaca955646357437fea0f06436297455`  
		Last Modified: Tue, 18 Apr 2023 05:12:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2-jdk11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:17c78c33aa15e22e5267d9e16b13c3bc1f219f73fe6581bfcac8d2caebb1d1da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275316058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92f651c6af7ba81922bbbab07e1a934674b21b0f305db05761b24320822bc76`
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
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 01:41:43 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 03:14:48 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:48 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:48 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:50 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:50 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:50 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:57 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:57 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:58 GMT
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
	-	`sha256:73bc3d968f2da6a6fe292e47c2c89c7441de812edd76a4ff3427b36273c34e1e`  
		Last Modified: Tue, 18 Apr 2023 01:44:09 GMT  
		Size: 195.2 MB (195247232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fa06f508956a3c52e6ab6c8de1aa5c430e059d9869f1b7bac4bdd55ec9d385`  
		Last Modified: Tue, 18 Apr 2023 01:43:58 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c56105999f385265f58ed429f24ff002c54a933f627b1fdd54141c0836db5f`  
		Last Modified: Tue, 18 Apr 2023 03:17:41 GMT  
		Size: 6.0 MB (6030832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9814a9eacdc7026ca0123660f7984e73e270a66dc53f5569fa8f449631caec22`  
		Last Modified: Tue, 18 Apr 2023 03:17:42 GMT  
		Size: 29.5 MB (29529459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac549d8e656c1f9178905ffe5d890d1752b1935c55c71ebb0967aedbbdaf0c`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481d21b229013161de0195fba897b7c0805a86e9902e175cd556da561a53c2ef`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252ec4a31c209a4dd9dbd1ddc90897d93780310b4564f55d2d3afb32291f1c7f`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jdk17`

```console
$ docker pull jruby@sha256:4938d2e1528308a7239eaa26eebe245d306894e05a95fa35804e60cf97b7b1fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:b48a46eae0a24bd392d80998a0f91c2070e3edb2dd7ca2b3d7b7b5a79d7d5394
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.8 MB (278820337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2020c2643b40eeea4f6addf069ae91cf76a452a82643e5d002a41752b4174a40`
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
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:58 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:44 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:44 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:44 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:46 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:46 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:47 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:55 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:55 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:55 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ebc9b7986f0210261b9474e28924822358a3e7811682aa6991dfdc2eed3ae`  
		Last Modified: Tue, 18 Apr 2023 00:47:49 GMT  
		Size: 192.4 MB (192448102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd987ac8d27cbef298907f5f282f9e895970ba27e01a15d63ac9131563958a`  
		Last Modified: Tue, 18 Apr 2023 00:47:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419e06a88be997f34d392d377eacd6ff8d1e44759a26af8e6348521015cfa83`  
		Last Modified: Tue, 18 Apr 2023 05:12:49 GMT  
		Size: 7.1 MB (7068634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef705ef14e7a1e229b3a5570eacd4d03495ba06289b989f059d3a4672e675311`  
		Last Modified: Tue, 18 Apr 2023 05:12:50 GMT  
		Size: 29.5 MB (29529422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d16ec92b8a476e710c531b79f1e1f8ad63aced53f1f76c5f98eb24d5c94417`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e417fd2440cc796efc47cd6567c93335b95ad69fdfaadf4df7c0e878a841a3e`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 1.1 MB (1098203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f89cb8f1bcc34d0d83a28c56181268896c9e64ffb957e33282c8a89539dd5f`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2-jdk17` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:37253098b53560eeb6b88c54ba73ff7e33e1a5ca04564b6e40ac2d1ff18d2692
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.9 MB (275939626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2abe7a0445986f6e1647343735a42d9eaf0c6c1469706ff47824021951086e`
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
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 01:42:31 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 03:15:05 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:15:05 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:15:05 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:15:07 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:15:07 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:15:07 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:15:14 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:15:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:15:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:15:15 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:15:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:15:15 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc3b28649d32ea96d611a7bedb76863b3b800ee2bcd2235adf9fb7300a2f8`  
		Last Modified: Tue, 18 Apr 2023 01:44:46 GMT  
		Size: 191.3 MB (191267093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400034484de605c0d52622a38b90a4fafcd53115f266ffe3d002dc453135c14b`  
		Last Modified: Tue, 18 Apr 2023 01:44:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0518bf339cdf9c7ecf25bd86ac1c8d34922c66bb80b9444811b8b2f2bc155bb`  
		Last Modified: Tue, 18 Apr 2023 03:17:53 GMT  
		Size: 6.0 MB (6032687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d379dfb0979d7dd5c9bf90ecfa8ef42c2d0d47adb3098c95c30b270861f9ee`  
		Last Modified: Tue, 18 Apr 2023 03:17:53 GMT  
		Size: 29.5 MB (29529475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8549c3e3016698b772ffeb10df7eceea56ba8c6bcd99dcdcd51c550e0639f3`  
		Last Modified: Tue, 18 Apr 2023 03:17:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0775450c6c74be44739c5ba526182c73d5c8981e3c654926911f1b9f7ce24035`  
		Last Modified: Tue, 18 Apr 2023 03:17:52 GMT  
		Size: 1.1 MB (1098198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce9c082433ebb40b70642e6f6649aef9f4d7ce100ed3e503e02a48e4ad3034`  
		Last Modified: Tue, 18 Apr 2023 03:17:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jdk8`

```console
$ docker pull jruby@sha256:b519152224ca75417c7447244fca57e3209558bf6bbe46c6e90bd8900855b59c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jdk8` - linux; amd64

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

### `jruby:9.4.2-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:5cf8bcc8593e073fcab0a1214111f6eab500f46cd24a708edadcea6a40d916eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133800690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b5c86414bbd2e81b0347f5f4de65c2217d88471addae46456e44b70e5b0007`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:16 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:16 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:18 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:18 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:19 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:26 GMT
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
	-	`sha256:555e98cd5715a0c03df0b6570efc8e34e5eaf64959b4f25c32600201dd304c75`  
		Last Modified: Tue, 18 Apr 2023 01:43:33 GMT  
		Size: 53.7 MB (53731774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fbc060ab7aea2bac49b1d333c9f16148a551e3c54e6e974af800da8ebded00`  
		Last Modified: Tue, 18 Apr 2023 01:43:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86e1918500d49d0684daaebb68671c814c2dc1602a2215fb3f8c1a90c30a70b`  
		Last Modified: Tue, 18 Apr 2023 03:17:06 GMT  
		Size: 6.0 MB (6030871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8a71c44ec9d8582bcf4eed8c149905ea76685a99fd3c83a0240fa9f1dcc2e3`  
		Last Modified: Tue, 18 Apr 2023 03:17:07 GMT  
		Size: 29.5 MB (29529525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9baf37653df1d43b84ae7ba0e0cbe1adf7706ac8a604a275afaee07e4fcd42`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a532d09bd65e1113c21013e197f12acbb5f0e0a5cfe3a91fa913221cfb74f6`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2d669edfbce042dcb28a426fa45336db48806d2d5623b73ddf6f8f31b03f5`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jre`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jre` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2-jre` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jre11`

```console
$ docker pull jruby@sha256:2f96df61030f5d5d741dbbf2bf37af248bb8dd97a1fe89cd1c9d059ae08ba024
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:7105ac6d73723e47610b81c3dee1a9bb0f14ca9d9a13e523b6efd43d2a518ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129252180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2efc9b19c25aeb7b5dbab194ca9d90438970d3307017daf168e2a16ecc5918`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:05 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:05 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:06 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:07 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:07 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:16 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:16 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:17 GMT
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
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109a326f4fabe4a7280054399df681dda4f0d9dedb8622400684c2a5a319299`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 7.1 MB (7066154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50f846640c718edf425de6bd612bde9089dcd36c592f901204cc387cbdba360`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 29.5 MB (29529469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c43f16c3a59380af076169d20874389df0bb673e7826cd93fe2f008ca746edf`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aae8efd09fc04eb749bd8b1b0a910e55af24c300355143baa5a890d0bb49a1d`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 1.1 MB (1098218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abd999047f08223d572bff36ecf8dcbab2bebe8bfc90f04c2f5ff2be4ba01a`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2-jre11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:847f6c1717a8602731692caf81da91f2766ed627099f529474a506cd417cd7b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125048285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee5a85fb427b81885dc837811668acac608eb9816f333c6bf73f13090aaf23`
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
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:14:32 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:32 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:32 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:34 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:34 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:34 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:41 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:42 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:42 GMT
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
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886bf5eff32cf1af790d0dc271b18c64579fbe05c0a2a845c478fe6ff1fd84ae`  
		Last Modified: Tue, 18 Apr 2023 03:17:27 GMT  
		Size: 6.0 MB (6030846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1e742173261482f7ae1dcbc0415de78147d5f50e084bf2c7a58fd15acf741`  
		Last Modified: Tue, 18 Apr 2023 03:17:28 GMT  
		Size: 29.5 MB (29529479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b1330611b193e5722056732324feca67913b1fb0e63fb2bda6a010cbd5e05c`  
		Last Modified: Tue, 18 Apr 2023 03:17:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea50f6821eee8593fc43b3e61f85ed25898146c5067f2e3e3c72f82127577a`  
		Last Modified: Tue, 18 Apr 2023 03:17:27 GMT  
		Size: 1.1 MB (1098195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2bd9f6b6e72dc254b9f036f39b77da4e7bc6ef1604270d2048941f2fcd6ab`  
		Last Modified: Tue, 18 Apr 2023 03:17:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2-jre8`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2-jre8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2.0` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jdk`

```console
$ docker pull jruby@sha256:b519152224ca75417c7447244fca57e3209558bf6bbe46c6e90bd8900855b59c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jdk` - linux; amd64

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

### `jruby:9.4.2.0-jdk` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:5cf8bcc8593e073fcab0a1214111f6eab500f46cd24a708edadcea6a40d916eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133800690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b5c86414bbd2e81b0347f5f4de65c2217d88471addae46456e44b70e5b0007`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:16 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:16 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:18 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:18 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:19 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:26 GMT
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
	-	`sha256:555e98cd5715a0c03df0b6570efc8e34e5eaf64959b4f25c32600201dd304c75`  
		Last Modified: Tue, 18 Apr 2023 01:43:33 GMT  
		Size: 53.7 MB (53731774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fbc060ab7aea2bac49b1d333c9f16148a551e3c54e6e974af800da8ebded00`  
		Last Modified: Tue, 18 Apr 2023 01:43:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86e1918500d49d0684daaebb68671c814c2dc1602a2215fb3f8c1a90c30a70b`  
		Last Modified: Tue, 18 Apr 2023 03:17:06 GMT  
		Size: 6.0 MB (6030871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8a71c44ec9d8582bcf4eed8c149905ea76685a99fd3c83a0240fa9f1dcc2e3`  
		Last Modified: Tue, 18 Apr 2023 03:17:07 GMT  
		Size: 29.5 MB (29529525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9baf37653df1d43b84ae7ba0e0cbe1adf7706ac8a604a275afaee07e4fcd42`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a532d09bd65e1113c21013e197f12acbb5f0e0a5cfe3a91fa913221cfb74f6`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2d669edfbce042dcb28a426fa45336db48806d2d5623b73ddf6f8f31b03f5`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jdk11`

```console
$ docker pull jruby@sha256:0184904adf78f1c1f6e66b96a74c08083aa3b5e621472c6d82b80d319408d872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jdk11` - linux; amd64

```console
$ docker pull jruby@sha256:0d502abb8ef3c71e13fb87b3566f5fee2453759b1daad845a4c20fc8fe8a2c8b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281108014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f51efd6f253395ba99b1599bfb34a834ceca3c16c0c38d53136db02fe40b214e`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:04 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:24 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:24 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:24 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:26 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:26 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:27 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:35 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:36 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:36 GMT
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
	-	`sha256:92c807db9f3053b04e5e7309b190d1af31a410554295b83b7e42ebd37d795fbc`  
		Last Modified: Tue, 18 Apr 2023 00:47:07 GMT  
		Size: 198.5 MB (198488083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ff7975ce69e8bb8b5432bab0d34d5de1e7798930490c9cc19d7121bdda9227`  
		Last Modified: Tue, 18 Apr 2023 00:46:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e486a90411bbeb5de2cdc83a866e2e92d3bacee895c402a91b84da503ecd6d1`  
		Last Modified: Tue, 18 Apr 2023 05:12:37 GMT  
		Size: 7.1 MB (7066139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3586cbc609ca5384d34f9faee0f6cebdf82b9191e83a6790cb5812da99d35f9`  
		Last Modified: Tue, 18 Apr 2023 05:12:38 GMT  
		Size: 29.5 MB (29529441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38083fce0e66808ff07678dba7e1a2f0c9cefa87bfc5f9c8ca9023da2dd95d8a`  
		Last Modified: Tue, 18 Apr 2023 05:12:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c084193dabbcc18ebf0cc5500676ae05d181d3732b25c692a277d68712271a`  
		Last Modified: Tue, 18 Apr 2023 05:12:35 GMT  
		Size: 1.1 MB (1098202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4726e1e20661483fa043d8afd86f4c6eaca955646357437fea0f06436297455`  
		Last Modified: Tue, 18 Apr 2023 05:12:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2.0-jdk11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:17c78c33aa15e22e5267d9e16b13c3bc1f219f73fe6581bfcac8d2caebb1d1da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275316058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92f651c6af7ba81922bbbab07e1a934674b21b0f305db05761b24320822bc76`
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
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 01:41:43 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 03:14:48 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:48 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:48 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:50 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:50 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:50 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:57 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:57 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:58 GMT
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
	-	`sha256:73bc3d968f2da6a6fe292e47c2c89c7441de812edd76a4ff3427b36273c34e1e`  
		Last Modified: Tue, 18 Apr 2023 01:44:09 GMT  
		Size: 195.2 MB (195247232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fa06f508956a3c52e6ab6c8de1aa5c430e059d9869f1b7bac4bdd55ec9d385`  
		Last Modified: Tue, 18 Apr 2023 01:43:58 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c56105999f385265f58ed429f24ff002c54a933f627b1fdd54141c0836db5f`  
		Last Modified: Tue, 18 Apr 2023 03:17:41 GMT  
		Size: 6.0 MB (6030832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9814a9eacdc7026ca0123660f7984e73e270a66dc53f5569fa8f449631caec22`  
		Last Modified: Tue, 18 Apr 2023 03:17:42 GMT  
		Size: 29.5 MB (29529459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daac549d8e656c1f9178905ffe5d890d1752b1935c55c71ebb0967aedbbdaf0c`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481d21b229013161de0195fba897b7c0805a86e9902e175cd556da561a53c2ef`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252ec4a31c209a4dd9dbd1ddc90897d93780310b4564f55d2d3afb32291f1c7f`  
		Last Modified: Tue, 18 Apr 2023 03:17:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jdk17`

```console
$ docker pull jruby@sha256:4938d2e1528308a7239eaa26eebe245d306894e05a95fa35804e60cf97b7b1fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jdk17` - linux; amd64

```console
$ docker pull jruby@sha256:b48a46eae0a24bd392d80998a0f91c2070e3edb2dd7ca2b3d7b7b5a79d7d5394
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.8 MB (278820337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2020c2643b40eeea4f6addf069ae91cf76a452a82643e5d002a41752b4174a40`
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
# Tue, 18 Apr 2023 00:44:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 00:44:48 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 00:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 00:44:58 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 05:09:44 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:44 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:44 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:46 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:46 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:47 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:55 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:55 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:55 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493027a1bf3e6a19b932ebe3c6dbfe19dc6a4583dfe39282977a57c89b31e87`  
		Last Modified: Tue, 18 Apr 2023 00:47:39 GMT  
		Size: 20.1 MB (20096839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ebc9b7986f0210261b9474e28924822358a3e7811682aa6991dfdc2eed3ae`  
		Last Modified: Tue, 18 Apr 2023 00:47:49 GMT  
		Size: 192.4 MB (192448102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd987ac8d27cbef298907f5f282f9e895970ba27e01a15d63ac9131563958a`  
		Last Modified: Tue, 18 Apr 2023 00:47:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1419e06a88be997f34d392d377eacd6ff8d1e44759a26af8e6348521015cfa83`  
		Last Modified: Tue, 18 Apr 2023 05:12:49 GMT  
		Size: 7.1 MB (7068634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef705ef14e7a1e229b3a5570eacd4d03495ba06289b989f059d3a4672e675311`  
		Last Modified: Tue, 18 Apr 2023 05:12:50 GMT  
		Size: 29.5 MB (29529422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d16ec92b8a476e710c531b79f1e1f8ad63aced53f1f76c5f98eb24d5c94417`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e417fd2440cc796efc47cd6567c93335b95ad69fdfaadf4df7c0e878a841a3e`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 1.1 MB (1098203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f89cb8f1bcc34d0d83a28c56181268896c9e64ffb957e33282c8a89539dd5f`  
		Last Modified: Tue, 18 Apr 2023 05:12:48 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2.0-jdk17` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:37253098b53560eeb6b88c54ba73ff7e33e1a5ca04564b6e40ac2d1ff18d2692
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.9 MB (275939626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2abe7a0445986f6e1647343735a42d9eaf0c6c1469706ff47824021951086e`
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
# Tue, 18 Apr 2023 01:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:42:18 GMT
ENV JAVA_VERSION=jdk-17.0.6+10
# Tue, 18 Apr 2023 01:42:27 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9e0e88bbd9fa662567d0c1e22d469268c68ac078e9e5fe5a7244f56fec71f55f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.6_10.tar.gz';          ;;        armhf|arm)          ESUM='fe4d0c6d5bb8cf7f59f7ff82c0c1fd988bbe5cccf3bc7377dc8ae50740b46c82';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_arm_linux_hotspot_17.0.6_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cb772c3fdf3f9fed56f23a37472acf2b80de20a7113fe09933891c6ef0ecde95';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.6_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='32e53321dd3e724e111e5445fbdcbcefde893e59055cc1f102d20fa3bb62ccc3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.6_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='a0b1b9dd809d51a438f5fa08918f9aca7b2135721097f0858cf29f77a35d4289';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.6%2B10/OpenJDK17U-jdk_x64_linux_hotspot_17.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:42:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 01:42:31 GMT
CMD ["jshell"]
# Tue, 18 Apr 2023 03:15:05 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:15:05 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:15:05 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:15:07 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:15:07 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:15:07 GMT
RUN mkdir -p /opt/jruby/etc        && {                echo 'install: --no-document';                echo 'update: --no-document';        } >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:15:14 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:15:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:15:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:15:15 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:15:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:15:15 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f855dc454f40dbe47d375c509772787d9d27ff505e14349af4f2e3944f28f75`  
		Last Modified: Tue, 18 Apr 2023 01:44:38 GMT  
		Size: 20.8 MB (20815202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618bc3b28649d32ea96d611a7bedb76863b3b800ee2bcd2235adf9fb7300a2f8`  
		Last Modified: Tue, 18 Apr 2023 01:44:46 GMT  
		Size: 191.3 MB (191267093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400034484de605c0d52622a38b90a4fafcd53115f266ffe3d002dc453135c14b`  
		Last Modified: Tue, 18 Apr 2023 01:44:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0518bf339cdf9c7ecf25bd86ac1c8d34922c66bb80b9444811b8b2f2bc155bb`  
		Last Modified: Tue, 18 Apr 2023 03:17:53 GMT  
		Size: 6.0 MB (6032687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d379dfb0979d7dd5c9bf90ecfa8ef42c2d0d47adb3098c95c30b270861f9ee`  
		Last Modified: Tue, 18 Apr 2023 03:17:53 GMT  
		Size: 29.5 MB (29529475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8549c3e3016698b772ffeb10df7eceea56ba8c6bcd99dcdcd51c550e0639f3`  
		Last Modified: Tue, 18 Apr 2023 03:17:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0775450c6c74be44739c5ba526182c73d5c8981e3c654926911f1b9f7ce24035`  
		Last Modified: Tue, 18 Apr 2023 03:17:52 GMT  
		Size: 1.1 MB (1098198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ce9c082433ebb40b70642e6f6649aef9f4d7ce100ed3e503e02a48e4ad3034`  
		Last Modified: Tue, 18 Apr 2023 03:17:51 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jdk8`

```console
$ docker pull jruby@sha256:b519152224ca75417c7447244fca57e3209558bf6bbe46c6e90bd8900855b59c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jdk8` - linux; amd64

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

### `jruby:9.4.2.0-jdk8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:5cf8bcc8593e073fcab0a1214111f6eab500f46cd24a708edadcea6a40d916eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.8 MB (133800690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b5c86414bbd2e81b0347f5f4de65c2217d88471addae46456e44b70e5b0007`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:16 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:16 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:16 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:18 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:18 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:19 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:25 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:26 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:26 GMT
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
	-	`sha256:555e98cd5715a0c03df0b6570efc8e34e5eaf64959b4f25c32600201dd304c75`  
		Last Modified: Tue, 18 Apr 2023 01:43:33 GMT  
		Size: 53.7 MB (53731774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fbc060ab7aea2bac49b1d333c9f16148a551e3c54e6e974af800da8ebded00`  
		Last Modified: Tue, 18 Apr 2023 01:43:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86e1918500d49d0684daaebb68671c814c2dc1602a2215fb3f8c1a90c30a70b`  
		Last Modified: Tue, 18 Apr 2023 03:17:06 GMT  
		Size: 6.0 MB (6030871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8a71c44ec9d8582bcf4eed8c149905ea76685a99fd3c83a0240fa9f1dcc2e3`  
		Last Modified: Tue, 18 Apr 2023 03:17:07 GMT  
		Size: 29.5 MB (29529525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9baf37653df1d43b84ae7ba0e0cbe1adf7706ac8a604a275afaee07e4fcd42`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a532d09bd65e1113c21013e197f12acbb5f0e0a5cfe3a91fa913221cfb74f6`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 1.1 MB (1098215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2d669edfbce042dcb28a426fa45336db48806d2d5623b73ddf6f8f31b03f5`  
		Last Modified: Tue, 18 Apr 2023 03:17:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jre`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jre` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2.0-jre` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jre11`

```console
$ docker pull jruby@sha256:2f96df61030f5d5d741dbbf2bf37af248bb8dd97a1fe89cd1c9d059ae08ba024
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jre11` - linux; amd64

```console
$ docker pull jruby@sha256:7105ac6d73723e47610b81c3dee1a9bb0f14ca9d9a13e523b6efd43d2a518ddd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.3 MB (129252180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2efc9b19c25aeb7b5dbab194ca9d90438970d3307017daf168e2a16ecc5918`
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
# Tue, 18 Apr 2023 00:43:54 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 00:44:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 00:44:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:09:05 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:09:05 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:09:06 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:09:07 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:07 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:09:16 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:09:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:09:16 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:09:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:09:17 GMT
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
	-	`sha256:b5fb5d08d03b0834295af88b5b911dca1240bcbdc3268dbc4c8ce24934ae017e`  
		Last Modified: Tue, 18 Apr 2023 00:47:26 GMT  
		Size: 46.6 MB (46632203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ef4a2443f5b89eae76a92c01bf3a006c986bb4fe658aa46a8dccc0bed2f523`  
		Last Modified: Tue, 18 Apr 2023 00:47:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109a326f4fabe4a7280054399df681dda4f0d9dedb8622400684c2a5a319299`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 7.1 MB (7066154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50f846640c718edf425de6bd612bde9089dcd36c592f901204cc387cbdba360`  
		Last Modified: Tue, 18 Apr 2023 05:12:24 GMT  
		Size: 29.5 MB (29529469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c43f16c3a59380af076169d20874389df0bb673e7826cd93fe2f008ca746edf`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aae8efd09fc04eb749bd8b1b0a910e55af24c300355143baa5a890d0bb49a1d`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 1.1 MB (1098218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abd999047f08223d572bff36ecf8dcbab2bebe8bfc90f04c2f5ff2be4ba01a`  
		Last Modified: Tue, 18 Apr 2023 05:12:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2.0-jre11` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:847f6c1717a8602731692caf81da91f2766ed627099f529474a506cd417cd7b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125048285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ee5a85fb427b81885dc837811668acac608eb9816f333c6bf73f13090aaf23`
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
# Tue, 18 Apr 2023 01:41:31 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 18 Apr 2023 01:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 18 Apr 2023 01:41:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 18 Apr 2023 03:14:32 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:32 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:32 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:34 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:34 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:34 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:41 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:42 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:42 GMT
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
	-	`sha256:5775e69497bdf42d2ad7b39be6112c42f7fb711efa0036c55e9a5ddf8b30c244`  
		Last Modified: Tue, 18 Apr 2023 01:44:26 GMT  
		Size: 45.0 MB (44979459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff94c7a5594b10847f2895eb9f20938960ec3194f7398f5da8e801aff22ab00`  
		Last Modified: Tue, 18 Apr 2023 01:44:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886bf5eff32cf1af790d0dc271b18c64579fbe05c0a2a845c478fe6ff1fd84ae`  
		Last Modified: Tue, 18 Apr 2023 03:17:27 GMT  
		Size: 6.0 MB (6030846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd1e742173261482f7ae1dcbc0415de78147d5f50e084bf2c7a58fd15acf741`  
		Last Modified: Tue, 18 Apr 2023 03:17:28 GMT  
		Size: 29.5 MB (29529479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b1330611b193e5722056732324feca67913b1fb0e63fb2bda6a010cbd5e05c`  
		Last Modified: Tue, 18 Apr 2023 03:17:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ea50f6821eee8593fc43b3e61f85ed25898146c5067f2e3e3c72f82127577a`  
		Last Modified: Tue, 18 Apr 2023 03:17:27 GMT  
		Size: 1.1 MB (1098195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2bd9f6b6e72dc254b9f036f39b77da4e7bc6ef1604270d2048941f2fcd6ab`  
		Last Modified: Tue, 18 Apr 2023 03:17:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:9.4.2.0-jre8`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:9.4.2.0-jre8` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:9.4.2.0-jre8` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jruby:latest`

```console
$ docker pull jruby@sha256:aaf504b5ed327ad08762bf46848566121a0b5e1caed3f1347e390634c812474a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jruby:latest` - linux; amd64

```console
$ docker pull jruby@sha256:bc438ad496ee8576a5ebd8e6b7e07a876db0d6cb68f91292f7e10d8b852df319
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124443948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b52d9dd28c9167635d852ab353452aac1b616eeaeac6a60eca5c8081a0edac`
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
# Tue, 18 Apr 2023 00:43:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 00:43:44 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 05:08:23 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 05:08:23 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 05:08:25 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 05:08:25 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:26 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 05:08:33 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 05:08:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 05:08:34 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 05:08:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 05:08:34 GMT
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
	-	`sha256:6ff10a83ab17ee8fa2430a8c0e54770df3f0fcbca12814cf20abe44407e7aac8`  
		Last Modified: Tue, 18 Apr 2023 00:46:44 GMT  
		Size: 41.8 MB (41824180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b5353de6a9b9e23cda740ab29ba1ab74b7c7bf65d0781380a232891e90df`  
		Last Modified: Tue, 18 Apr 2023 00:46:39 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca6f1562e51eb82fab0435687da5697e7fccde8bf09c88a9714090596c6fd0f`  
		Last Modified: Tue, 18 Apr 2023 05:11:33 GMT  
		Size: 7.1 MB (7066046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7abcfa0eee67ea24871e19d71ba9fce3e4a946d4107e6f76a29edba3b795b5`  
		Last Modified: Tue, 18 Apr 2023 05:11:34 GMT  
		Size: 29.5 MB (29529361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3181ae2b08cef4d5a29e8006e982ac13833309b819245ea1db6eb39c68293`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53662dd946f49cbbdfca3c74e93d5754f98648186285b14d5d9d3dd853d988`  
		Last Modified: Tue, 18 Apr 2023 05:11:32 GMT  
		Size: 1.1 MB (1098224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0bac7c5df23c04665a81b2f672976cf4dbee503da77747d6abc397051bc429`  
		Last Modified: Tue, 18 Apr 2023 05:11:31 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jruby:latest` - linux; arm64 variant v8

```console
$ docker pull jruby@sha256:c37fc585230a0a0f8b246d2148b44c3ba45930b5d1b5a1c4565e9000623df448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120877733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4d4e1ced4eda72acc8f6fba6c61f326e2737f334f601267c3b405a8726ea639`
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
# Tue, 18 Apr 2023 01:41:09 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 18 Apr 2023 01:41:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 18 Apr 2023 01:41:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 18 Apr 2023 03:14:00 GMT
RUN apt-get update && apt-get install -y libc6-dev make --no-install-recommends && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_VERSION=9.4.2.0
# Tue, 18 Apr 2023 03:14:00 GMT
ENV JRUBY_SHA256=c2b065c5546d398343f86ddea68892bb4a4b4345e6c8875e964a97377733c3f1
# Tue, 18 Apr 2023 03:14:02 GMT
RUN mkdir /opt/jruby   && curl -fSL https://repo1.maven.org/maven2/org/jruby/jruby-dist/${JRUBY_VERSION}/jruby-dist-${JRUBY_VERSION}-bin.tar.gz -o /tmp/jruby.tar.gz   && echo "$JRUBY_SHA256 /tmp/jruby.tar.gz" | sha256sum -c -   && tar -zx --strip-components=1 -f /tmp/jruby.tar.gz -C /opt/jruby   && rm /tmp/jruby.tar.gz   && update-alternatives --install /usr/local/bin/ruby ruby /opt/jruby/bin/jruby 1
# Tue, 18 Apr 2023 03:14:02 GMT
ENV PATH=/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:03 GMT
RUN mkdir -p /opt/jruby/etc 	&& { 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /opt/jruby/etc/gemrc
# Tue, 18 Apr 2023 03:14:10 GMT
RUN gem install bundler rake net-telnet xmlrpc
# Tue, 18 Apr 2023 03:14:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 18 Apr 2023 03:14:10 GMT
ENV PATH=/usr/local/bundle/bin:/opt/jruby/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 03:14:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 18 Apr 2023 03:14:11 GMT
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
	-	`sha256:11c9a641299c233d12b31ad8fa08ca122c83cb9bd516c9555463b8adfefe6b48`  
		Last Modified: Tue, 18 Apr 2023 01:43:48 GMT  
		Size: 40.8 MB (40808798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27c8ad0a15fa9f0227db3651996ee8fbcde12d045fac190cc6b78c29ae41f72`  
		Last Modified: Tue, 18 Apr 2023 01:43:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71559509a8e0d18787db68f44747ba4e3cfe8e2f8afeab633588fd5781fec1b`  
		Last Modified: Tue, 18 Apr 2023 03:16:39 GMT  
		Size: 6.0 MB (6030880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e183a65a503c4a438e262b09ed43641df3fb31f56ec85f1cfe61c19ff2ffa11a`  
		Last Modified: Tue, 18 Apr 2023 03:16:40 GMT  
		Size: 29.5 MB (29529537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74b54dbc3be42966ce6b687e18a102a6ab7d0cb5c9af77e46919cd95945bc03`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e351f221e3e199e1764f7fd6e61ca7da49d6e3039aa767efba1bce1ad4788337`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 1.1 MB (1098213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b8dc62fe6b9e2244b2485af612528934870c20ca1640e05311ed8600778844`  
		Last Modified: Tue, 18 Apr 2023 03:16:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
