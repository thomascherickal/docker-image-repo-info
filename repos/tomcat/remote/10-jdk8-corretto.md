## `tomcat:10-jdk8-corretto`

```console
$ docker pull tomcat@sha256:afd0b28af39ee65e491571f28bfeb0c868ef59daf08a1783429db9f0c203a7d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jdk8-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:0472dfc5991133dc2744024981ec73d4d2cb153a7b050c90bdd0f6f967107995
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154551071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db5ebdb0408e02bbac326f422febd66ed8794fef6c8ab549528eb5b64305bca`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Mar 2022 04:17:58 GMT
ADD file:6e25b6e9b3976f8d699ddf69117d5af30565798c52f777c8b4b99e38aca8523f in / 
# Fri, 04 Mar 2022 04:17:59 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 04:35:57 GMT
ARG version=1.8.0_322.b06-2
# Fri, 04 Mar 2022 04:36:22 GMT
# ARGS: version=1.8.0_322.b06-2
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 04 Mar 2022 04:36:22 GMT
ENV LANG=C.UTF-8
# Fri, 04 Mar 2022 04:36:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 04 Mar 2022 06:58:11 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 06:58:11 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 06:58:11 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 06:58:11 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 06:58:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 06:58:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 06:58:12 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 06:58:12 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 06:58:12 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 06:58:12 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 06:59:25 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 04 Mar 2022 06:59:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 06:59:26 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 06:59:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:bda57ff2d0d885374555b8bf3f1aaa48d5f044446a24a98acedbef6acc0b727e`  
		Last Modified: Thu, 03 Mar 2022 02:21:35 GMT  
		Size: 62.2 MB (62239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f4f62799c66b6f786072457b9a5aff0f3ad7aae2dc133eb97c440b632897df`  
		Last Modified: Fri, 04 Mar 2022 04:39:22 GMT  
		Size: 75.6 MB (75558079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb53552df04f9f3c78d9cf8f8774670159452c166be4c936e0aa184e6b3457b6`  
		Last Modified: Fri, 04 Mar 2022 07:29:41 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f44cc57d820a5406afb6cca60e2ebe4302c43f557a18fe1e08b2899be3c2f1b`  
		Last Modified: Fri, 04 Mar 2022 07:29:42 GMT  
		Size: 16.8 MB (16753393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693eaffd8ef6119c851b8966e23ab9b06a9d3781243a8b4695c4084d79a12c32`  
		Last Modified: Fri, 04 Mar 2022 07:29:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk8-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:ff381b75730306dd73b7a73436f46de6b98bbf108a2f3ff91de155b9790e9451
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140042026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b38b39deea24aee0962cf8802812c316f431b5f217692da2760ba819bd35c60`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Mar 2022 02:54:31 GMT
ADD file:d8fe7ad66f762a8aad81401877fc5d61f1a4b58eac91f47145e6e443aa3ac8ee in / 
# Fri, 04 Mar 2022 02:54:32 GMT
CMD ["/bin/bash"]
# Fri, 04 Mar 2022 03:11:59 GMT
ARG version=1.8.0_322.b06-2
# Fri, 04 Mar 2022 03:12:13 GMT
# ARGS: version=1.8.0_322.b06-2
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 04 Mar 2022 03:12:14 GMT
ENV LANG=C.UTF-8
# Fri, 04 Mar 2022 03:12:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 04 Mar 2022 03:48:15 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Mar 2022 03:48:15 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Mar 2022 03:48:16 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Mar 2022 03:48:17 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Mar 2022 03:48:18 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 03:48:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Mar 2022 03:48:20 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 04 Mar 2022 03:48:21 GMT
ENV TOMCAT_MAJOR=10
# Fri, 04 Mar 2022 03:48:22 GMT
ENV TOMCAT_VERSION=10.0.17
# Fri, 04 Mar 2022 03:48:23 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Fri, 04 Mar 2022 03:48:59 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 04 Mar 2022 03:49:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 04 Mar 2022 03:49:01 GMT
EXPOSE 8080
# Fri, 04 Mar 2022 03:49:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:12990ee66856745f12f3a508d82e3d48a09d0378d91aaca8ca153c3819e7a686`  
		Last Modified: Thu, 03 Mar 2022 02:21:31 GMT  
		Size: 63.8 MB (63816961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cffc695980b09d73a5662cf1b4d59cc6d5b3870797b1dd748a4eba8182e5b9`  
		Last Modified: Fri, 04 Mar 2022 03:13:52 GMT  
		Size: 59.6 MB (59550934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f81ad39953d89e3df52186cf1f73a946f02004694c3328887b97559a52474c`  
		Last Modified: Fri, 04 Mar 2022 06:02:51 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ee8995b26891b52fd3c85eab16593eaaf0a835940eb98a0094a94597e12454`  
		Last Modified: Fri, 04 Mar 2022 06:02:54 GMT  
		Size: 16.7 MB (16673993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
