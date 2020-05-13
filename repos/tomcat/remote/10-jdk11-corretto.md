## `tomcat:10-jdk11-corretto`

```console
$ docker pull tomcat@sha256:374546e00ef8fe3b981a7ce4cfd92e8a886cfabe90b9ea53dce2e0e0684742d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jdk11-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:8d166ef30286edf8ebbec1b9921c30fef1a9c6277722cf0fa9ec46dd92bd9af3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221577196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944a0bf013900b1f5ea61eb65212966475af8b5074fa080af7ff22f5fc49116`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:51:29 GMT
ARG version=11.0.7.10-1
# Wed, 29 Apr 2020 23:20:27 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 29 Apr 2020 23:20:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 29 Apr 2020 23:37:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 29 Apr 2020 23:37:27 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Apr 2020 23:37:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 29 Apr 2020 23:37:28 GMT
WORKDIR /usr/local/tomcat
# Wed, 29 Apr 2020 23:37:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 29 Apr 2020 23:37:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 29 Apr 2020 23:37:28 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 29 Apr 2020 23:37:28 GMT
ENV TOMCAT_MAJOR=10
# Wed, 13 May 2020 01:58:05 GMT
ENV TOMCAT_VERSION=10.0.0-M5
# Wed, 13 May 2020 01:58:05 GMT
ENV TOMCAT_SHA512=09d6d4c084857d3a7846fdb4ed562ef49402a164dbd140636a7d8fe1370f902f56144d8a20cc71b698189b873ce38cec2a12c38abedb6d7173b091eb46ea26a9
# Wed, 13 May 2020 01:59:36 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| sort -u 			| xargs -r rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 13 May 2020 01:59:38 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 May 2020 01:59:38 GMT
EXPOSE 8080
# Wed, 13 May 2020 01:59:38 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d195fe3929b2a2dd78d22148b5ee06df7ffc52f14a78429cf5f833e0e26c9fe5`  
		Last Modified: Wed, 29 Apr 2020 23:21:08 GMT  
		Size: 145.1 MB (145126677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91648fac434f865f0cfdb58f6a87af6c3d72464cc19b3a61c6fa89454584066`  
		Last Modified: Wed, 29 Apr 2020 23:52:42 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7faa9dca559a306bc76680f0d3c49791152e283edb4a86262f78b22dcacea8`  
		Last Modified: Wed, 13 May 2020 02:29:31 GMT  
		Size: 14.8 MB (14831182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404a49cb3a29963ddd0b9903499af09ef16752b5ef6fc91b1d1e08f8daca3b0`  
		Last Modified: Wed, 13 May 2020 02:29:29 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk11-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:f21dd215aff6114eff0d3af51589e745c7b48e5363d64d392f771f7f07a75204
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.8 MB (221843355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b176f08b189627572519bfe1e97e6bcc02c13fc0938512e4cd5caccd1ea56229`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 19:26:46 GMT
ARG version=11.0.7.10-1
# Wed, 29 Apr 2020 23:40:57 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 29 Apr 2020 23:40:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 30 Apr 2020 00:01:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 30 Apr 2020 00:01:03 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Apr 2020 00:01:04 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 30 Apr 2020 00:01:05 GMT
WORKDIR /usr/local/tomcat
# Thu, 30 Apr 2020 00:01:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 30 Apr 2020 00:01:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 30 Apr 2020 00:01:07 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 30 Apr 2020 00:01:08 GMT
ENV TOMCAT_MAJOR=10
# Wed, 13 May 2020 01:47:30 GMT
ENV TOMCAT_VERSION=10.0.0-M5
# Wed, 13 May 2020 01:47:32 GMT
ENV TOMCAT_SHA512=09d6d4c084857d3a7846fdb4ed562ef49402a164dbd140636a7d8fe1370f902f56144d8a20cc71b698189b873ce38cec2a12c38abedb6d7173b091eb46ea26a9
# Wed, 13 May 2020 01:49:05 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| sort -u 			| xargs -r rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 13 May 2020 01:49:12 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 May 2020 01:49:13 GMT
EXPOSE 8080
# Wed, 13 May 2020 01:49:13 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719ce9c572714bce34bed2d488330731b35adac7227db1447baef738078401`  
		Last Modified: Wed, 29 Apr 2020 23:42:00 GMT  
		Size: 144.0 MB (143963197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a250aed1a7404c01c03b4ea4b77e6cc04a450644a06a0f668d1757f4970a32`  
		Last Modified: Thu, 30 Apr 2020 00:14:14 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6807f63cb2d9c96022ecde4ac8759a21741e04d3035b7db2b70b1a4fd220cd`  
		Last Modified: Wed, 13 May 2020 02:12:56 GMT  
		Size: 14.8 MB (14800061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370fb300549239751e2256a1e1fb819ddbd61ddbdcaca0abf1d3e37b463bb73c`  
		Last Modified: Wed, 13 May 2020 02:12:53 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
