## `clojure:temurin-19-boot-focal`

```console
$ docker pull clojure@sha256:fd9f2c7b8ca8549e82e8902eaeb84269125ce64ce494a258170e8d6161010dd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `clojure:temurin-19-boot-focal` - linux; amd64

```console
$ docker pull clojure@sha256:7b459faaf4746fa15352b6c51414827fb4ac55e0ccc858303441f11227650ae4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.9 MB (308946705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea735c312cae2256ff58a8bc0b04155d9373dfc9a6a106c0cba9f20a34a0f88`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:36:50 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Feb 2023 18:36:50 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Feb 2023 18:36:50 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Feb 2023 18:38:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:39:08 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 01 Feb 2023 18:39:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c4be9aa173cb0deb0d215643d9509c8900e5497290b29eee4bee335fa57984f';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='6a51cb3868b5a3b81848a0d276267230ff3f8639f20ba9ae9ef1d386440bf1fd';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_arm_linux_hotspot_19.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='173d1256dfb9d13d309b5390e6bdf72d143b512201b0868f9d349d5ed3d64072';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f2512f9a8e9847dd5d3557c39b485a8e7a1ef37b601dcbcb748d22e49f44815c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3a3ba7a3f8c3a5999e2c91ea1dca843435a0d1c43737bd2f6822b2f02fc52165';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_linux_hotspot_19.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 01 Feb 2023 18:39:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 01 Feb 2023 18:39:20 GMT
CMD ["jshell"]
# Wed, 01 Feb 2023 23:20:00 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 01 Feb 2023 23:20:00 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 01 Feb 2023 23:20:00 GMT
WORKDIR /tmp
# Wed, 01 Feb 2023 23:20:06 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 01 Feb 2023 23:20:07 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 01 Feb 2023 23:20:07 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 01 Feb 2023 23:20:27 GMT
RUN boot
# Wed, 01 Feb 2023 23:20:27 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 01 Feb 2023 23:20:27 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 01 Feb 2023 23:20:27 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a0b756617433db760e0d40331dc725a2851279db749e1433f987c8e22f5db4`  
		Last Modified: Wed, 01 Feb 2023 18:43:06 GMT  
		Size: 20.1 MB (20090178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880a56649f84467771ca60f236068b78d81cabcf64e9ca765c6114af830ac5ad`  
		Last Modified: Wed, 01 Feb 2023 18:44:04 GMT  
		Size: 201.1 MB (201117720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c539c4ae40bac71aa661705abf163d06e599605ac01a3015869bbdd71179a8`  
		Last Modified: Wed, 01 Feb 2023 18:43:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7ce682eedc35efde4b2f7d074ddc7ac22f8c666eac07a28ea0cc76293a50cd`  
		Last Modified: Wed, 01 Feb 2023 23:27:01 GMT  
		Size: 340.2 KB (340152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0786a0b9848ffa58d35443e3093e5c4e38807cf5b8528eae3f906bc3bc148344`  
		Last Modified: Wed, 01 Feb 2023 23:27:05 GMT  
		Size: 58.8 MB (58820196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb24fa84081b2647e9698ea0506451bcc262196ab4c1be750edecd55470979b`  
		Last Modified: Wed, 01 Feb 2023 23:27:01 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `clojure:temurin-19-boot-focal` - linux; arm64 variant v8

```console
$ docker pull clojure@sha256:099699c9f9992a681fea24358466eff04718742ccaebb2e85bafc227f84b3acf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (307023881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdcf7a2ee4a5d6be4b601e2309dd01d5f1462d6ab1450acc338da5b8473cc341`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["repl"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:21:36 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 01 Feb 2023 18:21:36 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Feb 2023 18:21:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 01 Feb 2023 18:23:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 18:23:51 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 01 Feb 2023 18:24:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1c4be9aa173cb0deb0d215643d9509c8900e5497290b29eee4bee335fa57984f';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_aarch64_linux_hotspot_19.0.2_7.tar.gz';          ;;        armhf|arm)          ESUM='6a51cb3868b5a3b81848a0d276267230ff3f8639f20ba9ae9ef1d386440bf1fd';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_arm_linux_hotspot_19.0.2_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='173d1256dfb9d13d309b5390e6bdf72d143b512201b0868f9d349d5ed3d64072';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_ppc64le_linux_hotspot_19.0.2_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='f2512f9a8e9847dd5d3557c39b485a8e7a1ef37b601dcbcb748d22e49f44815c';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_s390x_linux_hotspot_19.0.2_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3a3ba7a3f8c3a5999e2c91ea1dca843435a0d1c43737bd2f6822b2f02fc52165';          BINARY_URL='https://github.com/adoptium/temurin19-binaries/releases/download/jdk-19.0.2%2B7/OpenJDK19U-jdk_x64_linux_hotspot_19.0.2_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 01 Feb 2023 18:24:12 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 01 Feb 2023 18:24:12 GMT
CMD ["jshell"]
# Wed, 01 Feb 2023 20:20:31 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 01 Feb 2023 20:20:31 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 01 Feb 2023 20:20:31 GMT
WORKDIR /tmp
# Wed, 01 Feb 2023 20:20:34 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 01 Feb 2023 20:20:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 01 Feb 2023 20:20:35 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 01 Feb 2023 20:20:51 GMT
RUN boot
# Wed, 01 Feb 2023 20:20:51 GMT
COPY file:0282db266eb050a3ad3609149efe2188243cb9f95c0b3e48a312ddef6c6bea02 in /usr/local/bin/entrypoint 
# Wed, 01 Feb 2023 20:20:51 GMT
ENTRYPOINT ["entrypoint"]
# Wed, 01 Feb 2023 20:20:52 GMT
CMD ["repl"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084b4fa446fbabac4c2afa5e093ea705545bb3e520bd7d960bfedb45e832e237`  
		Last Modified: Wed, 01 Feb 2023 18:27:25 GMT  
		Size: 20.8 MB (20801306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c6dcd89e7b9c2371e43510521b4a7c12451640f9cefcaabb57592ace89e2b6`  
		Last Modified: Wed, 01 Feb 2023 18:28:20 GMT  
		Size: 199.9 MB (199868037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a6ececa73a8a1a22787dff53391c2d62341ea3f7387c442b209274405d2fda`  
		Last Modified: Wed, 01 Feb 2023 18:28:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0cb60bc1d20fa869e493c38143a36568f28369bc7285a91e385e2831861645`  
		Last Modified: Wed, 01 Feb 2023 20:27:03 GMT  
		Size: 340.0 KB (339990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f389ab41c6b693ba6753c3f2cf8f97daf0ea2a7c550eecb9974f82a5a3376c4`  
		Last Modified: Wed, 01 Feb 2023 20:27:06 GMT  
		Size: 58.8 MB (58820238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4b82157dfc7c064918a20ee65ef2676624582695178dbcf7dc29ad176941f5`  
		Last Modified: Wed, 01 Feb 2023 20:27:02 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
