## `tomcat:10-jdk21-openjdk-bookworm`

```console
$ docker pull tomcat@sha256:33c98b405b1c85fbfdd90fea152cfc7d8cf7fe3c6742becee692f0fa5f656f37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jdk21-openjdk-bookworm` - linux; amd64

```console
$ docker pull tomcat@sha256:5ce66e956ac9b8614dfef3230efb64e0e52c3b250e1f3b289ebdcee9e059a059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.2 MB (371191143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6750145595b46e1599c824593d79a197494c5f6f9bc562f81f74599f3bb936`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:47:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 17:48:54 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 17:48:54 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:48:54 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 17:48:54 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 17:49:04 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='414ca270602b11d0b674c105d1d5577793c9db79e2947187e663dba4750cbf9b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='ddfa7ea3dd22c846676b4def3aef78a5411c208987ace8f47bbcfafd33f26f46'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 04 Jul 2023 17:49:04 GMT
CMD ["jshell"]
# Tue, 04 Jul 2023 17:55:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 04 Jul 2023 17:55:21 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:55:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 04 Jul 2023 17:55:22 GMT
WORKDIR /usr/local/tomcat
# Tue, 04 Jul 2023 17:55:22 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 04 Jul 2023 17:55:22 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 04 Jul 2023 17:56:24 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 04 Jul 2023 17:56:25 GMT
ENV TOMCAT_MAJOR=10
# Tue, 04 Jul 2023 17:56:25 GMT
ENV TOMCAT_VERSION=10.1.10
# Tue, 04 Jul 2023 17:56:25 GMT
ENV TOMCAT_SHA512=be35edeb7f63be2d087da6b5cf3c1250eb5fbaa484ba788870780109278d1f5607bf8dfb40f718beda82352109c131fc97f7907f5521dc462bd60773b33e2c68
# Tue, 04 Jul 2023 17:56:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Tue, 04 Jul 2023 17:56:46 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 04 Jul 2023 17:56:46 GMT
EXPOSE 8080
# Tue, 04 Jul 2023 17:56:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe2eadbbcddf082c22d3a63d0dabdea67e8dca87688709258efc404506be95b`  
		Last Modified: Tue, 04 Jul 2023 17:50:58 GMT  
		Size: 16.9 MB (16947014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2856a1a6da1367c73cf89de086d5a15e709f50929e72bfc864dfdded38e6e97`  
		Last Modified: Tue, 04 Jul 2023 17:53:00 GMT  
		Size: 204.0 MB (203984575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f58da83f79b5765e65d209a6a0676fbc580267a4f942dcd6cfe404e55f9ad7`  
		Last Modified: Tue, 04 Jul 2023 18:05:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c91a7503dcdf622864137f5b844224506182bf7712dcfefd0aa8d16423810bc`  
		Last Modified: Tue, 04 Jul 2023 18:06:00 GMT  
		Size: 12.6 MB (12565614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e35b8a048e1ca0e20db0ef5185a62da5ba4cc280e9318b27fca0fea58145a1`  
		Last Modified: Tue, 04 Jul 2023 18:05:59 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk21-openjdk-bookworm` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:f03130d6b38567686a46a0953b411cc2a996eaf08b2bf608f41f883a02e27e94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.7 MB (369745882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6b983b6ddebb72d90c7ec3d8624db00f64b7623ed9bd2786921f14fb30f338`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:26:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:28:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 04 Jul 2023 13:28:21 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 13:28:21 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 13:28:21 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 13:28:29 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='414ca270602b11d0b674c105d1d5577793c9db79e2947187e663dba4750cbf9b'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='ddfa7ea3dd22c846676b4def3aef78a5411c208987ace8f47bbcfafd33f26f46'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 04 Jul 2023 13:28:31 GMT
CMD ["jshell"]
# Wed, 05 Jul 2023 02:51:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Jul 2023 02:51:46 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 02:51:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Jul 2023 02:51:46 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Jul 2023 02:51:46 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 02:51:46 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 02:52:47 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 05 Jul 2023 02:52:47 GMT
ENV TOMCAT_MAJOR=10
# Wed, 05 Jul 2023 02:52:47 GMT
ENV TOMCAT_VERSION=10.1.10
# Wed, 05 Jul 2023 02:52:47 GMT
ENV TOMCAT_SHA512=be35edeb7f63be2d087da6b5cf3c1250eb5fbaa484ba788870780109278d1f5607bf8dfb40f718beda82352109c131fc97f7907f5521dc462bd60773b33e2c68
# Wed, 05 Jul 2023 02:53:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 05 Jul 2023 02:53:04 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 05 Jul 2023 02:53:04 GMT
EXPOSE 8080
# Wed, 05 Jul 2023 02:53:04 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194d600b7f300615aada88430a937774f4f19a53f70de68b85504b8cb5bfbf3`  
		Last Modified: Tue, 04 Jul 2023 13:30:27 GMT  
		Size: 17.7 MB (17728896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81b58cf25e2ab89be6d1f8fb56265202684cb1d019b3a35b3c55eb1c38cc549`  
		Last Modified: Tue, 04 Jul 2023 13:32:44 GMT  
		Size: 202.3 MB (202322122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2777424bfc4aea7914d91cfd7020f0c08911554258e0278676cee7be757e12`  
		Last Modified: Wed, 05 Jul 2023 03:11:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce83ece177b42f860866305212a84b26bcef517c6967a3b8b7481e669fc11419`  
		Last Modified: Wed, 05 Jul 2023 03:12:09 GMT  
		Size: 12.6 MB (12568160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d94a23df084d8223c019313d9c5ed68379b4865f26468f3dd229688aed44fc`  
		Last Modified: Wed, 05 Jul 2023 03:12:08 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
