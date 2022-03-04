## `tomcat:jdk17-temurin-focal`

```console
$ docker pull tomcat@sha256:8f0e37723dd47b4d5f6d3e0fedf7a6dd2f06e21bce418a16cdcad86c8251499a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jdk17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:bd0089c80d5912b24546eda22389ab860564d302edc479803fce9a682e2b3955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.2 MB (263174688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf7ecd2cfe59647803009bd12192aa9dfcae8816bcca1bed2a5c09ec0ed9c922`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:23:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 21:25:04 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 21:25:31 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Thu, 03 Mar 2022 21:25:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='302caf29f73481b2b914ba2b89705036010c65eb9bc8d7712b27d6e9bedf6200';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='544936145a4a9b1a316ed3708cd91b3960d5e8e87578bea73ef674ca3047158e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='532d831d6a977e821b7331ecf9ed995e5bbfe76f18a1b00ffa8dbb3a4e2887de';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='383ac8ad392036bedab9a08eb55395b95593a6cc268c422a2bab53f0977a4c54';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='288f34e3ba8a4838605636485d0365ce23e57d5f2f68997ac4c2e4c01967cd48';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 21:25:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 21:25:50 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 21:25:50 GMT
CMD ["jshell"]
# Fri, 04 Mar 2022 02:29:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 02:29:13 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:29:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 02:29:14 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 02:29:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:29:14 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:29:14 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 02:29:14 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 02:33:33 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 02:33:33 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 02:34:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 04 Mar 2022 02:34:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 02:34:09 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 02:34:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead8efdcc90ae14990292c6f83165336d0bdeed825c627da155c6d6acd9fb5ed`  
		Last Modified: Thu, 03 Mar 2022 21:28:53 GMT  
		Size: 28.6 MB (28566161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f83be9adab414d68b95a808bb8ed6388a348ce1efb2b826f5518388a55f8ce`  
		Last Modified: Thu, 03 Mar 2022 21:29:35 GMT  
		Size: 193.0 MB (193011362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f519ee9b037897bb0865028aee76c540fadc15ccffbc2177f9e91637d3af2f`  
		Last Modified: Thu, 03 Mar 2022 21:29:19 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3e31c4a6415f0be0c6182663a64228ba95dfd6c6ca5b1d3d04b5eaa2d5f6e3`  
		Last Modified: Fri, 04 Mar 2022 02:57:39 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ccb1d55f376b2deeff6c1b6093a706563d66b346790074db0089e0ed806157`  
		Last Modified: Fri, 04 Mar 2022 02:59:59 GMT  
		Size: 13.0 MB (13030953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6e363814dd86bbfec71bafdba180d7fae7ef7d30deb9ce9aad9a1683a1bf60`  
		Last Modified: Fri, 04 Mar 2022 02:59:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jdk17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:a239dc020eb8d351b7aef4dd8cce7f9dbace132324a5ab3bae08d254da6d0279
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.4 MB (254437918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c753a3f6fe6979b64b74a18edf9b9344118ca7ca6f834c9a4dde95db94deee9f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 21:21:31 GMT
ADD file:984d3d8b31abd025bb9be52f42d60245a76b1ee991f286db819ae204da45390c in / 
# Thu, 03 Mar 2022 21:21:32 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 04:40:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 04 Mar 2022 04:44:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Mar 2022 04:45:25 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Fri, 04 Mar 2022 04:45:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='302caf29f73481b2b914ba2b89705036010c65eb9bc8d7712b27d6e9bedf6200';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='544936145a4a9b1a316ed3708cd91b3960d5e8e87578bea73ef674ca3047158e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='532d831d6a977e821b7331ecf9ed995e5bbfe76f18a1b00ffa8dbb3a4e2887de';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='383ac8ad392036bedab9a08eb55395b95593a6cc268c422a2bab53f0977a4c54';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='288f34e3ba8a4838605636485d0365ce23e57d5f2f68997ac4c2e4c01967cd48';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 04 Mar 2022 04:45:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 04:45:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 04 Mar 2022 04:45:55 GMT
CMD ["jshell"]
# Fri, 04 Mar 2022 08:42:53 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 08:42:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 08:42:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 08:42:56 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 08:42:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 08:42:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 08:42:57 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 08:42:57 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 08:49:14 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 08:49:15 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 08:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 04 Mar 2022 08:50:25 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 08:50:26 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 08:50:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:12a77aaceb8aa1438ebb61cb4904d74fc225cfa20464a060980580674a0a31e9`  
		Last Modified: Thu, 03 Mar 2022 21:25:09 GMT  
		Size: 24.1 MB (24073718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70a2e69fec13bdcb7c23e4494afab8160dfd5a076ef7c77ed8324ea6d93b66`  
		Last Modified: Fri, 04 Mar 2022 04:52:53 GMT  
		Size: 27.4 MB (27368418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d361f0f4d66ae4d869c46c4349e33f77efe61e5b55445b2aa9f61666b94389f`  
		Last Modified: Fri, 04 Mar 2022 04:55:15 GMT  
		Size: 190.0 MB (190040306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c0013c0fe87a65fad7d2e78d487c5cb19d4df76e27f593160f17b74358a5e1`  
		Last Modified: Fri, 04 Mar 2022 04:54:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d517562ed8ad2782dfa80f848a13d0854775475ad8aa16d4499b2c4a5357aed7`  
		Last Modified: Fri, 04 Mar 2022 09:26:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205a6467cd621ab16e79f9e6779d78b205df51ff252301690c321fed7173d82`  
		Last Modified: Fri, 04 Mar 2022 09:29:53 GMT  
		Size: 13.0 MB (12955015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f905bc94e01fe41675959104dac4af137150510ef3b22972e693c0b47bf2d63`  
		Last Modified: Fri, 04 Mar 2022 09:29:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jdk17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:29b0a5321aeaad2e3357fe48fcc7218343631c5fc46134208ab21bde404d2713
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259304311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47328723a65a8498410f5308777dcfa7b0a7ef6dcc70d3cdf459d86471b5aa1b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:02 GMT
ADD file:f2fffe739729839aa17484bc4d79d33425549c5052824eac12131b16c23565d3 in / 
# Thu, 03 Mar 2022 19:41:03 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 20:21:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 20:23:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:23:37 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Thu, 03 Mar 2022 20:23:48 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='302caf29f73481b2b914ba2b89705036010c65eb9bc8d7712b27d6e9bedf6200';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='544936145a4a9b1a316ed3708cd91b3960d5e8e87578bea73ef674ca3047158e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='532d831d6a977e821b7331ecf9ed995e5bbfe76f18a1b00ffa8dbb3a4e2887de';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='383ac8ad392036bedab9a08eb55395b95593a6cc268c422a2bab53f0977a4c54';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='288f34e3ba8a4838605636485d0365ce23e57d5f2f68997ac4c2e4c01967cd48';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 20:23:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 20:23:50 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 20:23:50 GMT
CMD ["jshell"]
# Thu, 03 Mar 2022 23:31:23 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 03 Mar 2022 23:31:24 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 23:31:25 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 03 Mar 2022 23:31:26 GMT
WORKDIR /usr/local/tomcat
# Thu, 03 Mar 2022 23:31:27 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 23:31:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 23:31:29 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 03 Mar 2022 23:31:30 GMT
ENV TOMCAT_MAJOR=10
# Thu, 03 Mar 2022 23:38:04 GMT
ENV TOMCAT_VERSION=10.0.17
# Thu, 03 Mar 2022 23:38:05 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Thu, 03 Mar 2022 23:39:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 03 Mar 2022 23:39:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 03 Mar 2022 23:39:03 GMT
EXPOSE 8080
# Thu, 03 Mar 2022 23:39:04 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5a7855fb0d7ae372c824d9c76be5ad2f42ce178c1910fa54a8543036b5325fd5`  
		Last Modified: Thu, 03 Mar 2022 19:42:38 GMT  
		Size: 27.2 MB (27169631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7afec2522dcf8183cf124997a84e381fcddfe101348ae644fdd54a349167ef`  
		Last Modified: Thu, 03 Mar 2022 20:27:34 GMT  
		Size: 29.4 MB (29380102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f7869dd47c74b1623deddc941ff3f440b3e8a909f873ca230be860a961d6f`  
		Last Modified: Thu, 03 Mar 2022 20:28:26 GMT  
		Size: 189.9 MB (189944711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac4679f75449eb96ae5869d48db04466b793755601bd602140a011f80008a88`  
		Last Modified: Thu, 03 Mar 2022 20:28:07 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57e6ee824c3dd79802482f7eb6d329e2602b9fa8afc6883644349e3a7efd421`  
		Last Modified: Fri, 04 Mar 2022 00:28:53 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02446df1fafaf3ff88aa96ab61bee67d41a2fac4f6caf632b47649f45d41e58b`  
		Last Modified: Fri, 04 Mar 2022 00:31:52 GMT  
		Size: 12.8 MB (12809603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jdk17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:d7b562ade85f040a22c1e9c1accabdc76d625f91dad7dfee1d6d8e889958ad8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.5 MB (267494292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88b54797f8a6a8d6da9a5b15a75932d5d6e935010a08b0351e99876ab52c5783`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 20:28:30 GMT
ADD file:039f04ac6c5dbbe3fb0a5eee16945cf7c5fb7565751d6bdf8ec0c1102798c1de in / 
# Thu, 03 Mar 2022 20:28:38 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:04:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 22:11:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 22:12:53 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Thu, 03 Mar 2022 22:13:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='302caf29f73481b2b914ba2b89705036010c65eb9bc8d7712b27d6e9bedf6200';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='544936145a4a9b1a316ed3708cd91b3960d5e8e87578bea73ef674ca3047158e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='532d831d6a977e821b7331ecf9ed995e5bbfe76f18a1b00ffa8dbb3a4e2887de';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='383ac8ad392036bedab9a08eb55395b95593a6cc268c422a2bab53f0977a4c54';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='288f34e3ba8a4838605636485d0365ce23e57d5f2f68997ac4c2e4c01967cd48';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 22:13:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 22:13:46 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 22:13:50 GMT
CMD ["jshell"]
# Fri, 04 Mar 2022 02:15:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 02:15:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 02:15:40 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 02:15:45 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 02:15:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:15:51 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 02:15:52 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 02:15:55 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 02:32:42 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 02:32:45 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 02:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 04 Mar 2022 02:35:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 02:35:45 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 02:35:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a16b43de69d1e799ea2cb675e7e605db0ff3a8d692fd326fbde80a370e0676d5`  
		Last Modified: Thu, 03 Mar 2022 20:33:55 GMT  
		Size: 33.3 MB (33292195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849817e98afbf9ee5cdf1650e92b780ddfc3ab08fd11774b21e9643406ae1ca9`  
		Last Modified: Thu, 03 Mar 2022 22:18:39 GMT  
		Size: 31.1 MB (31122304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d132fa6da0d9f87b881c7ae377616e60ecabc70da0a742386b763b6a5091bd`  
		Last Modified: Thu, 03 Mar 2022 22:19:36 GMT  
		Size: 190.0 MB (189983507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b213ed99d6e1b1425fee2b8ca5bf7ee92adb3f09dccdfb00c405d78ab2bcb09`  
		Last Modified: Thu, 03 Mar 2022 22:19:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d2fda897ae49f40cca3324af0ed65165a2bd09a4138967f722430872bdc2cd`  
		Last Modified: Fri, 04 Mar 2022 03:45:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a6a4818fe6a64e990b6cdb4bb7b7e344860bdcc7c8911238031773690a9d32`  
		Last Modified: Fri, 04 Mar 2022 03:47:32 GMT  
		Size: 13.1 MB (13095823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae49381ce0758e572f0c6ec18d2985d84438f578025489c4fbba67073bca80b`  
		Last Modified: Fri, 04 Mar 2022 03:47:30 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jdk17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:a4613a0613cb600a5b062e433dbc4bfc3589432385bcaafa410d1a8733f22f5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248499192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61fadabfc0965627633d0f8d8f173b3ca79db98209a00ff591038c0bc2a9fae9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 03 Mar 2022 19:41:52 GMT
ADD file:3162233da685a36a9f274a7fa1d99452cab76f37e3640d38851c782ca506f75b in / 
# Thu, 03 Mar 2022 19:41:53 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 19:59:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 20:00:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 03 Mar 2022 20:00:43 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Thu, 03 Mar 2022 20:00:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='302caf29f73481b2b914ba2b89705036010c65eb9bc8d7712b27d6e9bedf6200';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.2_8.tar.gz';          ;;        armhf|arm)          ESUM='544936145a4a9b1a316ed3708cd91b3960d5e8e87578bea73ef674ca3047158e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_arm_linux_hotspot_17.0.2_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='532d831d6a977e821b7331ecf9ed995e5bbfe76f18a1b00ffa8dbb3a4e2887de';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.2_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='383ac8ad392036bedab9a08eb55395b95593a6cc268c422a2bab53f0977a4c54';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.2_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='288f34e3ba8a4838605636485d0365ce23e57d5f2f68997ac4c2e4c01967cd48';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.2%2B8/OpenJDK17U-jdk_x64_linux_hotspot_17.0.2_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 03 Mar 2022 20:00:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 20:00:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 03 Mar 2022 20:00:55 GMT
CMD ["jshell"]
# Thu, 03 Mar 2022 21:09:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 03 Mar 2022 21:09:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Mar 2022 21:09:06 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 03 Mar 2022 21:09:07 GMT
WORKDIR /usr/local/tomcat
# Thu, 03 Mar 2022 21:09:07 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 21:09:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 03 Mar 2022 21:09:07 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 03 Mar 2022 21:09:07 GMT
ENV TOMCAT_MAJOR=10
# Thu, 03 Mar 2022 21:12:42 GMT
ENV TOMCAT_VERSION=10.0.17
# Thu, 03 Mar 2022 21:12:42 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Thu, 03 Mar 2022 21:13:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 03 Mar 2022 21:13:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 03 Mar 2022 21:13:26 GMT
EXPOSE 8080
# Thu, 03 Mar 2022 21:13:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ade7e68f4e34f438527a34c9761a285c3c3864e3daab0544b2c4f4163c7c3f56`  
		Last Modified: Thu, 03 Mar 2022 19:43:22 GMT  
		Size: 27.1 MB (27084671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67794419b7271832d65da191bde592a4c2e4dbf8f986cd2cde08544ec953bcfc`  
		Last Modified: Thu, 03 Mar 2022 20:02:48 GMT  
		Size: 27.9 MB (27942763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4959680ee63d12ffb90da2240f8665902c4c77ddf7a425e7d139b3509c76863c`  
		Last Modified: Thu, 03 Mar 2022 20:03:17 GMT  
		Size: 180.4 MB (180427154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0d4deb0650b7ea090f2eb79d73e2ad6d610261e07aa7bdb0e57f67725819d`  
		Last Modified: Thu, 03 Mar 2022 20:03:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032b5c9f88d46434dd47ad4a0432a8fe5f9b105384dfea26bc18253feda3226e`  
		Last Modified: Thu, 03 Mar 2022 21:29:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cf2db16db0a186b2aae1162c2feb734439dc91c3d7e1bab9eaed4dde4ce4a6`  
		Last Modified: Thu, 03 Mar 2022 21:31:13 GMT  
		Size: 13.0 MB (13044141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c5a8f7ae404065d7af27f2dae94c41969284bfdde1d92ffd5f0aaeed2dc6c`  
		Last Modified: Thu, 03 Mar 2022 21:31:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
