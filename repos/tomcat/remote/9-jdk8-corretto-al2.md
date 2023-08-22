## `tomcat:9-jdk8-corretto-al2`

```console
$ docker pull tomcat@sha256:bbdd42aba0d3599d1c2e8774a925dde010542f7c2bfea07c7cd4809edb4a1800
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk8-corretto-al2` - linux; amd64

```console
$ docker pull tomcat@sha256:c8a28d471d1ecc5b87fa21c161ea3f80ee9e4c3951e469c0891c2681d93cd86f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154930011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4fe4d5a475638837ec5a1ee1a580c3095fd69fa8931192b6e3c377f724dbb5`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:52 GMT
COPY dir:74433340f66bb20aa9bebf7ee91eaada91d987f210fbb253d98f2ee60012726f in / 
# Tue, 22 Aug 2023 20:19:52 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:25:20 GMT
ARG version=1.8.0_382.b05-1
# Tue, 22 Aug 2023 21:25:41 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 22 Aug 2023 21:25:41 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:25:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 22 Aug 2023 22:33:03 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 22 Aug 2023 22:33:03 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Aug 2023 22:33:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 22 Aug 2023 22:33:03 GMT
WORKDIR /usr/local/tomcat
# Tue, 22 Aug 2023 22:33:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 22:33:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 22:33:03 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 22 Aug 2023 22:33:04 GMT
ENV TOMCAT_MAJOR=9
# Tue, 22 Aug 2023 22:33:04 GMT
ENV TOMCAT_VERSION=9.0.79
# Tue, 22 Aug 2023 22:33:04 GMT
ENV TOMCAT_SHA512=7a0d99b5fc37c9e9ac26b554fab9147ce0a2ba59fad41e2565b15e9f6e137bf0105f5c9cd6b7b508837ff24feb7b95b2aba49e0abc7b1480a30a11606e79802a
# Tue, 22 Aug 2023 22:33:39 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Tue, 22 Aug 2023 22:33:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Aug 2023 22:33:40 GMT
EXPOSE 8080
# Tue, 22 Aug 2023 22:33:40 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:8cd2389cb7276ab6d8d1154ee827bc715858f6827bdde1e9b5499a2eb3b76dc4`  
		Last Modified: Wed, 16 Aug 2023 14:05:30 GMT  
		Size: 62.5 MB (62492616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23ce1ce76a8e2b1c8c2610954ecb0d81269c24a4043c91b054756a8fddc113f`  
		Last Modified: Tue, 22 Aug 2023 21:37:35 GMT  
		Size: 75.6 MB (75596009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a0a3cf6595342163a98cf48e0240d155b4b7a647b980d2c28a7967a08404ab`  
		Last Modified: Tue, 22 Aug 2023 22:39:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb53b1ebfb347005348327901dd80b856758ec8ff98e40f269229e7f43ec1bf3`  
		Last Modified: Tue, 22 Aug 2023 22:39:42 GMT  
		Size: 16.8 MB (16841081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f468f23f6f19fd5907db840d0b870413111c5033d31010ea61267a9777411308`  
		Last Modified: Tue, 22 Aug 2023 22:39:40 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk8-corretto-al2` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:8b11d50fa67924157ad78badb7318392f2b1d5130cf542399f76933c12c164e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140529074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d259a5ca708daa2eb4679a61725732bafad1e3bf1d7b5fa007e0e2b4630da0c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:53 GMT
COPY dir:e20aef745ed6033815440b78b98680b9989b365a1e5e12e6f94169e6de7e94c3 in / 
# Tue, 22 Aug 2023 19:39:54 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:06:27 GMT
ARG version=1.8.0_382.b05-1
# Tue, 22 Aug 2023 21:06:44 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 22 Aug 2023 21:06:45 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:06:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 22 Aug 2023 21:46:49 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 22 Aug 2023 21:46:49 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Aug 2023 21:46:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 22 Aug 2023 21:46:50 GMT
WORKDIR /usr/local/tomcat
# Tue, 22 Aug 2023 21:46:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 21:46:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 21:46:50 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 22 Aug 2023 21:46:50 GMT
ENV TOMCAT_MAJOR=9
# Tue, 22 Aug 2023 21:46:50 GMT
ENV TOMCAT_VERSION=9.0.79
# Tue, 22 Aug 2023 21:46:50 GMT
ENV TOMCAT_SHA512=7a0d99b5fc37c9e9ac26b554fab9147ce0a2ba59fad41e2565b15e9f6e137bf0105f5c9cd6b7b508837ff24feb7b95b2aba49e0abc7b1480a30a11606e79802a
# Tue, 22 Aug 2023 21:47:18 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Tue, 22 Aug 2023 21:47:19 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Aug 2023 21:47:19 GMT
EXPOSE 8080
# Tue, 22 Aug 2023 21:47:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3e86c88b00180fc8094116a7111cfe1c0e88e04a6c513618fbde52ee5d97a51a`  
		Last Modified: Wed, 16 Aug 2023 18:15:18 GMT  
		Size: 64.1 MB (64127623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98935d9922b7094d86020761e111996454d12c4520b10dd7b9fcac792eaa8d3`  
		Last Modified: Tue, 22 Aug 2023 21:15:44 GMT  
		Size: 59.6 MB (59621381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dae355bc297fd1a72160164412cd141f4bac74d8338b084c165605691bd92da`  
		Last Modified: Tue, 22 Aug 2023 21:52:39 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb19c3fe2f8b92d127f2ce07893c22a907adbf1f7ceb422bf9e367542416c662`  
		Last Modified: Tue, 22 Aug 2023 21:52:41 GMT  
		Size: 16.8 MB (16779765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196b7ef202a8fc260d21f88f42f90e5b68d5c5a3564f24c633ba2e79d58aecca`  
		Last Modified: Tue, 22 Aug 2023 21:52:39 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
