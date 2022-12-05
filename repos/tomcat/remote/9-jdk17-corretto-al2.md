## `tomcat:9-jdk17-corretto-al2`

```console
$ docker pull tomcat@sha256:91a238980406ecb1263efcdba63eeccd9afed081355c697c581018a66ed01a50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk17-corretto-al2` - linux; amd64

```console
$ docker pull tomcat@sha256:da58214eb37f60840fe8bfc839fff63e0fbd3200ba02027f6e16a35cd94ea573
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.6 MB (230645037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab236c607b71f06c596bcfb3a6e32159bb5bfc542553d03be0b98a936a33aba6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Nov 2022 01:32:34 GMT
ADD file:d5f7c1dc2e62cbd216adb0c4ff82770915f2b4e4660989515782faeca4e486ed in / 
# Thu, 17 Nov 2022 01:32:35 GMT
CMD ["/bin/bash"]
# Thu, 17 Nov 2022 01:51:16 GMT
ARG version=17.0.5.8-1
# Thu, 17 Nov 2022 01:51:40 GMT
# ARGS: version=17.0.5.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 17 Nov 2022 01:51:41 GMT
ENV LANG=C.UTF-8
# Thu, 17 Nov 2022 01:51:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 17 Nov 2022 02:37:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 17 Nov 2022 02:37:21 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Nov 2022 02:37:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 17 Nov 2022 02:37:22 GMT
WORKDIR /usr/local/tomcat
# Thu, 17 Nov 2022 02:37:22 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:37:22 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:39:53 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 17 Nov 2022 02:39:53 GMT
ENV TOMCAT_MAJOR=9
# Mon, 05 Dec 2022 22:25:25 GMT
ENV TOMCAT_VERSION=9.0.70
# Mon, 05 Dec 2022 22:25:25 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Mon, 05 Dec 2022 22:26:00 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Mon, 05 Dec 2022 22:26:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 05 Dec 2022 22:26:02 GMT
EXPOSE 8080
# Mon, 05 Dec 2022 22:26:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:68028ec3b506bca4d81560b5fcbd408dc7cc49f4b1717a69d5396ff22700f80a`  
		Last Modified: Wed, 16 Nov 2022 20:32:28 GMT  
		Size: 62.3 MB (62262225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d137d23130653f2307ef578a322d90337873796341997aae991c075dac9870e8`  
		Last Modified: Thu, 17 Nov 2022 01:56:06 GMT  
		Size: 151.9 MB (151923805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64cc5c129336fc766adc2c7ba8fe647267d7b5a0ab4ea5c5090c389ff1e9f561`  
		Last Modified: Thu, 17 Nov 2022 02:49:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9158d7d07c253b1c9e4ea6962a15f90ef519f6a712da2054c1f9e98e5bd8f0e`  
		Last Modified: Mon, 05 Dec 2022 22:39:53 GMT  
		Size: 16.5 MB (16458703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb87dfde0d1279cf243f51e75d436af34d2ecf3753ebf3605301e2d1581ad35`  
		Last Modified: Mon, 05 Dec 2022 22:39:52 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk17-corretto-al2` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:013cc6adc55aa806052a1ab52bc8f839eddd1b771a60d38c7a3cdb07d14d6482
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.7 MB (230684316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d1274ca02b2f0482a4795913ba162f1e4318ca3677d8b6615857f28c3e5cc7d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Nov 2022 01:39:24 GMT
ADD file:ff78f504eef6d6952dca0350e26f9d78bcb442569cbd5a99bdc6206091485de4 in / 
# Thu, 17 Nov 2022 01:39:26 GMT
CMD ["/bin/bash"]
# Thu, 17 Nov 2022 01:56:55 GMT
ARG version=17.0.5.8-1
# Thu, 17 Nov 2022 01:57:13 GMT
# ARGS: version=17.0.5.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 17 Nov 2022 01:57:15 GMT
ENV LANG=C.UTF-8
# Thu, 17 Nov 2022 01:57:15 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 17 Nov 2022 02:19:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 17 Nov 2022 02:19:58 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Nov 2022 02:19:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 17 Nov 2022 02:19:58 GMT
WORKDIR /usr/local/tomcat
# Thu, 17 Nov 2022 02:19:59 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:19:59 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 17 Nov 2022 02:22:09 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 17 Nov 2022 02:22:09 GMT
ENV TOMCAT_MAJOR=9
# Mon, 05 Dec 2022 22:52:54 GMT
ENV TOMCAT_VERSION=9.0.70
# Mon, 05 Dec 2022 22:52:54 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Mon, 05 Dec 2022 22:53:20 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Mon, 05 Dec 2022 22:53:22 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 05 Dec 2022 22:53:22 GMT
EXPOSE 8080
# Mon, 05 Dec 2022 22:53:22 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4c4d0334d8224869629842fadc7a498ccbda1acc05e7995a0a7283b23fc39c24`  
		Last Modified: Wed, 16 Nov 2022 20:31:50 GMT  
		Size: 63.9 MB (63867424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7091ff225e6d0e6fff53ebbea228516d68e22d6469aee982ce7e63865a618606`  
		Last Modified: Thu, 17 Nov 2022 01:59:33 GMT  
		Size: 150.4 MB (150442128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf363273182c6b3ffd8897a60d0da255501e1b7f0961cc4d834abde967f18ec`  
		Last Modified: Thu, 17 Nov 2022 02:31:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6a4015c9b35ead89ad3ae2eb987d3ac9ec716a7d75c64e690cb7e24b23c2de`  
		Last Modified: Mon, 05 Dec 2022 23:06:28 GMT  
		Size: 16.4 MB (16374463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecb0d18a613322f2c1f1ac13b4381aa1f91720dd5849baca893140cf301bae0`  
		Last Modified: Mon, 05 Dec 2022 23:06:26 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
