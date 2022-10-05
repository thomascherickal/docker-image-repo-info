## `eclipse-temurin:8u345-b01-jdk-jammy`

```console
$ docker pull eclipse-temurin@sha256:2eb8ce595716f1e301784cbbe31b81ac857d8221b6e9da3f2b504d0d74043d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `eclipse-temurin:8u345-b01-jdk-jammy` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:a037215c8fac519595a5e67c20ba06f4093ebbfcb98ba137e1065084f30f8556
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.4 MB (146387258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b733286d61550ff4a31c2bceaa557ec9e6a7134af3edd4767ea5f854512a8b8`
-	Default Command: `["bash"]`

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
# Wed, 05 Oct 2022 17:00:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:00:38 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 05 Oct 2022 17:00:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 05 Oct 2022 17:00:44 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7f172af2471a1945e9feb3dab4254026b8c38f20c75ae781436a4495e6db`  
		Last Modified: Wed, 05 Oct 2022 17:07:10 GMT  
		Size: 12.4 MB (12442343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bb7e3e8c3e2df0794920ee96f32424648dea897d3c64b9af15ced4c94978ea`  
		Last Modified: Wed, 05 Oct 2022 17:07:17 GMT  
		Size: 103.5 MB (103515827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4644ab39eedf31f62aa81b7ec8b08413c9119d45150c12784fc23a22694960`  
		Last Modified: Wed, 05 Oct 2022 17:07:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u345-b01-jdk-jammy` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:b9df040a1adba2a3789597c3dfffde15fbac074080885662c88a6b2f72c97035
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138210105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111d722b851d987b23c1155792f6cb24b66826e0235b7578460b374401d10d11`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 06:08:32 GMT
ADD file:8b109e7521f26505639a07128de43f93636fcc05ecf26c6358f893f22df38acd in / 
# Fri, 02 Sep 2022 06:08:32 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 09:45:27 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Sep 2022 09:45:27 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 09:45:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 09:45:44 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 09:45:44 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Fri, 02 Sep 2022 09:45:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 02 Sep 2022 09:45:57 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:af25ea170fdc3ef953710312fcb7b9706eae0149cf05cd81c8281f1c511208bb`  
		Last Modified: Fri, 02 Sep 2022 06:10:34 GMT  
		Size: 27.0 MB (27016783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da9840adb350b2d84237efca40f31798e5e831ff841f7bb7df249d366253709`  
		Last Modified: Fri, 02 Sep 2022 09:53:10 GMT  
		Size: 12.0 MB (12016203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd66001e8e9cf26a14e61eb0990860e5cf66b2ba8ad91feca2cccba5b6c3077`  
		Last Modified: Fri, 02 Sep 2022 09:53:17 GMT  
		Size: 99.2 MB (99176959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25ac25c262aa3543be783c24605aeeab60d366c6b6b573c5aed61717d2507b5`  
		Last Modified: Fri, 02 Sep 2022 09:53:07 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u345-b01-jdk-jammy` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:2c06157c1f86e356ac4938cedeef1842bb80c131e8c556e2606956f5855115e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143395316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d7beb84205b762e4495af2f65131cebb93968c057f4be65582f3c95b22b7c85`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:44:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 15:44:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 15:44:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 15:44:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 15:44:19 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 05 Oct 2022 15:44:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 05 Oct 2022 15:44:26 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02ffb58034794e0992216f802a3c5320c4b6b9cc80080bdd07eb7afa7db54bd`  
		Last Modified: Wed, 05 Oct 2022 15:52:13 GMT  
		Size: 12.4 MB (12397643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f130659f1f5099939cfd713643cde819bb17814b6a28efea72a5b1aade910f1`  
		Last Modified: Wed, 05 Oct 2022 15:52:21 GMT  
		Size: 102.6 MB (102615290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23bd073459caf625b7279b9a79059667527491a38b2cc1679971652c3e1fee7`  
		Last Modified: Wed, 05 Oct 2022 15:52:09 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u345-b01-jdk-jammy` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:d9631992ccda27c2f29f343340dcb876b0a5acdc9aeaa335a51f874eb7260840
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.0 MB (149984854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e2667703442d780f8f6625af97bf6fbfa2dde1ef63b8081423ea649e43b891a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 10:52:24 GMT
ADD file:5f3953a21754ce756642c9ddcf521f2cfe220a5fe988ccec51085bd074fbe46e in / 
# Wed, 05 Oct 2022 10:52:26 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 19:58:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 19:58:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 19:58:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 19:59:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 19:59:19 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Wed, 05 Oct 2022 19:59:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1965fb24dded7d7944e2da36cd902adf3b7b1d327aaa21ea507cff00a5a0090';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_aarch64_linux_hotspot_8u345b01.tar.gz';          ;;        armhf|arm)          ESUM='af4ecd311df32b405142d5756f966418d0200fbf6cb9009c20a44dc691e8da6f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_arm_linux_hotspot_8u345b01.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='f2be72678f6c2ad283453d0e21a6cb03144dda356e4edf79f818d99c37feaf34';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u345b01.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ed6c9db3719895584fb1fd69fc79c29240977675f26631911c5a1dbce07b7d58';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u345-b01/OpenJDK8U-jdk_x64_linux_hotspot_8u345b01.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 05 Oct 2022 19:59:35 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5053ecffedc109608feacf4836ad15e0f7b2f6a411250a41574342de479c4760`  
		Last Modified: Wed, 05 Oct 2022 10:54:49 GMT  
		Size: 35.7 MB (35709341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4f9e13e4031adf0b715a42563ea24351addfc9631c435164aa809dc791f3dd`  
		Last Modified: Wed, 05 Oct 2022 20:10:39 GMT  
		Size: 13.3 MB (13266274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a8a7505519db73f19b057a8e2cb63b4a2fd7c8a4a4f760a7bb06d2af501e31`  
		Last Modified: Wed, 05 Oct 2022 20:10:50 GMT  
		Size: 101.0 MB (101009078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca5235a78016dc6c28c2a10288f471abe5c65b55373f8fe59773d9c032fb27e`  
		Last Modified: Wed, 05 Oct 2022 20:10:35 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
