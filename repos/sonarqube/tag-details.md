<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sonarqube`

-	[`sonarqube:7.9.4-community`](#sonarqube794-community)
-	[`sonarqube:7.9-community`](#sonarqube79-community)
-	[`sonarqube:8.4.1-community`](#sonarqube841-community)
-	[`sonarqube:8.4.1-developer`](#sonarqube841-developer)
-	[`sonarqube:8.4.1-enterprise`](#sonarqube841-enterprise)
-	[`sonarqube:8.4-community`](#sonarqube84-community)
-	[`sonarqube:8.4-developer`](#sonarqube84-developer)
-	[`sonarqube:8.4-enterprise`](#sonarqube84-enterprise)
-	[`sonarqube:8-community`](#sonarqube8-community)
-	[`sonarqube:8-developer`](#sonarqube8-developer)
-	[`sonarqube:8-enterprise`](#sonarqube8-enterprise)
-	[`sonarqube:community`](#sonarqubecommunity)
-	[`sonarqube:developer`](#sonarqubedeveloper)
-	[`sonarqube:enterprise`](#sonarqubeenterprise)
-	[`sonarqube:latest`](#sonarqubelatest)
-	[`sonarqube:lts`](#sonarqubelts)

## `sonarqube:7.9.4-community`

**does not exist** (yet?)

## `sonarqube:7.9-community`

```console
$ docker pull sonarqube@sha256:0f6984003b51df517f759fdf23fae7cfdd0eaae473e44ec879e82dd34b81be53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:7.9-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:78fe85076b640618b903b7571dc321ee4ce638adc9dcd6bc0054949397684ef7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.7 MB (286706357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2f4d9abb5582755ed8f9d5e83ad602649982ab0e74d38c8d7db7112aab7462`
-	Entrypoint: `[".\/bin\/run.sh"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:35:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:35:24 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 22:40:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 22 Jul 2020 22:40:32 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 22:40:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 22 Jul 2020 22:40:33 GMT
ENV JAVA_VERSION=11.0.8
# Wed, 22 Jul 2020 22:41:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_
# Wed, 22 Jul 2020 22:41:22 GMT
ENV JAVA_URL_VERSION=11.0.8_10
# Wed, 22 Jul 2020 22:41:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 23 Jul 2020 09:46:03 GMT
RUN apt-get update     && apt-get install -y curl gnupg2 unzip     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 09:46:03 GMT
ENV SONAR_VERSION=7.9.3 SONARQUBE_HOME=/opt/sonarqube SONARQUBE_JDBC_USERNAME=sonar SONARQUBE_JDBC_PASSWORD=sonar SONARQUBE_JDBC_URL=
# Thu, 23 Jul 2020 09:46:04 GMT
EXPOSE 9000
# Thu, 23 Jul 2020 09:46:04 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Thu, 23 Jul 2020 09:46:05 GMT
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done
# Thu, 23 Jul 2020 09:46:19 GMT
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip     && curl -o sonarqube.zip.asc -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip.asc     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv sonarqube-$SONAR_VERSION sonarqube     && chown -R sonarqube:sonarqube sonarqube     && rm sonarqube.zip*     && rm -rf $SONARQUBE_HOME/bin/*
# Thu, 23 Jul 2020 09:46:19 GMT
VOLUME [/opt/sonarqube/data]
# Thu, 23 Jul 2020 09:46:19 GMT
WORKDIR /opt/sonarqube
# Thu, 23 Jul 2020 09:46:19 GMT
COPY file:aa007fcc6be4125cbbb27fe345978294add03a4f05e942a5208a37be832addca in /opt/sonarqube/bin/ 
# Thu, 23 Jul 2020 09:46:20 GMT
USER sonarqube
# Thu, 23 Jul 2020 09:46:20 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa4e9b7780660af457791b3bbbd51d1d25c8d9681c1f7ebe5e3a59e0179cecd`  
		Last Modified: Wed, 22 Jul 2020 22:44:33 GMT  
		Size: 3.2 MB (3248441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b5d3bc409673c9f77720030b623cb2c26bda1203fbcca9734ebfe1c68f18d`  
		Last Modified: Wed, 22 Jul 2020 22:47:26 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63bc6ae26706f2964c7797e192b3141fb5d797712c440d6f07154202c9fd0e`  
		Last Modified: Wed, 22 Jul 2020 22:48:13 GMT  
		Size: 42.2 MB (42225249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c164eb43c04b1a046c75695ade27ae7c130021b79ff52bd0079eef60472ff`  
		Last Modified: Thu, 23 Jul 2020 09:46:43 GMT  
		Size: 6.0 MB (5984842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afa0e94e8006b8aaf322f2551149a49866b820feb9e5e91559e4685dabc6adf`  
		Last Modified: Thu, 23 Jul 2020 09:46:42 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec94ff2322ec5acef43e4252dd1ecbc809ba8fe06065ad282e36f1da090b9ed`  
		Last Modified: Thu, 23 Jul 2020 09:46:42 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fb561aad2c7b8f4b456573ee0e8a6b7af401b72da3e6ecbdec0255bf2ee28`  
		Last Modified: Thu, 23 Jul 2020 09:46:55 GMT  
		Size: 208.1 MB (208144778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264d9a5f0c2259aa5ff374e0bd8b109cfad6513a217a8f025ccbc0b91ee8e444`  
		Last Modified: Thu, 23 Jul 2020 09:46:42 GMT  
		Size: 788.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.4.1-community`

```console
$ docker pull sonarqube@sha256:c8330c1cf1e8cf50f359ecab396cf12bd870ec9e4397e1adfa0991d51932b30d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.4.1-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:b76725666b3c1b9d4eb6f0e65e86b6b59a3abe976b4615913b43c74d6fd4604b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294409861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce76b6b9372a3f9fba5326432778d0a4c81ba18f50a1be3315107a7dab4fd6ec`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:49:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:03 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2106c7b928bf49fbfa0588943a6a0f0b0cf4ae75cde0b8fd14054b76518a08e`  
		Last Modified: Wed, 15 Jul 2020 23:51:35 GMT  
		Size: 242.4 MB (242378410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1166e713d353319f45853bd04aa63eb0dd06164e87b9ee40edb1894cf433226d`  
		Last Modified: Wed, 15 Jul 2020 23:51:19 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.4.1-developer`

```console
$ docker pull sonarqube@sha256:8c241901b661f66a869e264d7e9943bda49979f09c6added8f3ec1a07bbc4117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.4.1-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:747aedf76aa97a15b3dd3bef0e032ce8800de3cdbfa506f8686d06d37613578e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358514146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dadba0c4995de67d93cfd45e22b414ea51f8d64c96917f103a417da30b8615a`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:09 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:31 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:32 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:32 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:32 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:32 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:32 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3321c65a21730ab3292bb5995c743976092b84ee188ce8e70d9759cb7e2e4fc3`  
		Last Modified: Wed, 15 Jul 2020 23:52:00 GMT  
		Size: 306.5 MB (306482695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7830eb92df87d35771f8b8b10e42c83506b60d2eac98f8f0816f02d4c42ace`  
		Last Modified: Wed, 15 Jul 2020 23:51:41 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.4.1-enterprise`

```console
$ docker pull sonarqube@sha256:4d1ddfb2053c3c73532d85be1aec6a834d0312ca99521f27c5924794c576d915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.4.1-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:06328e9ff42fd3df8c13b34180542405e1ebd86501a372822c0c2b6b54796574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.8 MB (380806163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915e14a5fd31883f26e2944d33cf580d45afe90730cba64289ae9f2cd8284e42`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:39 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:51:02 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:51:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:51:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:51:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:51:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:51:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7611f32954ce88c4dee2db375ff78ef2080aa8ebbeafc4be31b9814c4df13b`  
		Last Modified: Wed, 15 Jul 2020 23:52:24 GMT  
		Size: 328.8 MB (328774713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddacb81fd3a0d8f9e81d03021b4a335fe0221588ed22e702bb511a578455a9d1`  
		Last Modified: Wed, 15 Jul 2020 23:52:04 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.4-community`

```console
$ docker pull sonarqube@sha256:c8330c1cf1e8cf50f359ecab396cf12bd870ec9e4397e1adfa0991d51932b30d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.4-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:b76725666b3c1b9d4eb6f0e65e86b6b59a3abe976b4615913b43c74d6fd4604b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294409861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce76b6b9372a3f9fba5326432778d0a4c81ba18f50a1be3315107a7dab4fd6ec`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:49:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:03 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2106c7b928bf49fbfa0588943a6a0f0b0cf4ae75cde0b8fd14054b76518a08e`  
		Last Modified: Wed, 15 Jul 2020 23:51:35 GMT  
		Size: 242.4 MB (242378410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1166e713d353319f45853bd04aa63eb0dd06164e87b9ee40edb1894cf433226d`  
		Last Modified: Wed, 15 Jul 2020 23:51:19 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.4-developer`

```console
$ docker pull sonarqube@sha256:8c241901b661f66a869e264d7e9943bda49979f09c6added8f3ec1a07bbc4117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.4-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:747aedf76aa97a15b3dd3bef0e032ce8800de3cdbfa506f8686d06d37613578e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358514146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dadba0c4995de67d93cfd45e22b414ea51f8d64c96917f103a417da30b8615a`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:09 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:31 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:32 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:32 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:32 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:32 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:32 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3321c65a21730ab3292bb5995c743976092b84ee188ce8e70d9759cb7e2e4fc3`  
		Last Modified: Wed, 15 Jul 2020 23:52:00 GMT  
		Size: 306.5 MB (306482695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7830eb92df87d35771f8b8b10e42c83506b60d2eac98f8f0816f02d4c42ace`  
		Last Modified: Wed, 15 Jul 2020 23:51:41 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8.4-enterprise`

```console
$ docker pull sonarqube@sha256:4d1ddfb2053c3c73532d85be1aec6a834d0312ca99521f27c5924794c576d915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8.4-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:06328e9ff42fd3df8c13b34180542405e1ebd86501a372822c0c2b6b54796574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.8 MB (380806163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915e14a5fd31883f26e2944d33cf580d45afe90730cba64289ae9f2cd8284e42`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:39 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:51:02 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:51:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:51:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:51:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:51:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:51:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7611f32954ce88c4dee2db375ff78ef2080aa8ebbeafc4be31b9814c4df13b`  
		Last Modified: Wed, 15 Jul 2020 23:52:24 GMT  
		Size: 328.8 MB (328774713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddacb81fd3a0d8f9e81d03021b4a335fe0221588ed22e702bb511a578455a9d1`  
		Last Modified: Wed, 15 Jul 2020 23:52:04 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8-community`

```console
$ docker pull sonarqube@sha256:c8330c1cf1e8cf50f359ecab396cf12bd870ec9e4397e1adfa0991d51932b30d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-community` - linux; amd64

```console
$ docker pull sonarqube@sha256:b76725666b3c1b9d4eb6f0e65e86b6b59a3abe976b4615913b43c74d6fd4604b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294409861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce76b6b9372a3f9fba5326432778d0a4c81ba18f50a1be3315107a7dab4fd6ec`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:49:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:03 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2106c7b928bf49fbfa0588943a6a0f0b0cf4ae75cde0b8fd14054b76518a08e`  
		Last Modified: Wed, 15 Jul 2020 23:51:35 GMT  
		Size: 242.4 MB (242378410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1166e713d353319f45853bd04aa63eb0dd06164e87b9ee40edb1894cf433226d`  
		Last Modified: Wed, 15 Jul 2020 23:51:19 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8-developer`

```console
$ docker pull sonarqube@sha256:8c241901b661f66a869e264d7e9943bda49979f09c6added8f3ec1a07bbc4117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:747aedf76aa97a15b3dd3bef0e032ce8800de3cdbfa506f8686d06d37613578e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358514146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dadba0c4995de67d93cfd45e22b414ea51f8d64c96917f103a417da30b8615a`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:09 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:31 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:32 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:32 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:32 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:32 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:32 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3321c65a21730ab3292bb5995c743976092b84ee188ce8e70d9759cb7e2e4fc3`  
		Last Modified: Wed, 15 Jul 2020 23:52:00 GMT  
		Size: 306.5 MB (306482695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7830eb92df87d35771f8b8b10e42c83506b60d2eac98f8f0816f02d4c42ace`  
		Last Modified: Wed, 15 Jul 2020 23:51:41 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:8-enterprise`

```console
$ docker pull sonarqube@sha256:4d1ddfb2053c3c73532d85be1aec6a834d0312ca99521f27c5924794c576d915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:8-enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:06328e9ff42fd3df8c13b34180542405e1ebd86501a372822c0c2b6b54796574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.8 MB (380806163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915e14a5fd31883f26e2944d33cf580d45afe90730cba64289ae9f2cd8284e42`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:39 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:51:02 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:51:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:51:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:51:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:51:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:51:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7611f32954ce88c4dee2db375ff78ef2080aa8ebbeafc4be31b9814c4df13b`  
		Last Modified: Wed, 15 Jul 2020 23:52:24 GMT  
		Size: 328.8 MB (328774713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddacb81fd3a0d8f9e81d03021b4a335fe0221588ed22e702bb511a578455a9d1`  
		Last Modified: Wed, 15 Jul 2020 23:52:04 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:community`

```console
$ docker pull sonarqube@sha256:c8330c1cf1e8cf50f359ecab396cf12bd870ec9e4397e1adfa0991d51932b30d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:community` - linux; amd64

```console
$ docker pull sonarqube@sha256:b76725666b3c1b9d4eb6f0e65e86b6b59a3abe976b4615913b43c74d6fd4604b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294409861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce76b6b9372a3f9fba5326432778d0a4c81ba18f50a1be3315107a7dab4fd6ec`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:49:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:03 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2106c7b928bf49fbfa0588943a6a0f0b0cf4ae75cde0b8fd14054b76518a08e`  
		Last Modified: Wed, 15 Jul 2020 23:51:35 GMT  
		Size: 242.4 MB (242378410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1166e713d353319f45853bd04aa63eb0dd06164e87b9ee40edb1894cf433226d`  
		Last Modified: Wed, 15 Jul 2020 23:51:19 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:developer`

```console
$ docker pull sonarqube@sha256:8c241901b661f66a869e264d7e9943bda49979f09c6added8f3ec1a07bbc4117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:developer` - linux; amd64

```console
$ docker pull sonarqube@sha256:747aedf76aa97a15b3dd3bef0e032ce8800de3cdbfa506f8686d06d37613578e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.5 MB (358514146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dadba0c4995de67d93cfd45e22b414ea51f8d64c96917f103a417da30b8615a`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:09 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:31 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:32 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:32 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:32 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:32 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:32 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3321c65a21730ab3292bb5995c743976092b84ee188ce8e70d9759cb7e2e4fc3`  
		Last Modified: Wed, 15 Jul 2020 23:52:00 GMT  
		Size: 306.5 MB (306482695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7830eb92df87d35771f8b8b10e42c83506b60d2eac98f8f0816f02d4c42ace`  
		Last Modified: Wed, 15 Jul 2020 23:51:41 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:enterprise`

```console
$ docker pull sonarqube@sha256:4d1ddfb2053c3c73532d85be1aec6a834d0312ca99521f27c5924794c576d915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:enterprise` - linux; amd64

```console
$ docker pull sonarqube@sha256:06328e9ff42fd3df8c13b34180542405e1ebd86501a372822c0c2b6b54796574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.8 MB (380806163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915e14a5fd31883f26e2944d33cf580d45afe90730cba64289ae9f2cd8284e42`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:50:39 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:50:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:51:02 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/CommercialDistribution/sonarqube-enterprise/sonarqube-enterprise-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:51:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:51:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:51:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:51:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:51:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7611f32954ce88c4dee2db375ff78ef2080aa8ebbeafc4be31b9814c4df13b`  
		Last Modified: Wed, 15 Jul 2020 23:52:24 GMT  
		Size: 328.8 MB (328774713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddacb81fd3a0d8f9e81d03021b4a335fe0221588ed22e702bb511a578455a9d1`  
		Last Modified: Wed, 15 Jul 2020 23:52:04 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:latest`

```console
$ docker pull sonarqube@sha256:c8330c1cf1e8cf50f359ecab396cf12bd870ec9e4397e1adfa0991d51932b30d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:latest` - linux; amd64

```console
$ docker pull sonarqube@sha256:b76725666b3c1b9d4eb6f0e65e86b6b59a3abe976b4615913b43c74d6fd4604b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.4 MB (294409861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce76b6b9372a3f9fba5326432778d0a4c81ba18f50a1be3315107a7dab4fd6ec`
-	Entrypoint: `["bin\/run.sh"]`
-	Default Command: `["bin\/sonar.sh"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Apr 2020 01:20:11 GMT
ENV JAVA_VERSION=jdk-11.0.6+10 LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 30 Apr 2020 01:20:53 GMT
RUN set -eux;     apk add --no-cache --virtual .build-deps curl binutils;     GLIBC_VER="2.31-r0";     ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download";     GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-9.1.0-2-x86_64.pkg.tar.xz";     GCC_LIBS_SHA256="91dba90f3c20d32fcf7f1dbe91523653018aa0b8d2230b00f822f6722804cf08";     ZLIB_URL="https://archive.archlinux.org/packages/z/zlib/zlib-1%3A1.2.11-3-x86_64.pkg.tar.xz";     ZLIB_SHA256=17aede0b9f8baa789c5aa3f358fbf8c68a5f1228c5e6cba1a5dd34102ef4d4e5;     curl -LfsS https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /etc/apk/keys/sgerrand.rsa.pub;     SGERRAND_RSA_SHA256="823b54589c93b02497f1ba4dc622eaef9c813e6b0f0ebbb2f771e32adf9f4ef2";     echo "${SGERRAND_RSA_SHA256} */etc/apk/keys/sgerrand.rsa.pub" | sha256sum -c -;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/glibc-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-bin-${GLIBC_VER}.apk > /tmp/glibc-bin-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-bin-${GLIBC_VER}.apk;     curl -LfsS ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-i18n-${GLIBC_VER}.apk > /tmp/glibc-i18n-${GLIBC_VER}.apk;     apk add --no-cache /tmp/glibc-i18n-${GLIBC_VER}.apk;     /usr/glibc-compat/bin/localedef --force --inputfile POSIX --charmap UTF-8 "$LANG" || true;     echo "export LANG=$LANG" > /etc/profile.d/locale.sh;     curl -LfsS ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz;     echo "${GCC_LIBS_SHA256} */tmp/gcc-libs.tar.xz" | sha256sum -c -;     mkdir /tmp/gcc;     tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc;     mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib;     strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*;     curl -LfsS ${ZLIB_URL} -o /tmp/libz.tar.xz;     echo "${ZLIB_SHA256} */tmp/libz.tar.xz" | sha256sum -c -;     mkdir /tmp/libz;     tar -xf /tmp/libz.tar.xz -C /tmp/libz;     mv /tmp/libz/usr/lib/libz.so* /usr/glibc-compat/lib;     apk del --purge .build-deps glibc-i18n;     rm -rf /tmp/*.apk /tmp/gcc /tmp/gcc-libs.tar.xz /tmp/libz /tmp/libz.tar.xz /var/cache/apk/*;
# Thu, 30 Apr 2020 01:20:58 GMT
RUN set -eux;     apk add --no-cache --virtual .fetch-deps curl;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        aarch64|arm64)          ESUM='7ed04ed9ed7271528e7f03490f1fd7dfbbc2d391414bd6fe4dd80ec3bad76d30';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='49231f2c36487b53141ade3f7eb291e2855138b14b1129f9acf435ea9cc0e899';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='bcb3f46cbad742b08c81e922e313549c029f436ac7d91ef3c9bed8e4049d67d2';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='c5a4e69e2be0e3e5f5bb7c759960b20650967d0f571baad4a7f15b2c03bda352';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     apk del --purge .fetch-deps;     rm -rf /var/cache/apk/*;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_VERSION=8.4.1.35646
# Wed, 15 Jul 2020 23:49:44 GMT
ARG SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
# Wed, 15 Jul 2020 23:49:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin SONARQUBE_HOME=/opt/sonarqube SONAR_VERSION=8.4.1.35646 SQ_DATA_DIR=/opt/sonarqube/data SQ_EXTENSIONS_DIR=/opt/sonarqube/extensions SQ_LOGS_DIR=/opt/sonarqube/logs SQ_TEMP_DIR=/opt/sonarqube/temp
# Wed, 15 Jul 2020 23:50:03 GMT
# ARGS: SONARQUBE_VERSION=8.4.1.35646 SONARQUBE_ZIP_URL=https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-8.4.1.35646.zip
RUN set -ex     && addgroup -S -g 1000 sonarqube     && adduser -S -D -u 1000 -G sonarqube sonarqube     && apk add --no-cache --virtual build-dependencies gnupg unzip curl     && apk add --no-cache bash su-exec ttf-dejavu     && sed --in-place --expression="s?securerandom.source=file:/dev/random?securerandom.source=file:/dev/urandom?g" "${JAVA_HOME}/conf/security/java.security"     && for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "${server}" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done     && mkdir --parents /opt     && cd /opt     && curl --fail --location --output sonarqube.zip --silent --show-error "${SONARQUBE_ZIP_URL}"     && curl --fail --location --output sonarqube.zip.asc --silent --show-error "${SONARQUBE_ZIP_URL}.asc"     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv "sonarqube-${SONARQUBE_VERSION}" sonarqube     && rm sonarqube.zip*     && rm -rf ${SONARQUBE_HOME}/bin/*     && chown -R sonarqube:sonarqube ${SONARQUBE_HOME}     && chmod -R 777 "${SQ_DATA_DIR}" "${SQ_EXTENSIONS_DIR}" "${SQ_LOGS_DIR}" "${SQ_TEMP_DIR}"     && apk del --purge build-dependencies
# Wed, 15 Jul 2020 23:50:03 GMT
COPY --chown=sonarqube:sonarqubemulti:aed345498324cc768d63aba16bd3b3de027a0213cb3a62a9a3b27799dbf88552 in /opt/sonarqube/bin/ 
# Wed, 15 Jul 2020 23:50:04 GMT
WORKDIR /opt/sonarqube
# Wed, 15 Jul 2020 23:50:04 GMT
EXPOSE 9000
# Wed, 15 Jul 2020 23:50:04 GMT
ENTRYPOINT ["bin/run.sh"]
# Wed, 15 Jul 2020 23:50:04 GMT
CMD ["bin/sonar.sh"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02126857e210d47eda3c53a90daba276fd6e3e5a4331351da4ee07f38b794d4d`  
		Last Modified: Thu, 30 Apr 2020 01:22:33 GMT  
		Size: 6.3 MB (6284131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a2496a4dd7bd3c72b32552a7982b0a3b63e00c845b22ef366ad4149e676cf`  
		Last Modified: Thu, 30 Apr 2020 01:22:40 GMT  
		Size: 42.9 MB (42932909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2106c7b928bf49fbfa0588943a6a0f0b0cf4ae75cde0b8fd14054b76518a08e`  
		Last Modified: Wed, 15 Jul 2020 23:51:35 GMT  
		Size: 242.4 MB (242378410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1166e713d353319f45853bd04aa63eb0dd06164e87b9ee40edb1894cf433226d`  
		Last Modified: Wed, 15 Jul 2020 23:51:19 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sonarqube:lts`

```console
$ docker pull sonarqube@sha256:0f6984003b51df517f759fdf23fae7cfdd0eaae473e44ec879e82dd34b81be53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sonarqube:lts` - linux; amd64

```console
$ docker pull sonarqube@sha256:78fe85076b640618b903b7571dc321ee4ce638adc9dcd6bc0054949397684ef7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.7 MB (286706357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2f4d9abb5582755ed8f9d5e83ad602649982ab0e74d38c8d7db7112aab7462`
-	Entrypoint: `[".\/bin\/run.sh"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 22:35:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:35:24 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 22:40:31 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 22 Jul 2020 22:40:32 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 22:40:32 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 22 Jul 2020 22:40:33 GMT
ENV JAVA_VERSION=11.0.8
# Wed, 22 Jul 2020 22:41:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jre_
# Wed, 22 Jul 2020 22:41:22 GMT
ENV JAVA_URL_VERSION=11.0.8_10
# Wed, 22 Jul 2020 22:41:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 23 Jul 2020 09:46:03 GMT
RUN apt-get update     && apt-get install -y curl gnupg2 unzip     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 09:46:03 GMT
ENV SONAR_VERSION=7.9.3 SONARQUBE_HOME=/opt/sonarqube SONARQUBE_JDBC_USERNAME=sonar SONARQUBE_JDBC_PASSWORD=sonar SONARQUBE_JDBC_URL=
# Thu, 23 Jul 2020 09:46:04 GMT
EXPOSE 9000
# Thu, 23 Jul 2020 09:46:04 GMT
RUN groupadd -r sonarqube && useradd -r -g sonarqube sonarqube
# Thu, 23 Jul 2020 09:46:05 GMT
RUN for server in $(shuf -e ha.pool.sks-keyservers.net                             hkp://p80.pool.sks-keyservers.net:80                             keyserver.ubuntu.com                             hkp://keyserver.ubuntu.com:80                             pgp.mit.edu) ; do         gpg --batch --keyserver "$server" --recv-keys F1182E81C792928921DBCAB4CFCA4A29D26468DE && break || : ;     done
# Thu, 23 Jul 2020 09:46:19 GMT
RUN set -x     && cd /opt     && curl -o sonarqube.zip -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip     && curl -o sonarqube.zip.asc -fSL https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-$SONAR_VERSION.zip.asc     && gpg --batch --verify sonarqube.zip.asc sonarqube.zip     && unzip -q sonarqube.zip     && mv sonarqube-$SONAR_VERSION sonarqube     && chown -R sonarqube:sonarqube sonarqube     && rm sonarqube.zip*     && rm -rf $SONARQUBE_HOME/bin/*
# Thu, 23 Jul 2020 09:46:19 GMT
VOLUME [/opt/sonarqube/data]
# Thu, 23 Jul 2020 09:46:19 GMT
WORKDIR /opt/sonarqube
# Thu, 23 Jul 2020 09:46:19 GMT
COPY file:aa007fcc6be4125cbbb27fe345978294add03a4f05e942a5208a37be832addca in /opt/sonarqube/bin/ 
# Thu, 23 Jul 2020 09:46:20 GMT
USER sonarqube
# Thu, 23 Jul 2020 09:46:20 GMT
ENTRYPOINT ["./bin/run.sh"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa4e9b7780660af457791b3bbbd51d1d25c8d9681c1f7ebe5e3a59e0179cecd`  
		Last Modified: Wed, 22 Jul 2020 22:44:33 GMT  
		Size: 3.2 MB (3248441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b5d3bc409673c9f77720030b623cb2c26bda1203fbcca9734ebfe1c68f18d`  
		Last Modified: Wed, 22 Jul 2020 22:47:26 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d63bc6ae26706f2964c7797e192b3141fb5d797712c440d6f07154202c9fd0e`  
		Last Modified: Wed, 22 Jul 2020 22:48:13 GMT  
		Size: 42.2 MB (42225249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c164eb43c04b1a046c75695ade27ae7c130021b79ff52bd0079eef60472ff`  
		Last Modified: Thu, 23 Jul 2020 09:46:43 GMT  
		Size: 6.0 MB (5984842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afa0e94e8006b8aaf322f2551149a49866b820feb9e5e91559e4685dabc6adf`  
		Last Modified: Thu, 23 Jul 2020 09:46:42 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec94ff2322ec5acef43e4252dd1ecbc809ba8fe06065ad282e36f1da090b9ed`  
		Last Modified: Thu, 23 Jul 2020 09:46:42 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778fb561aad2c7b8f4b456573ee0e8a6b7af401b72da3e6ecbdec0255bf2ee28`  
		Last Modified: Thu, 23 Jul 2020 09:46:55 GMT  
		Size: 208.1 MB (208144778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264d9a5f0c2259aa5ff374e0bd8b109cfad6513a217a8f025ccbc0b91ee8e444`  
		Last Modified: Thu, 23 Jul 2020 09:46:42 GMT  
		Size: 788.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
