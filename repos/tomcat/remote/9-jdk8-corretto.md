## `tomcat:9-jdk8-corretto`

```console
$ docker pull tomcat@sha256:8920f44e51fecf32d19e0acb8149ae9d5d38be9bca911fd16aa4e8df3a12c828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk8-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:9f3a4bf503a3622ac4593e3140e25737941c4aa1971fd4c9e3737be221ba39bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154293684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1076fb98fc3ac63970fe2ee141d751c955d1daeb93622b5c9ca8cddf07dd7479`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Nov 2022 01:32:34 GMT
ADD file:d5f7c1dc2e62cbd216adb0c4ff82770915f2b4e4660989515782faeca4e486ed in / 
# Thu, 17 Nov 2022 01:32:35 GMT
CMD ["/bin/bash"]
# Thu, 17 Nov 2022 01:49:48 GMT
ARG version=1.8.0_352.b08-1
# Thu, 17 Nov 2022 01:50:08 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 17 Nov 2022 01:50:09 GMT
ENV LANG=C.UTF-8
# Thu, 17 Nov 2022 01:50:09 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 17 Nov 2022 02:39:01 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 17 Nov 2022 02:39:02 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Nov 2022 02:39:02 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 17 Nov 2022 02:39:02 GMT
WORKDIR /usr/local/tomcat
# Thu, 17 Nov 2022 02:39:02 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:39:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:41:36 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 17 Nov 2022 02:41:36 GMT
ENV TOMCAT_MAJOR=9
# Mon, 05 Dec 2022 22:30:18 GMT
ENV TOMCAT_VERSION=9.0.70
# Mon, 05 Dec 2022 22:30:18 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Mon, 05 Dec 2022 22:30:52 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Mon, 05 Dec 2022 22:30:53 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 05 Dec 2022 22:30:54 GMT
EXPOSE 8080
# Mon, 05 Dec 2022 22:30:54 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:68028ec3b506bca4d81560b5fcbd408dc7cc49f4b1717a69d5396ff22700f80a`  
		Last Modified: Wed, 16 Nov 2022 20:32:28 GMT  
		Size: 62.3 MB (62262225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34cf93602c3cc903e430dc668610135919ed5282725f1e24640cf42482d35c0`  
		Last Modified: Thu, 17 Nov 2022 01:54:34 GMT  
		Size: 75.6 MB (75568468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2aa0ac6997762e3d8ed2c8bfa09cef7bcd83f2d956097b26c128ebf72ba7a`  
		Last Modified: Thu, 17 Nov 2022 02:50:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190be9c69a04bc08c7347deee2936cb9ccbecf34f654d91681a89529e8e65f53`  
		Last Modified: Mon, 05 Dec 2022 22:42:51 GMT  
		Size: 16.5 MB (16462687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e902d9c4e99761c52f8c10f912087a2b3486ed82c0c68eaeb9edbb1fce616aa9`  
		Last Modified: Mon, 05 Dec 2022 22:42:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk8-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:2d40f61ceaed2ca1fda2a7ec8dbe18a8cdfd327929581cf3b81d8e2212c11aa2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139843375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b727409c15f217ff3224fc3ec40c548b7a0a258397b22bbd1e556760f3a5e4a8`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Nov 2022 01:39:24 GMT
ADD file:ff78f504eef6d6952dca0350e26f9d78bcb442569cbd5a99bdc6206091485de4 in / 
# Thu, 17 Nov 2022 01:39:26 GMT
CMD ["/bin/bash"]
# Thu, 17 Nov 2022 01:56:04 GMT
ARG version=1.8.0_352.b08-1
# Thu, 17 Nov 2022 01:56:20 GMT
# ARGS: version=1.8.0_352.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 17 Nov 2022 01:56:21 GMT
ENV LANG=C.UTF-8
# Thu, 17 Nov 2022 01:56:21 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Thu, 17 Nov 2022 02:21:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 17 Nov 2022 02:21:24 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Nov 2022 02:21:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 17 Nov 2022 02:21:24 GMT
WORKDIR /usr/local/tomcat
# Thu, 17 Nov 2022 02:21:24 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:21:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:23:38 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 17 Nov 2022 02:23:38 GMT
ENV TOMCAT_MAJOR=9
# Mon, 05 Dec 2022 22:56:39 GMT
ENV TOMCAT_VERSION=9.0.70
# Mon, 05 Dec 2022 22:56:39 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Mon, 05 Dec 2022 22:57:04 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Mon, 05 Dec 2022 22:57:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 05 Dec 2022 22:57:06 GMT
EXPOSE 8080
# Mon, 05 Dec 2022 22:57:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4c4d0334d8224869629842fadc7a498ccbda1acc05e7995a0a7283b23fc39c24`  
		Last Modified: Wed, 16 Nov 2022 20:31:50 GMT  
		Size: 63.9 MB (63867424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe0acb86ae5726e590110068a908126dde5bd0fd831610cc698ee13dde7bac4`  
		Last Modified: Thu, 17 Nov 2022 01:58:33 GMT  
		Size: 59.6 MB (59581489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf323a5000b4d367f89ece869f39dc8f95f6a74b81842ee6c6c580d758a0151`  
		Last Modified: Thu, 17 Nov 2022 02:32:18 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888b8b8e51235b973caca75c7e3a22e4672331e87f774007eb89990810eede86`  
		Last Modified: Mon, 05 Dec 2022 23:09:30 GMT  
		Size: 16.4 MB (16394159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec061d6eb3ffa961f74f00b7b7eea8d010af15649398fc57b958c6cf105022fd`  
		Last Modified: Mon, 05 Dec 2022 23:09:28 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
