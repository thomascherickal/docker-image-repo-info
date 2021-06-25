## `tomcat:9-jdk16-corretto`

```console
$ docker pull tomcat@sha256:a8a8ca64b85d95960a9b0962abfa26e8ecbccd973bef8687e195c3320ff7bda1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk16-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:cf1e2d13f259b482f47927bf3cc55da9475b7fb1183cb58033566250cf628869
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.2 MB (237151656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:043b3813ba9a92550fcfc4bef3782c81c239d5e5eceed86a64cba697655423bf`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 25 Jun 2021 17:19:49 GMT
ADD file:dc851f79dbfc66e08196951041e8c856c41a3cc24b8bc27e66722210d51e87cf in / 
# Fri, 25 Jun 2021 17:19:50 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 18:03:23 GMT
ARG version=16.0.1.9-1
# Fri, 25 Jun 2021 18:03:49 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 25 Jun 2021 18:03:50 GMT
ENV LANG=C.UTF-8
# Fri, 25 Jun 2021 18:03:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
# Fri, 25 Jun 2021 18:27:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 25 Jun 2021 18:27:00 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Jun 2021 18:27:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 25 Jun 2021 18:27:01 GMT
WORKDIR /usr/local/tomcat
# Fri, 25 Jun 2021 18:27:02 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 25 Jun 2021 18:27:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 25 Jun 2021 18:30:04 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 25 Jun 2021 18:30:04 GMT
ENV TOMCAT_MAJOR=9
# Fri, 25 Jun 2021 18:30:04 GMT
ENV TOMCAT_VERSION=9.0.48
# Fri, 25 Jun 2021 18:30:04 GMT
ENV TOMCAT_SHA512=9fcde76bc192c5b02b467c7fc01727ec7c72acfc207741b03a582c67565218dd9b6ea9b9cf007b5964e7794f271433f66e3452b33352b9b657cd7e2bfff08f02
# Fri, 25 Jun 2021 18:30:42 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 25 Jun 2021 18:30:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 25 Jun 2021 18:30:44 GMT
EXPOSE 8080
# Fri, 25 Jun 2021 18:30:44 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:85ee02fe1a09b50ffaacc1e7482fdbb3e80c577256420503196fc549b9e4ef29`  
		Last Modified: Fri, 25 Jun 2021 00:50:03 GMT  
		Size: 61.9 MB (61940054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dde7853a8f5c521d4040f9c8bdbf3f9be05512892d0d5e4dfddf5f7e686e897`  
		Last Modified: Fri, 25 Jun 2021 18:05:44 GMT  
		Size: 159.9 MB (159941545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d93366861ba584df4c8a3edebecc068df69fe2d8f67e4240a3437fb6e45381`  
		Last Modified: Fri, 25 Jun 2021 18:43:13 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1193bf879e0f07fd26ebc3b295120973025c4f005130cee890a3946df883559c`  
		Last Modified: Fri, 25 Jun 2021 18:44:36 GMT  
		Size: 15.3 MB (15269751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dd7b2bce7f9e061f063d2bd75390ca03ee5cae3b81d936e6f76bf677d89e73`  
		Last Modified: Fri, 25 Jun 2021 18:44:33 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk16-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:ff918abbb2cc8a081f0e37211fcbf5743a6f30964bbde341c1953744c723da01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.8 MB (238750649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa3b69a9fcf7822e50157dfa3a67887b36710d15b127ca7fc5b3f3287ebfa3c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 25 Jun 2021 17:39:34 GMT
ADD file:d4d6f883cd1ba97522a617c6f7b0125b0a82e12101c702ca57ac48063f0e3707 in / 
# Fri, 25 Jun 2021 17:39:35 GMT
CMD ["/bin/bash"]
# Fri, 25 Jun 2021 17:57:49 GMT
ARG version=16.0.1.9-1
# Fri, 25 Jun 2021 17:58:13 GMT
# ARGS: version=16.0.1.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-16-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-16-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 25 Jun 2021 17:58:14 GMT
ENV LANG=C.UTF-8
# Fri, 25 Jun 2021 17:58:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-16-amazon-corretto
# Fri, 25 Jun 2021 18:16:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 25 Jun 2021 18:16:46 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Jun 2021 18:16:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 25 Jun 2021 18:16:47 GMT
WORKDIR /usr/local/tomcat
# Fri, 25 Jun 2021 18:16:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 25 Jun 2021 18:16:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 25 Jun 2021 18:20:20 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 25 Jun 2021 18:20:20 GMT
ENV TOMCAT_MAJOR=9
# Fri, 25 Jun 2021 18:20:21 GMT
ENV TOMCAT_VERSION=9.0.48
# Fri, 25 Jun 2021 18:20:21 GMT
ENV TOMCAT_SHA512=9fcde76bc192c5b02b467c7fc01727ec7c72acfc207741b03a582c67565218dd9b6ea9b9cf007b5964e7794f271433f66e3452b33352b9b657cd7e2bfff08f02
# Fri, 25 Jun 2021 18:20:55 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 25 Jun 2021 18:20:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 25 Jun 2021 18:20:57 GMT
EXPOSE 8080
# Fri, 25 Jun 2021 18:20:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b19e557e673ca4274c5ee576b0d897c535e4329a596ac20b3ff70225b734a125`  
		Last Modified: Fri, 25 Jun 2021 00:50:31 GMT  
		Size: 63.6 MB (63564395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c876d030feee18055fe588ade3e5438a15da1781912846f82ca1e19feb62474b`  
		Last Modified: Fri, 25 Jun 2021 18:00:29 GMT  
		Size: 159.9 MB (159915246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ea33a5ad74ddb451e8dfe791576b73a97b93327783eb30e784ca793fddbaf`  
		Last Modified: Fri, 25 Jun 2021 18:36:09 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821d7d3b3a762e8c8239683b3db82fd04fedb4d2b56977b84d15873d71c48bda`  
		Last Modified: Fri, 25 Jun 2021 18:37:53 GMT  
		Size: 15.3 MB (15270706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23740a61acb27efd14c85fb42d00fc3b51ea482f5459a3b9bfbd18bc746a534`  
		Last Modified: Fri, 25 Jun 2021 18:37:50 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
