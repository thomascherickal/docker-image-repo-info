## `tomcat:9-jdk8-corretto-al2`

```console
$ docker pull tomcat@sha256:41ed8da708e62e6bae0ed2d8f0db8c9ad5cd152d53655d8b469a27c241ea4215
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk8-corretto-al2` - linux; amd64

```console
$ docker pull tomcat@sha256:42bb55a1a7578621e146aaaa0f17c79cff195d98288a4eebda4191abed66075d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.8 MB (154828924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a8b9a000246445a3bafb4fce81a74ec3f8fd378bde94133f2d1801799bbbcd`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 26 Jul 2023 19:20:31 GMT
COPY dir:eb203b2e14f406c161ffae3b2fa7ec59db3f5a04437b6e040395c2bc34835c5f in / 
# Wed, 26 Jul 2023 19:20:31 GMT
CMD ["/bin/bash"]
# Wed, 26 Jul 2023 20:12:48 GMT
ARG version=1.8.0_382.b05-1
# Wed, 26 Jul 2023 20:13:09 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 26 Jul 2023 20:13:10 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jul 2023 20:13:10 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 26 Jul 2023 21:04:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Jul 2023 21:04:51 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 21:04:52 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Jul 2023 21:04:52 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Jul 2023 21:04:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Jul 2023 21:04:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Jul 2023 21:04:52 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Jul 2023 21:04:52 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Jul 2023 21:04:52 GMT
ENV TOMCAT_VERSION=9.0.78
# Wed, 26 Jul 2023 21:04:52 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Wed, 26 Jul 2023 21:05:28 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 26 Jul 2023 21:05:29 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Jul 2023 21:05:29 GMT
EXPOSE 8080
# Wed, 26 Jul 2023 21:05:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a8d554425610d474f28e23ecfc3224dd78fca045a5c09515dbf51a8606c33d8f`  
		Last Modified: Tue, 25 Jul 2023 11:25:06 GMT  
		Size: 62.5 MB (62451920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2636316b868c613e3e0627c33426925c0ca079e846226d77acaea1b8cf2ba371`  
		Last Modified: Wed, 26 Jul 2023 20:24:44 GMT  
		Size: 75.6 MB (75553652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c75c391e7ca6806535ded0f18e0236b18eae2e810e79f3d6e2a917e8c7c765c`  
		Last Modified: Wed, 26 Jul 2023 21:12:33 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af6571d3b86875b836095534d7bc4f87fc8c36aeb00ff8930a9a42685137491`  
		Last Modified: Wed, 26 Jul 2023 21:12:35 GMT  
		Size: 16.8 MB (16823047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326d3420ca225e6289b8f3f93052d934e6c74ea50002aa20124557f107b9af0c`  
		Last Modified: Wed, 26 Jul 2023 21:12:33 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk8-corretto-al2` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:9eb832f96482e1b97399c0330487bccedfddc5ea495e62ecaa41b3c0227731e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140512194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de3a47f201bdbae6b8c83d054a95831539a716fee78d9bdf1ca6fb2d4021239`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:56 GMT
COPY dir:95dabd7a234aac70a826a1e3c0eafa3928b0be72717af1dea469f66b7db891d5 in / 
# Mon, 07 Aug 2023 19:40:57 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:21:31 GMT
ARG version=1.8.0_382.b05-1
# Mon, 07 Aug 2023 20:21:48 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 07 Aug 2023 20:21:49 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:21:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Mon, 07 Aug 2023 21:44:32 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Aug 2023 21:44:32 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 21:44:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Aug 2023 21:44:32 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Aug 2023 21:44:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Aug 2023 21:44:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Aug 2023 21:44:33 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Aug 2023 21:44:33 GMT
ENV TOMCAT_MAJOR=9
# Mon, 07 Aug 2023 21:44:33 GMT
ENV TOMCAT_VERSION=9.0.78
# Mon, 07 Aug 2023 21:44:33 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Mon, 07 Aug 2023 21:45:01 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Mon, 07 Aug 2023 21:45:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Aug 2023 21:45:02 GMT
EXPOSE 8080
# Mon, 07 Aug 2023 21:45:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3b5a1e75067e9d540ad8d844cad5a291a8cce89e1a3ed8e0f362a5736d3030c`  
		Last Modified: Wed, 02 Aug 2023 19:26:38 GMT  
		Size: 64.1 MB (64129548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbd1cb3365e06c166f4568a7f2334e62e5e58ba9fe399ffc875b4a390d9e0e1`  
		Last Modified: Mon, 07 Aug 2023 20:33:09 GMT  
		Size: 59.6 MB (59621903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7828233f6351a6186cc203393aa5d51ea37f516e671cd3f1c763af991ce65`  
		Last Modified: Mon, 07 Aug 2023 21:51:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6d26020c08e1f4c54ae72a259ab375fa831dd504c4123e7b33a666e56da022`  
		Last Modified: Mon, 07 Aug 2023 21:51:27 GMT  
		Size: 16.8 MB (16760438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45762a4adf588b688a28b0f90ef77cdfb5a5974c699a821e9aeba2c1305ba616`  
		Last Modified: Mon, 07 Aug 2023 21:51:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
