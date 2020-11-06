## `tomcat:9-jdk8-corretto`

```console
$ docker pull tomcat@sha256:90ee2cddcb6b3005b9c93b636c42884ff8c22b87134dc4215c7f560bd6a25cf3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk8-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:6bc8eae96809bd57d574aa123c8833c6d6b61e85ec42656ba4b071b98367b3e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (161039935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59529339b5fba045671d30a4ab906fca296c81559d2eccbdf72f86e5df16b67f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:19:28 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:19:52 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:19:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:19:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 28 Oct 2020 00:57:28 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 28 Oct 2020 00:57:28 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 00:57:30 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 28 Oct 2020 00:57:30 GMT
WORKDIR /usr/local/tomcat
# Wed, 28 Oct 2020 00:57:31 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 28 Oct 2020 00:57:31 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 28 Oct 2020 01:02:02 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 28 Oct 2020 01:02:02 GMT
ENV TOMCAT_MAJOR=9
# Wed, 28 Oct 2020 01:02:03 GMT
ENV TOMCAT_VERSION=9.0.39
# Wed, 28 Oct 2020 01:02:03 GMT
ENV TOMCAT_SHA512=307ca646bac267e529fb0862278f7133fe80813f0af64a44aed949f4c7a9a98aeb9bd7f08b087645b40c6fefdd3a7fe519e4858a3dbf0a19c38c53704f92b575
# Fri, 06 Nov 2020 20:31:07 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 06 Nov 2020 20:31:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 06 Nov 2020 20:31:10 GMT
EXPOSE 8080
# Fri, 06 Nov 2020 20:31:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a3c2059a8a90e1819eafb917f66ddf3baae20fcfd47bb182749d9d7ca8a2d4`  
		Last Modified: Wed, 28 Oct 2020 00:21:51 GMT  
		Size: 75.2 MB (75241034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061c15b497b98fbb9e44aa4564093b9cdb9b0882ead79911573fa3b0f1114e`  
		Last Modified: Wed, 28 Oct 2020 01:18:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635bf882c8f52507f16f79d383ba68e131dbcee0dbb9be4c89dbba06c38528b5`  
		Last Modified: Fri, 06 Nov 2020 20:55:00 GMT  
		Size: 24.1 MB (24082090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7c967ded4e33735b8f8e35b9d43f6e9f6de3313778b6223493ddae961d3e34`  
		Last Modified: Fri, 06 Nov 2020 20:54:57 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk8-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:8e9e95bae1b5e14e13fa822e0c18052708e8e8fedc65c0307c33b974cf48ed28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.3 MB (147281700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb6641b7034969bba1628f59331ee40ff41f15fad77326ac7ac75c416eac7114`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Wed, 28 Oct 2020 00:39:50 GMT
ARG version=1.8.0_272.b10-3
# Wed, 28 Oct 2020 00:40:33 GMT
# ARGS: version=1.8.0_272.b10-3
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 28 Oct 2020 00:40:42 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 00:40:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 28 Oct 2020 01:59:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 28 Oct 2020 01:59:18 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Oct 2020 01:59:19 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 28 Oct 2020 01:59:20 GMT
WORKDIR /usr/local/tomcat
# Wed, 28 Oct 2020 01:59:21 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 28 Oct 2020 01:59:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 28 Oct 2020 02:04:06 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 28 Oct 2020 02:04:07 GMT
ENV TOMCAT_MAJOR=9
# Wed, 28 Oct 2020 02:04:08 GMT
ENV TOMCAT_VERSION=9.0.39
# Wed, 28 Oct 2020 02:04:09 GMT
ENV TOMCAT_SHA512=307ca646bac267e529fb0862278f7133fe80813f0af64a44aed949f4c7a9a98aeb9bd7f08b087645b40c6fefdd3a7fe519e4858a3dbf0a19c38c53704f92b575
# Fri, 06 Nov 2020 20:24:58 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 06 Nov 2020 20:25:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 06 Nov 2020 20:25:05 GMT
EXPOSE 8080
# Fri, 06 Nov 2020 20:25:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceaa740c3f1368a605094068479b55a57d62eb653f2548f24cf4af693e7b345`  
		Last Modified: Wed, 28 Oct 2020 00:42:47 GMT  
		Size: 59.3 MB (59335956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36bfe37602c62e12c6c7155a91e35556290b41582f0f509b2d56557725ce6af`  
		Last Modified: Wed, 28 Oct 2020 02:14:53 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a45b9e64d88324211f33615d1b103641b53e46da070f16ee39d32c7e290db8f`  
		Last Modified: Fri, 06 Nov 2020 20:48:39 GMT  
		Size: 24.6 MB (24591304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55766e97eab0423d2c1361fbc5a06404f62815ad4f437ae304aedca7c376faa9`  
		Last Modified: Fri, 06 Nov 2020 20:48:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
