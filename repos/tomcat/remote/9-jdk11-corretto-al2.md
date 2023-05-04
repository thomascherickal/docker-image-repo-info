## `tomcat:9-jdk11-corretto-al2`

```console
$ docker pull tomcat@sha256:8cf6161e9e4f737a11dcf5fb381865e92f3dee493750e6b03dde7ecac2c7fe1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk11-corretto-al2` - linux; amd64

```console
$ docker pull tomcat@sha256:27c38137b21971479cd0cd77fe10626149f923c39d3dbb1d7df0f217517e8bdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.9 MB (227905589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560ea2075cc8f10e47587cf1ef50e24b7ff4b7f75e5364bfd5afc6cf133f2b6f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 04 May 2023 19:20:10 GMT
COPY dir:e8a4b2d0bb4f52911c2b1115b27842bc606a63bd56c8563ded4e6b898fe187d1 in / 
# Thu, 04 May 2023 19:20:10 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 19:39:07 GMT
ARG version=11.0.19.7-1
# Thu, 04 May 2023 19:39:31 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 04 May 2023 19:39:31 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 19:39:32 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 04 May 2023 20:32:04 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 04 May 2023 20:32:04 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 20:32:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 04 May 2023 20:32:05 GMT
WORKDIR /usr/local/tomcat
# Thu, 04 May 2023 20:32:05 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 20:32:05 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 20:32:05 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 04 May 2023 20:32:05 GMT
ENV TOMCAT_MAJOR=9
# Thu, 04 May 2023 20:32:05 GMT
ENV TOMCAT_VERSION=9.0.74
# Thu, 04 May 2023 20:32:05 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Thu, 04 May 2023 20:32:46 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Thu, 04 May 2023 20:32:48 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 04 May 2023 20:32:48 GMT
EXPOSE 8080
# Thu, 04 May 2023 20:32:48 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7cbd40bc2978b9c91c4cf0a5064302062d07242909f83ad9d8d7e2a2d379cf03`  
		Last Modified: Tue, 25 Apr 2023 00:08:27 GMT  
		Size: 62.5 MB (62512332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cba9a7b3f80b34f78a02e3b4893afa6a121c457d71db0cb2fe82057f656d538`  
		Last Modified: Thu, 04 May 2023 19:45:03 GMT  
		Size: 147.8 MB (147808136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1652bad230403f393b246985410c7f0d59271abb6100d8e38d2e0fe633fb988f`  
		Last Modified: Thu, 04 May 2023 20:38:36 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b81cf10dd36d069e97ae5c9306f0817d8530cb3567abceab6c6c1c92be3ebb`  
		Last Modified: Thu, 04 May 2023 20:38:38 GMT  
		Size: 17.6 MB (17584821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22be9cf9bd80fd215e5897294e637b3864b7cfc2dbf7a87bb3a5f2801cde48f`  
		Last Modified: Thu, 04 May 2023 20:38:36 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk11-corretto-al2` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:476029ec1992ff27ceffecc1949031f122a7f3c535f83cee026d8524780e1f96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234511910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05131baf48af9d351a01c36d14621658c4333c4a786cde4ef219899a0f2536d3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 28 Mar 2023 18:40:10 GMT
COPY dir:1d0df99dbb2a961dca382ec30c27f40e06635a9186a0715c0d2a629262a04288 in / 
# Tue, 28 Mar 2023 18:40:10 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 17:40:45 GMT
ARG version=11.0.19.7-1
# Thu, 20 Apr 2023 17:41:07 GMT
# ARGS: version=11.0.19.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Apr 2023 17:41:08 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:41:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Thu, 20 Apr 2023 18:23:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 20 Apr 2023 18:23:05 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Apr 2023 18:23:06 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 20 Apr 2023 18:23:06 GMT
WORKDIR /usr/local/tomcat
# Thu, 20 Apr 2023 18:23:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 20 Apr 2023 18:23:06 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 20 Apr 2023 18:23:06 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 20 Apr 2023 18:23:06 GMT
ENV TOMCAT_MAJOR=9
# Thu, 20 Apr 2023 18:23:06 GMT
ENV TOMCAT_VERSION=9.0.74
# Thu, 20 Apr 2023 18:23:06 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Wed, 03 May 2023 10:35:20 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 03 May 2023 10:35:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 03 May 2023 10:35:22 GMT
EXPOSE 8080
# Wed, 03 May 2023 10:35:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:949542da27c3c0ab979766d37f455344960f838d9f661b9db50bec634ca7149e`  
		Last Modified: Thu, 23 Mar 2023 21:25:53 GMT  
		Size: 64.1 MB (64126936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc8a98f0e7be7c6120b0be56d2c543357756e751174d0d3d40efee7e82d0527`  
		Last Modified: Thu, 20 Apr 2023 17:50:08 GMT  
		Size: 145.0 MB (144951504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c628b01b8e4a4d3655cdbb866ca7ccb2a32ac3c058d405f56c0594b3be20ac`  
		Last Modified: Thu, 20 Apr 2023 18:29:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678f827795c626b1c8b5148853c4980ecdb037b14e7368e6caee39921d01083c`  
		Last Modified: Wed, 03 May 2023 10:50:08 GMT  
		Size: 25.4 MB (25433166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3bdc5a52bb337bb1aaed7e490ba9d2bdff0909e36795682f2c943009f59f14`  
		Last Modified: Wed, 03 May 2023 10:50:06 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
