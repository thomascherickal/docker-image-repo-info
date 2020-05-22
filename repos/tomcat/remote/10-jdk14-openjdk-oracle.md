## `tomcat:10-jdk14-openjdk-oracle`

```console
$ docker pull tomcat@sha256:55527f6a53b425b3b9acbebcd967cd75049c7fdf09c44b17186240d2990d7624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `tomcat:10-jdk14-openjdk-oracle` - linux; amd64

```console
$ docker pull tomcat@sha256:7d9b58edb01542510a103f77a674e717786745a7d70232a7d856cbe7d684c03a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.2 MB (274200072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd4e67dcc09a94c6a655388868e8303e59354e38bb658961aa0f3d15227577b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 04 May 2020 20:20:53 GMT
ADD file:d23891d2372d6aae3d738388c74dacd92f9406083ee0c1ac0e2bfd140f92ec2b in / 
# Mon, 04 May 2020 20:20:53 GMT
CMD ["/bin/bash"]
# Mon, 04 May 2020 20:38:21 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Mon, 04 May 2020 20:38:21 GMT
ENV LANG=en_US.UTF-8
# Mon, 04 May 2020 20:39:15 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Mon, 04 May 2020 20:39:15 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 May 2020 20:39:15 GMT
ENV JAVA_VERSION=14.0.1
# Fri, 22 May 2020 01:23:50 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_linux-x64_bin.tar.gz; 			downloadSha256=22ce248e0bd69f23028625bede9d1b3080935b68d011eaaf9e241f84d6b9c4cc; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 22 May 2020 01:23:50 GMT
CMD ["jshell"]
# Fri, 22 May 2020 02:26:15 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 22 May 2020 02:26:15 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 May 2020 02:26:16 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 22 May 2020 02:26:16 GMT
WORKDIR /usr/local/tomcat
# Fri, 22 May 2020 02:26:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 22 May 2020 02:26:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 22 May 2020 02:26:17 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 22 May 2020 02:26:17 GMT
ENV TOMCAT_MAJOR=10
# Fri, 22 May 2020 02:26:17 GMT
ENV TOMCAT_VERSION=10.0.0-M5
# Fri, 22 May 2020 02:26:18 GMT
ENV TOMCAT_SHA512=09d6d4c084857d3a7846fdb4ed562ef49402a164dbd140636a7d8fe1370f902f56144d8a20cc71b698189b873ce38cec2a12c38abedb6d7173b091eb46ea26a9
# Fri, 22 May 2020 02:27:18 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| sort -u 			| xargs -r rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 22 May 2020 02:27:20 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 May 2020 02:27:20 GMT
EXPOSE 8080
# Fri, 22 May 2020 02:27:20 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:83755823a002357171a0b229ef5769a60db47a90b624adc45f8c6b7cd1d1394f`  
		Last Modified: Mon, 04 May 2020 20:22:07 GMT  
		Size: 43.5 MB (43455265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e105caaf23acf967db67aa1f683d428603dbb51e12295bfe8f5df6a4cce8bb`  
		Last Modified: Mon, 04 May 2020 20:40:58 GMT  
		Size: 14.8 MB (14758294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aaeeabaf683143583aa9a565869c92a82fed3ae1a7e6daf3f81cc9f1d123e9`  
		Last Modified: Fri, 22 May 2020 01:27:57 GMT  
		Size: 199.2 MB (199224597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db1f7bfdcefe02fe249d232d453ea5cc73813e83533767e3aecad43e5d5c240`  
		Last Modified: Fri, 22 May 2020 02:36:36 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d443ce9e772ad362550fde96366f63284f912cc9117a0f52248fbdc4ba015bbc`  
		Last Modified: Fri, 22 May 2020 02:36:38 GMT  
		Size: 16.8 MB (16761647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1661d2bdd75ffa749e9ca6f23cb89095bc23130c1f268f2de6db675b01060d31`  
		Last Modified: Fri, 22 May 2020 02:36:36 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
