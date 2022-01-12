## `tomcat:10-jdk11-corretto`

```console
$ docker pull tomcat@sha256:4aea59f2fd575a890d5a93c30c69bef57a0fae9579a1a86246e8f6358b30e0e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jdk11-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:c97b20b3e358c0fb1a4fbe8d6b5efed41e5b96ac6ef1554b9fb31174f103d638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225728853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f94d6a4f7e2942f2da74d722351c5bfd4512563334aa3f795efe9231b4745aa`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 12 Jan 2022 02:20:04 GMT
ADD file:618cac8c5b6f6ff56ce221df12002d34997bcc996a0af3200b58db07d68be275 in / 
# Wed, 12 Jan 2022 02:20:04 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:40:24 GMT
ARG version=11.0.13.8-1
# Wed, 12 Jan 2022 02:40:45 GMT
# ARGS: version=11.0.13.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 12 Jan 2022 02:40:45 GMT
ENV LANG=C.UTF-8
# Wed, 12 Jan 2022 02:40:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 12 Jan 2022 03:08:49 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 12 Jan 2022 03:08:49 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Jan 2022 03:08:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 12 Jan 2022 03:08:50 GMT
WORKDIR /usr/local/tomcat
# Wed, 12 Jan 2022 03:08:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 12 Jan 2022 03:08:51 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 12 Jan 2022 03:08:51 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 12 Jan 2022 03:08:51 GMT
ENV TOMCAT_MAJOR=10
# Wed, 12 Jan 2022 03:11:13 GMT
ENV TOMCAT_VERSION=10.0.14
# Wed, 12 Jan 2022 03:11:13 GMT
ENV TOMCAT_SHA512=c2d2ad5ed17f7284e3aac5415774a8ef35434f14dbd9a87bc7230d8bfdbe9aa1258b97a59fa5c4030e4c973e4d93d29d20e40b6254347dbb66fae269ff4a61a5
# Wed, 12 Jan 2022 03:11:49 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 12 Jan 2022 03:11:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 12 Jan 2022 03:11:51 GMT
EXPOSE 8080
# Wed, 12 Jan 2022 03:11:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3a461b3ae562f8b6cf015b4c480a21b630a874f7fec851457680159226c81632`  
		Last Modified: Mon, 10 Jan 2022 23:29:44 GMT  
		Size: 62.2 MB (62212074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e03836ceba6f3c4f8dbad487f8ab31b2d002a01a6d813a4d718a4d66d70007b`  
		Last Modified: Wed, 12 Jan 2022 02:43:50 GMT  
		Size: 146.8 MB (146786722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9124bbfabdc5d72aefc6e89afbef5040d244c283f231fbc6d0ae4873d92c48`  
		Last Modified: Wed, 12 Jan 2022 03:33:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28cb1fb0a03d3509aba53ee90c716742d2a41cef1004a6cf4a38c24d6cead06`  
		Last Modified: Wed, 12 Jan 2022 03:35:25 GMT  
		Size: 16.7 MB (16729755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b99abb079a332a4372eacfb4588f16903f7db6677e6c61fece44b9e3897dee`  
		Last Modified: Wed, 12 Jan 2022 03:35:24 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk11-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:6eb316daab26bb426c01bd4f5c329e44bc77c0bf8aaee8ff0243e47c0499043e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.5 MB (224453720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65e61c23df5206d9e8555e120e98cbf88722fb9fa24061c82ae4fb9ad1416fec`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 12 Jan 2022 02:39:41 GMT
ADD file:afc90ca87d61fdaef5c9d192a5151ab745ac8b8ea4d7544c2dfdd66bdb3b7993 in / 
# Wed, 12 Jan 2022 02:39:43 GMT
CMD ["/bin/bash"]
# Wed, 12 Jan 2022 02:58:35 GMT
ARG version=11.0.13.8-1
# Wed, 12 Jan 2022 02:58:52 GMT
# ARGS: version=11.0.13.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 12 Jan 2022 02:58:53 GMT
ENV LANG=C.UTF-8
# Wed, 12 Jan 2022 02:58:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Wed, 12 Jan 2022 03:20:42 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 12 Jan 2022 03:20:42 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Jan 2022 03:20:43 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 12 Jan 2022 03:20:44 GMT
WORKDIR /usr/local/tomcat
# Wed, 12 Jan 2022 03:20:45 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 12 Jan 2022 03:20:46 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 12 Jan 2022 03:20:47 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 12 Jan 2022 03:20:48 GMT
ENV TOMCAT_MAJOR=10
# Wed, 12 Jan 2022 03:23:52 GMT
ENV TOMCAT_VERSION=10.0.14
# Wed, 12 Jan 2022 03:23:52 GMT
ENV TOMCAT_SHA512=c2d2ad5ed17f7284e3aac5415774a8ef35434f14dbd9a87bc7230d8bfdbe9aa1258b97a59fa5c4030e4c973e4d93d29d20e40b6254347dbb66fae269ff4a61a5
# Wed, 12 Jan 2022 03:24:11 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 12 Jan 2022 03:24:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 12 Jan 2022 03:24:13 GMT
EXPOSE 8080
# Wed, 12 Jan 2022 03:24:14 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b2e274b2b0f90c3d6329566163244a0f2e6d97e4c010c62133388ac89652105f`  
		Last Modified: Wed, 12 Jan 2022 02:41:56 GMT  
		Size: 63.8 MB (63836908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce9cb6ed9abd358bc46447abe7fb3a7ee2f8636cb224b8e3ee851fa0b84dfd6`  
		Last Modified: Wed, 12 Jan 2022 03:00:51 GMT  
		Size: 143.9 MB (143946652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234c4e8ef00595ae2ddca4afd1231e505029327b1364c7097ee8ac41e4bb9778`  
		Last Modified: Wed, 12 Jan 2022 03:54:05 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c3e397a3533d4fc2b6767a8e09af38000f85c58d62cf8649e20f39c6ed86b`  
		Last Modified: Wed, 12 Jan 2022 03:56:01 GMT  
		Size: 16.7 MB (16670021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
