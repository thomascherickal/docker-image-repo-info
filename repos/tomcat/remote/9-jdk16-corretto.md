## `tomcat:9-jdk16-corretto`

```console
$ docker pull tomcat@sha256:3af2ee66da4ccc63c79cdd11bb52945fb4279db760dc408a45735161160b46d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk16-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:e1da95f152d7f1d8d3248866bb87fe0bb4c727df63a36171fbd2ffe2d8338daf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.8 MB (238825755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf2db9b1b351fd7d469e20da8dcd8d1ea3a66e407ce8607294ec1fdbe0eb2e1`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Tue, 03 Aug 2021 00:05:15 GMT
ARG version=16.0.2.7-1
# Tue, 03 Aug 2021 00:05:37 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 03 Aug 2021 00:05:37 GMT
ENV LANG=C.UTF-8
# Tue, 03 Aug 2021 00:05:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
# Tue, 03 Aug 2021 00:23:18 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Aug 2021 00:23:18 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Aug 2021 00:23:19 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Aug 2021 00:23:19 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Aug 2021 00:23:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:23:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:26:15 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 03 Aug 2021 00:26:15 GMT
ENV TOMCAT_MAJOR=9
# Sat, 07 Aug 2021 00:56:34 GMT
ENV TOMCAT_VERSION=9.0.52
# Sat, 07 Aug 2021 00:56:34 GMT
ENV TOMCAT_SHA512=35e007e8e30e12889da27f9c71a6f4997b9cb5023b703d99add5de9271828e7d8d4956bf34dd2f48c7c71b4f8480f318c9067a4cd2a6d76eaae466286db4897b
# Sat, 07 Aug 2021 00:57:11 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 07 Aug 2021 00:57:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 07 Aug 2021 00:57:13 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 00:57:13 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd35e490fe48e50bf71ec9795af88a13249ced74e6f7a268c64bd95114226b8`  
		Last Modified: Tue, 03 Aug 2021 00:07:30 GMT  
		Size: 160.0 MB (159979624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f10a0df7651e7a5708a52dce26ee76cd8b01265ceef366ad8ec6bbe2104524`  
		Last Modified: Tue, 03 Aug 2021 00:35:38 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e47f078095703d9e23f3ed69adfba3904a00678fc5fc3198c9d8ec81be22be8`  
		Last Modified: Sat, 07 Aug 2021 01:10:24 GMT  
		Size: 16.9 MB (16880154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc9625c5ebcf3ab7114b0589d70b6181334dfc8925a539adaf82a98fe08da2`  
		Last Modified: Sat, 07 Aug 2021 01:10:22 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk16-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:695b5c2a54bb6b793a0f59fbc6a50a9db2cc5a72725f5fa4e520f518b1277d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.4 MB (240363795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d9d85b115dea40183173fe84edb130fb104e889c8fb9944d4d162868fa587b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Aug 2021 00:08:23 GMT
ARG version=16.0.2.7-1
# Tue, 03 Aug 2021 00:08:42 GMT
# ARGS: version=16.0.2.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 03 Aug 2021 00:08:42 GMT
ENV LANG=C.UTF-8
# Tue, 03 Aug 2021 00:08:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
# Tue, 03 Aug 2021 00:35:14 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Aug 2021 00:35:15 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Aug 2021 00:35:15 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Aug 2021 00:35:15 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Aug 2021 00:35:16 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:35:16 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:38:48 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 03 Aug 2021 00:38:48 GMT
ENV TOMCAT_MAJOR=9
# Sat, 07 Aug 2021 01:44:58 GMT
ENV TOMCAT_VERSION=9.0.52
# Sat, 07 Aug 2021 01:44:58 GMT
ENV TOMCAT_SHA512=35e007e8e30e12889da27f9c71a6f4997b9cb5023b703d99add5de9271828e7d8d4956bf34dd2f48c7c71b4f8480f318c9067a4cd2a6d76eaae466286db4897b
# Sat, 07 Aug 2021 01:45:35 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Sat, 07 Aug 2021 01:45:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 07 Aug 2021 01:45:37 GMT
EXPOSE 8080
# Sat, 07 Aug 2021 01:45:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e15c6ae6a2da5e8cb8ab33e18689b49f48632e7708b344185ae04e707f9163`  
		Last Modified: Tue, 03 Aug 2021 00:10:50 GMT  
		Size: 159.9 MB (159941289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7c5726f4cba88825c1fd16f5b3499d74d67e826b4120ee505ba8a25a0f1582`  
		Last Modified: Tue, 03 Aug 2021 00:52:44 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5ee7827862e50fe8302edc80e3e2ab298f42df842221a56233776788c35149`  
		Last Modified: Sat, 07 Aug 2021 02:02:09 GMT  
		Size: 16.9 MB (16875347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63841dedaade5b6d55b64bcae76fe91a128adf51130ab2e2a62c667692016ffb`  
		Last Modified: Sat, 07 Aug 2021 02:02:07 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
