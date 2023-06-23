## `tomcat:8-jdk21-openjdk-bullseye`

```console
$ docker pull tomcat@sha256:7a22b32484338a46ec496a8f47ce7bedab49250a90ffdb72bb1f8ec64113da5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:8-jdk21-openjdk-bullseye` - linux; amd64

```console
$ docker pull tomcat@sha256:43b53196e608308aae8bd1b6b6e864fd64018211713eccb693f25113664ca9dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355087247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cceaa938e1211c2a5c980d857d64cfe574eeda46024e94052481bd445a86b6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:29:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:19:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:20:35 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 07:20:35 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 07:20:36 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 00:28:28 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 00:28:39 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c5ff4dc462286ead4a7f1480719f695a976a130005df30d33ba210aadc094ff9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='4f98a729913be1d28fda8491420394e394fbbf84c4d1f41f05b83ba4c8b989aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:28:40 GMT
CMD ["jshell"]
# Fri, 23 Jun 2023 00:55:12 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 23 Jun 2023 00:55:12 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jun 2023 00:55:13 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 23 Jun 2023 00:55:13 GMT
WORKDIR /usr/local/tomcat
# Fri, 23 Jun 2023 00:55:13 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 23 Jun 2023 00:55:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 23 Jun 2023 00:58:24 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 23 Jun 2023 00:58:24 GMT
ENV TOMCAT_MAJOR=8
# Fri, 23 Jun 2023 00:58:24 GMT
ENV TOMCAT_VERSION=8.5.90
# Fri, 23 Jun 2023 00:58:24 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Fri, 23 Jun 2023 00:58:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Fri, 23 Jun 2023 00:58:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 23 Jun 2023 00:58:51 GMT
EXPOSE 8080
# Fri, 23 Jun 2023 00:58:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4d59f9abaeb4efe1c66ff2176044e93912966342d76d025b6d1a2a37dde7a`  
		Last Modified: Tue, 13 Jun 2023 03:37:49 GMT  
		Size: 54.6 MB (54585023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b6071e5acc46917aa272d6eccdeb02e82f41fada3c7c2a4fb0d54dcab17637`  
		Last Modified: Tue, 13 Jun 2023 07:22:22 GMT  
		Size: 14.1 MB (14071943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c515d919fbb285069396635313bc1326689f17c0ce2c191803bc93c849abb018`  
		Last Modified: Fri, 23 Jun 2023 00:35:57 GMT  
		Size: 204.0 MB (203960578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291dbcc70b4d41ec16b6d187a3e815c786e0d2febb080db7253fd027aace3eae`  
		Last Modified: Fri, 23 Jun 2023 01:05:19 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ed3ba3c6e9653c9fd4045e71a6678e0958d1abfa20053344525b834754894`  
		Last Modified: Fri, 23 Jun 2023 01:06:52 GMT  
		Size: 11.7 MB (11653909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c8cfd37aa26794d18b008be4cc75659541efd304a36eafe03e634b8f1e9119`  
		Last Modified: Fri, 23 Jun 2023 01:06:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk21-openjdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:b6405fa03d22bf6f379b2aed028bda3916306cc5056ce3c8848347b30bb2e73b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.6 MB (353614492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abdd0ff0d76dcd94dc13e89f023483d9f235f6ff60d0ecdb142049d5c31f1750`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:01:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:38:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:40:03 GMT
ENV JAVA_HOME=/usr/local/openjdk-21
# Tue, 13 Jun 2023 04:40:03 GMT
ENV PATH=/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 04:40:03 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 01:06:55 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 01:07:03 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c5ff4dc462286ead4a7f1480719f695a976a130005df30d33ba210aadc094ff9'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='4f98a729913be1d28fda8491420394e394fbbf84c4d1f41f05b83ba4c8b989aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 01:07:05 GMT
CMD ["jshell"]
# Fri, 23 Jun 2023 03:26:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 23 Jun 2023 03:26:02 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jun 2023 03:26:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 23 Jun 2023 03:26:03 GMT
WORKDIR /usr/local/tomcat
# Fri, 23 Jun 2023 03:26:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 23 Jun 2023 03:26:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 23 Jun 2023 03:28:27 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 23 Jun 2023 03:28:27 GMT
ENV TOMCAT_MAJOR=8
# Fri, 23 Jun 2023 03:28:28 GMT
ENV TOMCAT_VERSION=8.5.90
# Fri, 23 Jun 2023 03:28:28 GMT
ENV TOMCAT_SHA512=bce0659288ae46bcf7218dc133b7455d395572db6d09cba244119caf02c24590db0959e773a6e9187b6dbd0934482fe3f34add9e3ec512af8a9fe224993a9fe0
# Fri, 23 Jun 2023 03:28:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Fri, 23 Jun 2023 03:28:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 23 Jun 2023 03:28:51 GMT
EXPOSE 8080
# Fri, 23 Jun 2023 03:28:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b90602383b5196ae0f8744277182f671de6f12c55664a9f36b274ab9266b5cc`  
		Last Modified: Tue, 13 Jun 2023 03:08:47 GMT  
		Size: 54.7 MB (54676037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9763270a318f4900a86c9cd1703dbeac7939447c20ca52598ccbe2f05fabf9a1`  
		Last Modified: Tue, 13 Jun 2023 04:41:48 GMT  
		Size: 15.5 MB (15528952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264579f1c972102e07a1bfb76ee1fac37e2a559c7cd2387565a37a9c8a861e72`  
		Last Modified: Fri, 23 Jun 2023 03:07:24 GMT  
		Size: 202.3 MB (202292178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d5cdffb33695b0d17f10ff5643f537f6758e2a87d10bf7ba7874e9e7a31110`  
		Last Modified: Fri, 23 Jun 2023 03:34:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4bbc566721b2b09a8ac9b3fbed3d61fb4658a43bcb9fce960e0ded6fca762c`  
		Last Modified: Fri, 23 Jun 2023 03:35:29 GMT  
		Size: 11.7 MB (11666325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f5aa0a4f8457d59cc2a9ac17f3ea43bf871a567b2931fdf21174f65ac2b7b7`  
		Last Modified: Fri, 23 Jun 2023 03:35:27 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
