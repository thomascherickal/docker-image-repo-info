## `tomcat:jre21`

```console
$ docker pull tomcat@sha256:a9e00d29104c5d1ba6ee1d95c78dfeb56bda85bd76a3afec8b6a4182114acae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:jre21` - linux; amd64

```console
$ docker pull tomcat@sha256:667cabf69fc2f5d5de95ac67af3487e10a0e816a2e16abe3c207d0009519e448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.1 MB (114089417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30bb4ef798f7f212ee53075b7dec6b59cc7fc81c6e1eef22d2b15c7b7f63815`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:11:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 05:11:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 05:11:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 05:13:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:09:37 GMT
ENV JAVA_VERSION=jdk-21+35
# Wed, 11 Oct 2023 18:10:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5a36cde2956749aaad502e1df6729072e5483265fce142230516261da9a391db';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21%2B35/OpenJDK21U-jre_aarch64_linux_hotspot_21_35.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='080a53a3f75b94450779199f09c8d91b53637d315f128c58a4f160fb6272502d';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21%2B35/OpenJDK21U-jre_x64_linux_hotspot_21_35.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 11 Oct 2023 18:10:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 18:10:24 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 11 Oct 2023 18:10:24 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 00:15:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 13 Oct 2023 00:15:29 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 00:15:29 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 13 Oct 2023 00:15:29 GMT
WORKDIR /usr/local/tomcat
# Fri, 13 Oct 2023 00:15:29 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 00:15:29 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 00:16:15 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 13 Oct 2023 00:16:15 GMT
ENV TOMCAT_MAJOR=10
# Fri, 13 Oct 2023 00:16:15 GMT
ENV TOMCAT_VERSION=10.1.14
# Fri, 13 Oct 2023 00:16:15 GMT
ENV TOMCAT_SHA512=53b7e8cc001686fe3893e00420b469c2d99f0065ee00d9e77e0f4eebdf41b77e69a2e5f27ce2dae2248116f5a78824144d7724c8dda1442b0796152cf7b09081
# Fri, 13 Oct 2023 00:16:16 GMT
COPY dir:200c955b85a5c7ce69d4babf2eb2f3e43c2c566aa1a208493055b71301c876c4 in /usr/local/tomcat 
# Fri, 13 Oct 2023 00:16:20 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:16:21 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Oct 2023 00:16:21 GMT
EXPOSE 8080
# Fri, 13 Oct 2023 00:16:21 GMT
ENTRYPOINT []
# Fri, 13 Oct 2023 00:16:21 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e560b9ae2a605cbabd174647e334b0807409ab4cdb14e3ffa28655f8e033811`  
		Last Modified: Tue, 03 Oct 2023 05:17:36 GMT  
		Size: 17.5 MB (17455429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c900d789bf3402ba4c8597bcf30dc8620ab68b284858ae4bc5b0babaa6e81d`  
		Last Modified: Wed, 11 Oct 2023 18:14:10 GMT  
		Size: 53.5 MB (53493108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c455336b4589862140134e4186a71e2ab12894a28f83ad62332e3b5118a289`  
		Last Modified: Wed, 11 Oct 2023 18:14:02 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d9da8fdc2ee6d636022255ca61881912af74386763a419f6a24910774e7475`  
		Last Modified: Wed, 11 Oct 2023 18:14:02 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a75aa535429a234e8d41db1fb4d7074ed4b42b969fda91df33dd44891c6c5a1`  
		Last Modified: Fri, 13 Oct 2023 00:42:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36519f0e7d91f1c12c828ca22910d117a13bac4213628dad66c696c1db74859`  
		Last Modified: Fri, 13 Oct 2023 00:43:54 GMT  
		Size: 12.2 MB (12240339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2432e407b490284f42d63e4559cc8ed67e9b9a90f33e08dcb1825b0cc2466f`  
		Last Modified: Fri, 13 Oct 2023 00:43:53 GMT  
		Size: 458.5 KB (458476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9f5be95f05e9872ab13f48c99cb0d93fc49c58dfdeb1b88d4ffa09ce372958`  
		Last Modified: Fri, 13 Oct 2023 00:43:53 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre21` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:a88bac3a5055c33023e51f67d84e576be20d8e07e4e5cec08e9ee2c69aa32c1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.6 MB (112614349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:124639b0e207a2e5f9a548c31c680c3e8e3c22c6f17c3d9cbbb0d258b04ef99c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:06:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:06:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:06:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:08:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 17:34:25 GMT
ENV JAVA_VERSION=jdk-21+35
# Wed, 11 Oct 2023 17:35:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='5a36cde2956749aaad502e1df6729072e5483265fce142230516261da9a391db';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21%2B35/OpenJDK21U-jre_aarch64_linux_hotspot_21_35.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='080a53a3f75b94450779199f09c8d91b53637d315f128c58a4f160fb6272502d';          BINARY_URL='https://github.com/adoptium/temurin21-binaries/releases/download/jdk-21%2B35/OpenJDK21U-jre_x64_linux_hotspot_21_35.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 11 Oct 2023 17:35:09 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 17:35:09 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 11 Oct 2023 17:35:09 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 00:13:30 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 13 Oct 2023 00:13:31 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 00:13:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 13 Oct 2023 00:13:31 GMT
WORKDIR /usr/local/tomcat
# Fri, 13 Oct 2023 00:13:31 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 00:13:31 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 00:14:14 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 13 Oct 2023 00:14:14 GMT
ENV TOMCAT_MAJOR=10
# Fri, 13 Oct 2023 00:14:14 GMT
ENV TOMCAT_VERSION=10.1.14
# Fri, 13 Oct 2023 00:14:14 GMT
ENV TOMCAT_SHA512=53b7e8cc001686fe3893e00420b469c2d99f0065ee00d9e77e0f4eebdf41b77e69a2e5f27ce2dae2248116f5a78824144d7724c8dda1442b0796152cf7b09081
# Fri, 13 Oct 2023 00:14:14 GMT
COPY dir:f9d8b384aa320db9af46b1d6a986b601c51bd3da598032793956eef891cd2927 in /usr/local/tomcat 
# Fri, 13 Oct 2023 00:14:18 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:14:19 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Oct 2023 00:14:19 GMT
EXPOSE 8080
# Fri, 13 Oct 2023 00:14:19 GMT
ENTRYPOINT []
# Fri, 13 Oct 2023 00:14:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba2aefbab3334adfc4bfa89dd448c89bc452ab89a02053172fb42a8e5288ba3`  
		Last Modified: Tue, 03 Oct 2023 06:11:30 GMT  
		Size: 18.9 MB (18859718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546798705de448a653df481d363967420cb067cddd625ca494a4ec09bb809a22`  
		Last Modified: Wed, 11 Oct 2023 17:38:26 GMT  
		Size: 52.7 MB (52661246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765a06fca96497f0df0ae805c00bbff5ad4a8c16eca0d3f2e7531e6604bc6274`  
		Last Modified: Wed, 11 Oct 2023 17:38:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48171ec2aad526a39601e2f1c799d123c094967e066a82925f518a4d78b5571f`  
		Last Modified: Wed, 11 Oct 2023 17:38:20 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15df67f20b4c56d4c8ee4975c0ac852b21313662ad3eb4f93a9ae5e08ea0c291`  
		Last Modified: Fri, 13 Oct 2023 00:37:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5d4c4d2c9bc01b8b69da1123dd478beb90890bd48d0f09b84fddfd05397694`  
		Last Modified: Fri, 13 Oct 2023 00:38:47 GMT  
		Size: 12.2 MB (12241734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07e2ea997b0279c9a17e458924518e01240f635b415a6de9ca52989a7d30a4a`  
		Last Modified: Fri, 13 Oct 2023 00:38:47 GMT  
		Size: 458.4 KB (458385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057f4acfc1bf0e8172e5bef1241b5cc2cb3f5d3345a29f86ba29e1800ec040d6`  
		Last Modified: Fri, 13 Oct 2023 00:38:46 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
