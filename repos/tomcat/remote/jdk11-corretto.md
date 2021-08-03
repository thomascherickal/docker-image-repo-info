## `tomcat:jdk11-corretto`

```console
$ docker pull tomcat@sha256:50dcd35d5d05df8e402db1357bb5f16b6e17d944a47f715d81630f1328561475
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:jdk11-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:c03980948eb39af6acf728f1c4846d6385a9f4ae49754427a9715b485c2bd852
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.6 MB (225613011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e91075b1e6161fc3d332997602f8d81ef25aeb952232ec308b7e0a4405ac963c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 02 Aug 2021 23:19:37 GMT
ADD file:4cbe5850096b1ae39fe377dfe25245d1d635eafcbe0f58e1dc20e75716131cd3 in / 
# Mon, 02 Aug 2021 23:19:38 GMT
CMD ["/bin/bash"]
# Tue, 03 Aug 2021 00:04:41 GMT
ARG version=11.0.12.7-1
# Tue, 03 Aug 2021 00:05:03 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 03 Aug 2021 00:05:03 GMT
ENV LANG=C.UTF-8
# Tue, 03 Aug 2021 00:05:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 03 Aug 2021 00:24:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Aug 2021 00:24:31 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Aug 2021 00:24:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Aug 2021 00:24:32 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Aug 2021 00:24:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:24:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:27:29 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 03 Aug 2021 00:27:29 GMT
ENV TOMCAT_MAJOR=9
# Tue, 03 Aug 2021 00:27:29 GMT
ENV TOMCAT_VERSION=9.0.50
# Tue, 03 Aug 2021 00:27:30 GMT
ENV TOMCAT_SHA512=06cd51abbeebba9385f594ed092bd30e510b6314c90c421f4be5d8bec596c6a177785efc2ce27363813f6822af89fc88a2072d7b051960e5387130faf69c447b
# Tue, 03 Aug 2021 00:28:06 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Tue, 03 Aug 2021 00:28:07 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 03 Aug 2021 00:28:08 GMT
EXPOSE 8080
# Tue, 03 Aug 2021 00:28:08 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d36ac8072fa22f99e1b8c66984e2fa09296890d37276e65dd4dc83503a3cf4c2`  
		Last Modified: Fri, 30 Jul 2021 16:48:36 GMT  
		Size: 62.0 MB (61965674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f170fe744cfdd69b498f626d42da3fa5b31e4e88b3c49ee2ea881f4025eee5ad`  
		Last Modified: Tue, 03 Aug 2021 00:06:55 GMT  
		Size: 146.8 MB (146777358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c51b44415ac9de22bd5016c958f444dba8a52732d9c460f407ed0ab4ce4669e`  
		Last Modified: Tue, 03 Aug 2021 00:36:03 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c906ebd88a65d756b4fbaf1b8376944ea1faa702adb3d5212c456d9c82a59c`  
		Last Modified: Tue, 03 Aug 2021 00:37:23 GMT  
		Size: 16.9 MB (16869674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e67cdc0e4ce34294644181a2df9b3b84e90fee89eb7601eca1c2bda1a56c8d4`  
		Last Modified: Tue, 03 Aug 2021 00:37:20 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jdk11-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:a46c95f1efd5518a1d7b0758f4386689d663601d0a1c79e14dabb34257741f27
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224329140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9d54cd2b501f7ebcecd7c25fce9fac94dba02caff7932a40774c2755169ea3e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 02 Aug 2021 23:39:27 GMT
ADD file:d3c0f2c17135c35c4fec5abfa25c0f77c04517a31107e754d182e5985e962fbe in / 
# Mon, 02 Aug 2021 23:39:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Aug 2021 00:07:57 GMT
ARG version=11.0.12.7-1
# Tue, 03 Aug 2021 00:08:15 GMT
# ARGS: version=11.0.12.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 03 Aug 2021 00:08:16 GMT
ENV LANG=C.UTF-8
# Tue, 03 Aug 2021 00:08:16 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 03 Aug 2021 00:36:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 03 Aug 2021 00:36:19 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Aug 2021 00:36:20 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 03 Aug 2021 00:36:20 GMT
WORKDIR /usr/local/tomcat
# Tue, 03 Aug 2021 00:36:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:36:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 03 Aug 2021 00:39:57 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 03 Aug 2021 00:39:57 GMT
ENV TOMCAT_MAJOR=9
# Tue, 03 Aug 2021 00:39:57 GMT
ENV TOMCAT_VERSION=9.0.50
# Tue, 03 Aug 2021 00:39:57 GMT
ENV TOMCAT_SHA512=06cd51abbeebba9385f594ed092bd30e510b6314c90c421f4be5d8bec596c6a177785efc2ce27363813f6822af89fc88a2072d7b051960e5387130faf69c447b
# Tue, 03 Aug 2021 00:40:30 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Tue, 03 Aug 2021 00:40:31 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 03 Aug 2021 00:40:31 GMT
EXPOSE 8080
# Tue, 03 Aug 2021 00:40:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:63f4e95aab55922b1bd380df3233d11cc34653d71768884de620d921e24daf17`  
		Last Modified: Mon, 02 Aug 2021 23:40:24 GMT  
		Size: 63.5 MB (63546854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8b16728471d5d9ac7f454dcd3043e891b79ff4ad587d6f92b86edd9b49b1e8`  
		Last Modified: Tue, 03 Aug 2021 00:10:12 GMT  
		Size: 143.9 MB (143933602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91cfc76c25b9446ae4ea05f306cecb92fec00908e434efcef5eebe5f14c446a`  
		Last Modified: Tue, 03 Aug 2021 00:53:17 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f27e7b7a78bfa6b2fbac6c4106b65e552f8f6e8b3f068e6f468ef2a7eb3c786`  
		Last Modified: Tue, 03 Aug 2021 00:55:05 GMT  
		Size: 16.8 MB (16848380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95893114697a9a9aa0caf70586fec05690828cf7ce917fd7d2816723a59a70b3`  
		Last Modified: Tue, 03 Aug 2021 00:55:03 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
