## `eclipse-temurin:20_36-jre-jammy`

```console
$ docker pull eclipse-temurin@sha256:37f86bdeff1b6d4bcf6deed34d3c679cc3ce817eb2087da08301e94e742c4729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `eclipse-temurin:20_36-jre-jammy` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:e8cdfac813f06e2fa4d56778c7abbd1e7f1f1e77bf62a4f96a075993302f9106
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.1 MB (96097097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df0d0ddb89169cb6b04dff1da73df8b8c697784d43851626498d20ec510bc18`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:55:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 27 Mar 2023 19:40:57 GMT
ENV JAVA_VERSION=jdk-20+36
# Mon, 27 Mar 2023 19:41:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b226140b8efacf21d256203cc8f919549e295cb9bac88b24c15fb8e53a66b545';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_aarch64_linux_hotspot_20_36.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='a1c5a16d5a438ce7da4563cd51ff6778cdf62331c00a3096ab2388a916e076d2';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_ppc64le_linux_hotspot_20_36.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='f41be99b1fd21873b0fa1436bb206119706922e9c4b32298538faf3d1b632a72';          BINARY_URL='https://github.com/adoptium/temurin20-binaries/releases/download/jdk-20%2B36/OpenJDK20U-jre_x64_linux_hotspot_20_36.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 27 Mar 2023 19:41:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40b70fd7935308ad0e072e7e06ec8c3abdc59beae70ca716dcd04e971680865`  
		Last Modified: Thu, 16 Mar 2023 02:00:42 GMT  
		Size: 18.4 MB (18400790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d007df1ba6f500ed2c898111be92f3408cfd4d2a51f8e0008e5b512db03d7aea`  
		Last Modified: Mon, 27 Mar 2023 19:43:40 GMT  
		Size: 49.3 MB (49308594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765217ca892f3c70817b955f6efd377f5d5ad3ddc77ef580d82574aac5dd40b4`  
		Last Modified: Mon, 27 Mar 2023 19:43:34 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
