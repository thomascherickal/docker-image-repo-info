## `tomcat:9-jre8`

```console
$ docker pull tomcat@sha256:f5725bc74c4d5d9c0fdf0bd5bfc750f26a0515c05033aa8020a49ec4aee1bd7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8` - linux; amd64

```console
$ docker pull tomcat@sha256:1a84c774bc7be111fd98f9d3a7d99710cb39fc2cf682006716b5e3b061110e52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97340996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73d169925cab0a25abf7e071dc69b818fcaa63f30013566427444a560af2ad35`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:43:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:43:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:43:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:20:09 GMT
ENV JAVA_VERSION=jdk8u352-b08
# Fri, 04 Nov 2022 23:20:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cce4db7c4311378d8d2a174b2cf680d57b52a4036f37c995b14f936b6fc1141a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u352b08.tar.gz';          ;;        armhf|arm)          ESUM='d5ef8ced672a1b391e7949190b8d24db16290e06f257816d5bd0969aed593852';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_arm_linux_hotspot_8u352b08.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5649672dab65b3519ec16653fb2f154da90a7cd2afc568da03f3bff5c6b30a90';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u352b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='40b6b4c3d8f7332ea479527b530413bf0dbc13cff3c0ed9fcadf1ca053bed106';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_x64_linux_hotspot_8u352b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 04 Nov 2022 23:20:49 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 05 Nov 2022 01:38:09 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:38:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:38:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:38:10 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:38:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:38:10 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:41:25 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:41:25 GMT
ENV TOMCAT_MAJOR=9
# Mon, 05 Dec 2022 22:29:16 GMT
ENV TOMCAT_VERSION=9.0.70
# Mon, 05 Dec 2022 22:29:17 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Mon, 05 Dec 2022 22:29:17 GMT
COPY dir:a6675eba78be68dae20f9abd0540ba020bf6bb111e295d305383807a6ec1b829 in /usr/local/tomcat 
# Mon, 05 Dec 2022 22:29:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 22:29:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 05 Dec 2022 22:29:23 GMT
EXPOSE 8080
# Mon, 05 Dec 2022 22:29:23 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f23febae705afcbe0e1dbd31533557d90db42220fbf7e3d6a2c0732453318f`  
		Last Modified: Fri, 04 Nov 2022 23:26:42 GMT  
		Size: 41.8 MB (41818664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccbf47c061fb68ae0fb6b21e0e050d8ca99437b6abade62732747de2c9fb0d4`  
		Last Modified: Fri, 04 Nov 2022 23:26:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68fcdac94aa3e81bc9e52e4c5e5196823491b18ee9c83512dd6084863622bff`  
		Last Modified: Sat, 05 Nov 2022 01:53:07 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73427cadf82d691e4c012d8516b632697eb7c2928c399eeeccc98bcbeeb91a17`  
		Last Modified: Mon, 05 Dec 2022 22:42:03 GMT  
		Size: 12.2 MB (12204567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b1fb19d61d57091bcd65d1b3161cfb35c69ac7428a6774c9759cf2f03cb07d`  
		Last Modified: Mon, 05 Dec 2022 22:42:02 GMT  
		Size: 452.7 KB (452691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ab8d545900be8b64620696ea186c6a8ec438c4cf99b23538a51ce63e31ffa4`  
		Last Modified: Mon, 05 Dec 2022 22:42:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:652928a11cbfc4215d63f76a90f53e935b22efc8dcc3c8c78b7295ec347cbe37
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91137579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28de5e83924bada71a381f69519677397b2f3df05586bf4b55f1bbf02794fe59`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 17:58:54 GMT
ADD file:3acaa98e676fc52121edd2feea0fc71a60614dbf081f3db61809aab25af42a8c in / 
# Wed, 02 Nov 2022 17:58:54 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:35:35 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:35:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:35:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:35:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:58:15 GMT
ENV JAVA_VERSION=jdk8u352-b08
# Fri, 04 Nov 2022 22:59:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cce4db7c4311378d8d2a174b2cf680d57b52a4036f37c995b14f936b6fc1141a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u352b08.tar.gz';          ;;        armhf|arm)          ESUM='d5ef8ced672a1b391e7949190b8d24db16290e06f257816d5bd0969aed593852';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_arm_linux_hotspot_8u352b08.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5649672dab65b3519ec16653fb2f154da90a7cd2afc568da03f3bff5c6b30a90';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u352b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='40b6b4c3d8f7332ea479527b530413bf0dbc13cff3c0ed9fcadf1ca053bed106';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_x64_linux_hotspot_8u352b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 04 Nov 2022 22:59:08 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 04 Nov 2022 23:33:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:33:40 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:33:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:33:41 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:33:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:33:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:38:06 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:38:06 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 02:59:48 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 02:59:48 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 02:59:49 GMT
COPY dir:60413e7b5e504e425a750b5e0a9317396b39187e63313540e5c14e65f6086630 in /usr/local/tomcat 
# Tue, 15 Nov 2022 02:59:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:59:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 02:59:56 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 02:59:56 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3a947801223d5dd57236bed8663245ffddcbb4700ba3aec7edc7865fd8cd9d7`  
		Last Modified: Wed, 02 Nov 2022 18:00:26 GMT  
		Size: 27.0 MB (27020159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0829db637b9792b59814837768853e2024fa2d0f3ed5e36053294ccab7a0dd6`  
		Last Modified: Wed, 02 Nov 2022 18:45:01 GMT  
		Size: 12.0 MB (12012626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064e271d2360704d4839e1b892ac7121bfd35579980379557f6eb248fceb3346`  
		Last Modified: Fri, 04 Nov 2022 23:05:03 GMT  
		Size: 39.5 MB (39542760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433df5ff31ea4843c8939a0e9745c6af9c11ada0eece853f2912545e4e627b04`  
		Last Modified: Fri, 04 Nov 2022 23:04:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed1d60f5512cafe30e89635a6f203fa90662dd9234e0c02188026f149525f8f`  
		Last Modified: Fri, 04 Nov 2022 23:58:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eed9429410956807a7ed790eb49a6ebc661558f7c0daaa27248d636be0ad98`  
		Last Modified: Tue, 15 Nov 2022 03:21:18 GMT  
		Size: 12.1 MB (12134538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e9a942396cc958b54483b3599a317b5b47af5eebe7f20ff6f7a1e838d5551`  
		Last Modified: Tue, 15 Nov 2022 03:21:16 GMT  
		Size: 427.1 KB (427101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e62fd64c9ccb17d772098f22a8d850e8c8437ae1b2be4a1175b6d7c6dddd38`  
		Last Modified: Tue, 15 Nov 2022 03:21:16 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:6360da10593558a7362e073275df773229100a0800dc001a78f20cadcc531fc8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94250439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4eff3f7f5d2d4aab40689886a3d620345a1fb855517940c788215da35a4ec29`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:44:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 19:44:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 19:44:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:39:49 GMT
ENV JAVA_VERSION=jdk8u352-b08
# Fri, 04 Nov 2022 22:40:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cce4db7c4311378d8d2a174b2cf680d57b52a4036f37c995b14f936b6fc1141a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u352b08.tar.gz';          ;;        armhf|arm)          ESUM='d5ef8ced672a1b391e7949190b8d24db16290e06f257816d5bd0969aed593852';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_arm_linux_hotspot_8u352b08.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5649672dab65b3519ec16653fb2f154da90a7cd2afc568da03f3bff5c6b30a90';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u352b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='40b6b4c3d8f7332ea479527b530413bf0dbc13cff3c0ed9fcadf1ca053bed106';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_x64_linux_hotspot_8u352b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 04 Nov 2022 22:40:23 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Fri, 04 Nov 2022 23:51:43 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:51:43 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:51:43 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:51:44 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:51:44 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:51:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:54:27 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:54:27 GMT
ENV TOMCAT_MAJOR=9
# Mon, 05 Dec 2022 22:55:53 GMT
ENV TOMCAT_VERSION=9.0.70
# Mon, 05 Dec 2022 22:55:53 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Mon, 05 Dec 2022 22:55:54 GMT
COPY dir:8b43a96d2ebfbfbca6757bf9ccbcd7f91aaea6e7166a0e2a81e9cbf033cde0dc in /usr/local/tomcat 
# Mon, 05 Dec 2022 22:55:57 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 05 Dec 2022 22:55:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 05 Dec 2022 22:55:59 GMT
EXPOSE 8080
# Mon, 05 Dec 2022 22:55:59 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd66203f631549955cf8c4f71f60bc148efa34d467138bc7406e9b20cfd155c1`  
		Last Modified: Fri, 04 Nov 2022 22:44:50 GMT  
		Size: 40.8 MB (40807347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14c8761d4b12ec391f3de7086ce2d5554b3a25b4073842d4d4c2b52f617a52d`  
		Last Modified: Fri, 04 Nov 2022 22:44:46 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e28fdabedd020cfc0b3b9e48fcddb3e82d68fc443da502f2598b296aa9a8b0`  
		Last Modified: Sat, 05 Nov 2022 00:05:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fb3781caafb3ac16a75bb900a3d06720390ae39a817bf83022370ab195c744`  
		Last Modified: Mon, 05 Dec 2022 23:08:41 GMT  
		Size: 12.2 MB (12212145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4bd3fe7ad905d05b06ce0a5f736e4a890f5efe09a85778e2b56f6bc457bae6`  
		Last Modified: Mon, 05 Dec 2022 23:08:40 GMT  
		Size: 452.0 KB (452001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e68912c2efdd6d0741bd36ba14e5ac8efcc3664a0332cbb22be310a8097d16`  
		Last Modified: Mon, 05 Dec 2022 23:08:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8` - linux; ppc64le

```console
$ docker pull tomcat@sha256:fa3c312b95124f99d788d9b750048e41f2217c1487a375532f0fe07553212903
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102898959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d445d0c9f62f9add6698c67f0f8231b4c884cad8a90d3581375e039e55119b2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 02 Nov 2022 18:17:30 GMT
ADD file:e50d53011f99a82c70508eaba072b194b6498693db105f1b1e78adb85ea2f07a in / 
# Wed, 02 Nov 2022 18:17:33 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:55:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:55:38 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:55:38 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:56:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:17:18 GMT
ENV JAVA_VERSION=jdk8u352-b08
# Fri, 04 Nov 2022 23:18:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cce4db7c4311378d8d2a174b2cf680d57b52a4036f37c995b14f936b6fc1141a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_aarch64_linux_hotspot_8u352b08.tar.gz';          ;;        armhf|arm)          ESUM='d5ef8ced672a1b391e7949190b8d24db16290e06f257816d5bd0969aed593852';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_arm_linux_hotspot_8u352b08.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5649672dab65b3519ec16653fb2f154da90a7cd2afc568da03f3bff5c6b30a90';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_ppc64le_linux_hotspot_8u352b08.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='40b6b4c3d8f7332ea479527b530413bf0dbc13cff3c0ed9fcadf1ca053bed106';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u352-b08/OpenJDK8U-jre_x64_linux_hotspot_8u352b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 04 Nov 2022 23:18:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 05 Nov 2022 00:18:11 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 00:18:12 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:18:13 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 00:18:13 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 00:18:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 00:18:14 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 00:25:03 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 00:25:04 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:36:08 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:36:09 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:36:10 GMT
COPY dir:a583c46f14aa3dea88134bdaeec5a64bc47601c466ec93ae19aa6e396db237e9 in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:36:18 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:36:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:36:22 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:36:23 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:02f24970cf7d1a154c6565b42f393ba6a0e2c23a067c7571a6004bf88a1de8db`  
		Last Modified: Wed, 02 Nov 2022 18:18:59 GMT  
		Size: 35.7 MB (35707582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03873e196fa2aab86a981e0b5a73ace2c40cf4cd3da88abc4c2a4ce980ef6bc`  
		Last Modified: Wed, 02 Nov 2022 19:03:58 GMT  
		Size: 13.3 MB (13263240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77caf72d771e3770bb4b742ba76794160bc2a415a266012f4b3f48678e33dacd`  
		Last Modified: Fri, 04 Nov 2022 23:26:36 GMT  
		Size: 41.2 MB (41216665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12044dfe27fa028727095dd29c6e5fcda09571dd556c7beb6f09dfac06b7cb1`  
		Last Modified: Fri, 04 Nov 2022 23:26:29 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bc09e3fc9cc34490a7e07ee6774d0a8e5424d487c2fae85eab9f774f19b5eb`  
		Last Modified: Sat, 05 Nov 2022 00:46:30 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee99294739c4bbb5b7421782fc3be0ef2cc05155fc33c296618b1264be7db51`  
		Last Modified: Tue, 15 Nov 2022 03:55:18 GMT  
		Size: 12.2 MB (12227173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84596999243fa6c85c8544d9e456101ff5c4d7b93af53f3bbd303307f02f4d99`  
		Last Modified: Tue, 15 Nov 2022 03:55:16 GMT  
		Size: 483.8 KB (483838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aebf8ed1466d0d65dcf9c89983468927a3bbcaea03f7e85bc218712f35c5616`  
		Last Modified: Tue, 15 Nov 2022 03:55:16 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
