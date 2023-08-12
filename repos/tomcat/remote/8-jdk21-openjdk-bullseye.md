## `tomcat:8-jdk21-openjdk-bullseye`

```console
$ docker pull tomcat@sha256:a05818f2761dc900b7f2980a779c4563147277866bea4792f012872eeb37a173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:8-jdk21-openjdk-bullseye` - linux; amd64

```console
$ docker pull tomcat@sha256:2dd35ce7438384c48dce8867c9cfe02eaac9f8973762dd71086769603869edd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.2 MB (355186549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3385cc70d2968ab336cb2412562c35ff8a68434cd03c17783b95decca8629209`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:09:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:10:37 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Fri, 28 Jul 2023 04:10:37 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 04:10:37 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:05:03 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:05:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:05:14 GMT
CMD ["jshell"]
# Sat, 12 Aug 2023 00:16:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 12 Aug 2023 00:16:55 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Aug 2023 00:16:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 12 Aug 2023 00:16:55 GMT
WORKDIR /usr/local/tomcat
# Sat, 12 Aug 2023 00:16:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 12 Aug 2023 00:16:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 12 Aug 2023 00:19:56 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 12 Aug 2023 00:19:56 GMT
ENV TOMCAT_MAJOR=8
# Sat, 12 Aug 2023 00:19:57 GMT
ENV TOMCAT_VERSION=8.5.91
# Sat, 12 Aug 2023 00:19:57 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Sat, 12 Aug 2023 00:20:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 12 Aug 2023 00:20:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 12 Aug 2023 00:20:22 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:20:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28bfe4d14b6484ed32c77d146385c72ef90db4a661c6c0e87429110ac5eba9a`  
		Last Modified: Fri, 28 Jul 2023 04:13:30 GMT  
		Size: 14.1 MB (14072137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f367fb0642c194b8d4e1cced6c0128c417d68ba2b06fbbd499828981d441312`  
		Last Modified: Sat, 12 Aug 2023 00:12:46 GMT  
		Size: 204.0 MB (204045758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cdb189e27774dc486065a2dd939e00ca9dc8a58889c22b22af139172e60f9`  
		Last Modified: Sat, 12 Aug 2023 00:28:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d12c053bd6315fb4e73c65806b29f9fe87c24de6a0cd8bc6c809fd3d684088e`  
		Last Modified: Sat, 12 Aug 2023 00:32:45 GMT  
		Size: 11.7 MB (11667162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e6c2f767f0b741932a50e3b8345c0169e255bd209a18f2f80c656c644de6f8`  
		Last Modified: Sat, 12 Aug 2023 00:32:43 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk21-openjdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:f9a9fab0e6499b036f6bbd5173820f1a06c20c0e4ad87aec93508a08535b31a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.7 MB (353715219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98f6cfce627296fb3c39e30437b069e074c169042a79ea7d2f3044bc82fac474`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:07 GMT
ADD file:a0144d077c2c6b73bbb5f7e7b8e6b58e4127de2a5faf907cd4e83e4d83437fad in / 
# Thu, 27 Jul 2023 23:43:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:37:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:37:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:41:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:42:47 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Fri, 28 Jul 2023 10:42:48 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jul 2023 10:42:48 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:29:45 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:29:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:29:55 GMT
CMD ["jshell"]
# Sat, 12 Aug 2023 01:03:04 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 12 Aug 2023 01:03:04 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 12 Aug 2023 01:03:04 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 12 Aug 2023 01:03:04 GMT
WORKDIR /usr/local/tomcat
# Sat, 12 Aug 2023 01:03:04 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 12 Aug 2023 01:03:05 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 12 Aug 2023 01:05:33 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 12 Aug 2023 01:05:33 GMT
ENV TOMCAT_MAJOR=8
# Sat, 12 Aug 2023 01:05:33 GMT
ENV TOMCAT_VERSION=8.5.91
# Sat, 12 Aug 2023 01:05:33 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Sat, 12 Aug 2023 01:05:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 12 Aug 2023 01:05:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 12 Aug 2023 01:05:55 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 01:05:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:49185a1a3bc353699370ac57d50a7b7234b59616b6aebde79ba6a0a0314bb107`  
		Last Modified: Thu, 27 Jul 2023 23:46:34 GMT  
		Size: 53.7 MB (53704790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f6f6b31000e991bdd81caebc21e281fc1350f09586d393f3b8bf36dceeb99e`  
		Last Modified: Fri, 28 Jul 2023 01:42:56 GMT  
		Size: 15.7 MB (15746528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385ee361272e1c36fe7d96fe8ab6b0f30cf33bfb9bbe29bfc2d33f51bd771993`  
		Last Modified: Fri, 28 Jul 2023 01:43:10 GMT  
		Size: 54.7 MB (54676175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3685694dfe4a43e9db9358680ffcb69ef3c8ee13df6588581a7bc2d034d0e00`  
		Last Modified: Fri, 28 Jul 2023 10:45:29 GMT  
		Size: 15.5 MB (15529258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a05f123fb0f24deba67d1ed26819d584995ec0c665f66e61272cfd672d6edc`  
		Last Modified: Sat, 12 Aug 2023 00:36:35 GMT  
		Size: 202.4 MB (202382260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2075dc1fe343ce2a1eef97f1454b5c6e913defe0fd5e0c3fffe53118b55c3e03`  
		Last Modified: Sat, 12 Aug 2023 01:13:41 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dc72d885823d08a568ce91836034799e5181c8799e89e018cfd3d3434c0413`  
		Last Modified: Sat, 12 Aug 2023 01:17:50 GMT  
		Size: 11.7 MB (11675905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49700f5454d3235fe587b39003447d32f8358a0f34b7b2530ae640f44cdb7f8`  
		Last Modified: Sat, 12 Aug 2023 01:17:49 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
