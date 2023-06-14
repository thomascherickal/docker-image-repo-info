## `tomcat:9-jdk21-openjdk`

```console
$ docker pull tomcat@sha256:db9548f3fe3060cd03cd15c672f8230d46e17724f64fcd38d045f85b8e4d394b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk21-openjdk` - linux; amd64

```console
$ docker pull tomcat@sha256:68e99cd791eef7052c3a3d5f581a0faa25b4d68e377144717d1154ac7e4865ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.2 MB (371183371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7afd4ac50ae0038ec3909bee2fff208f79a247e222ec4b5ae95b72b5b759c96f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:28 GMT
ADD file:98cacc5890a8c0b29d7a2b296774428cb2268b01b4ff97a84deadcd3b513f319 in / 
# Mon, 12 Jun 2023 23:20:29 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:26:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:27:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:42:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:43:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 18:43:06 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:43:06 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 18:43:06 GMT
ENV JAVA_VERSION=21-ea+26
# Tue, 13 Jun 2023 18:43:17 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='16c6b09c742e73c9e092134517ecc36db2a5e44453c8b8b5374cfac1ee367a28'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='aa59bb222c548c18c21cb05a71854a46263a618a72ec6f2f408328689280380d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jun 2023 18:43:18 GMT
CMD ["jshell"]
# Wed, 14 Jun 2023 06:58:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 14 Jun 2023 06:58:37 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 06:58:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 14 Jun 2023 06:58:38 GMT
WORKDIR /usr/local/tomcat
# Wed, 14 Jun 2023 06:58:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 14 Jun 2023 06:58:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 14 Jun 2023 07:01:02 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 14 Jun 2023 07:01:02 GMT
ENV TOMCAT_MAJOR=9
# Wed, 14 Jun 2023 07:01:02 GMT
ENV TOMCAT_VERSION=9.0.76
# Wed, 14 Jun 2023 07:01:02 GMT
ENV TOMCAT_SHA512=028163cbe15367f0ab60e086b0ebc8d774e62d126d82ae9152f863d4680e280b11c9503e3b51ee7089ca9bea1bfa5b535b244a727a3021e5fa72dd7e9569af9a
# Wed, 14 Jun 2023 07:01:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 14 Jun 2023 07:01:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 14 Jun 2023 07:01:24 GMT
EXPOSE 8080
# Wed, 14 Jun 2023 07:01:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bba7bb10d5baebcaad1d68ab3cbfd37390c646b2a688529b1d118a47991116f4`  
		Last Modified: Mon, 12 Jun 2023 23:25:26 GMT  
		Size: 49.6 MB (49552112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2b820b8e87758dde67c29b25d4cbf88377601a4355cc5d556a9beebc80da00`  
		Last Modified: Tue, 13 Jun 2023 03:36:28 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284f2345db055020282f6e80a646f1111fb2d5dfc6f7ee871f89bc50919a51bf`  
		Last Modified: Tue, 13 Jun 2023 03:36:47 GMT  
		Size: 64.1 MB (64111555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9350d4cb97cd74af4173b0a47cb308cd97cec7c6d33e7f66f37adf410f7b5d31`  
		Last Modified: Tue, 13 Jun 2023 18:44:35 GMT  
		Size: 16.9 MB (16947115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f215860789dfaa9d4d1be50df534c0249d4f377c19870868732a54bb4a3f0e`  
		Last Modified: Tue, 13 Jun 2023 18:46:10 GMT  
		Size: 203.9 MB (203938200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ff926878b3299fa1f70289546d4ec135d865c933b2f9b51ae62ecdbb340e82`  
		Last Modified: Wed, 14 Jun 2023 07:08:33 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c4b8cbc0e0fb84504b126c7c38d2b0df5090a9a1358cfc5ed6930b07a951b2`  
		Last Modified: Wed, 14 Jun 2023 07:10:05 GMT  
		Size: 12.6 MB (12603547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad654f238b74ada3cb62ad39327470e273943959dadcb710e263e5f7421633`  
		Last Modified: Wed, 14 Jun 2023 07:10:04 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk21-openjdk` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:1da6bded92fd32e86d27e2041ce11bb9a1656a6dcb0180598b3125cbe26d35cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.8 MB (369752932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dab1f8b46358e8f8aff4bb1b6f73789496e724a22802db2eeb9a7b5bdb883a2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 12 Jun 2023 23:39:59 GMT
ADD file:0dfaa4beac7b0a95f2b33bc35e08b104057469f46fa35df2af7193451ab3714d in / 
# Mon, 12 Jun 2023 23:40:00 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:59:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:27:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:27:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 18:27:56 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 18:27:56 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 18:27:56 GMT
ENV JAVA_VERSION=21-ea+26
# Tue, 13 Jun 2023 18:28:06 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='16c6b09c742e73c9e092134517ecc36db2a5e44453c8b8b5374cfac1ee367a28'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='aa59bb222c548c18c21cb05a71854a46263a618a72ec6f2f408328689280380d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jun 2023 18:28:08 GMT
CMD ["jshell"]
# Wed, 14 Jun 2023 00:45:20 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 14 Jun 2023 00:45:20 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 00:45:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 14 Jun 2023 00:45:21 GMT
WORKDIR /usr/local/tomcat
# Wed, 14 Jun 2023 00:45:21 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 14 Jun 2023 00:45:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 14 Jun 2023 00:47:30 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 14 Jun 2023 00:47:30 GMT
ENV TOMCAT_MAJOR=9
# Wed, 14 Jun 2023 00:47:30 GMT
ENV TOMCAT_VERSION=9.0.76
# Wed, 14 Jun 2023 00:47:30 GMT
ENV TOMCAT_SHA512=028163cbe15367f0ab60e086b0ebc8d774e62d126d82ae9152f863d4680e280b11c9503e3b51ee7089ca9bea1bfa5b535b244a727a3021e5fa72dd7e9569af9a
# Wed, 14 Jun 2023 00:47:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 14 Jun 2023 00:47:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 14 Jun 2023 00:47:49 GMT
EXPOSE 8080
# Wed, 14 Jun 2023 00:47:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a31111d070044ed920abddebc16bfa67a69fb0e0e782b703073c93ec10dedf67`  
		Last Modified: Mon, 12 Jun 2023 23:43:47 GMT  
		Size: 49.6 MB (49573162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2455b35210792787557bbd2b0b976aa27a8bd5931191be95c7291b93b9e38f6c`  
		Last Modified: Tue, 13 Jun 2023 03:07:36 GMT  
		Size: 23.6 MB (23569494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd13397d6ccd754586b475131a51ebeb69394eb49de84b647f4fb6a38703da89`  
		Last Modified: Tue, 13 Jun 2023 03:07:53 GMT  
		Size: 64.0 MB (63983834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a8c967ff35ea3c019c6a9818d32a376ba3b75b94ba824f757a0d12df5614c3`  
		Last Modified: Tue, 13 Jun 2023 18:29:20 GMT  
		Size: 17.7 MB (17728902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88aedaf93b102b61dcc6c76bc7610c928b00281876c44ebf178bbde882533e6`  
		Last Modified: Tue, 13 Jun 2023 18:30:49 GMT  
		Size: 202.3 MB (202286131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f26f4a232a1aafbec890dd4a8bb76d48fcbb2a029932dfcddabe4a71e6193b`  
		Last Modified: Wed, 14 Jun 2023 00:54:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d8c8126a02b253347c42d065eb2870473efaa3c1db2e0c8ac4c926c0810e4b`  
		Last Modified: Wed, 14 Jun 2023 00:56:38 GMT  
		Size: 12.6 MB (12611109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59556ad6f36bc3713fc66851e21709b9fb74610bb1d216f1ea7609e3b7de2d97`  
		Last Modified: Wed, 14 Jun 2023 00:56:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
