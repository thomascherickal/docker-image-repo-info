## `tomcat:8-jdk8-corretto`

```console
$ docker pull tomcat@sha256:3e6197324663284c71fc6dcd7e898370ffb487e53043aa9e8b62200a8a52960d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:8-jdk8-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:a9507e07e40cdcc2375072582a9cb26c5b771009b47310ff6352130287825c1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161264122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:627ac42c39794e613479581f9b7fbe09e25249c0f9a8bb1cd7e25f7c2ff72172`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Dec 2020 07:04:34 GMT
ADD file:63bb1089f29109498e6000d9884216288b7b1b9093e0c247b99df2a8ba64d601 in / 
# Fri, 18 Dec 2020 07:04:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Dec 2020 09:26:32 GMT
ARG version=1.8.0_275.b01-1
# Fri, 18 Dec 2020 09:26:47 GMT
# ARGS: version=1.8.0_275.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 18 Dec 2020 09:26:47 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 09:26:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 18 Dec 2020 10:00:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 18 Dec 2020 10:00:51 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 10:00:52 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 18 Dec 2020 10:00:52 GMT
WORKDIR /usr/local/tomcat
# Fri, 18 Dec 2020 10:00:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 10:00:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 10:06:21 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 18 Dec 2020 10:06:21 GMT
ENV TOMCAT_MAJOR=8
# Fri, 18 Dec 2020 10:06:21 GMT
ENV TOMCAT_VERSION=8.5.61
# Fri, 18 Dec 2020 10:06:21 GMT
ENV TOMCAT_SHA512=55d7d0442a3c1bae7e470ba75c7473a8deeaf33c60ff66cecdc136ae0b0e852b871940c5deb720d501b444ccb00f0b8520b1930cbf564c2f46ceaf1e0367d41b
# Fri, 18 Dec 2020 10:07:03 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 18 Dec 2020 10:07:05 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 18 Dec 2020 10:07:05 GMT
EXPOSE 8080
# Fri, 18 Dec 2020 10:07:05 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b6f03d5d6f5a93eede753139822eca5ce4a921a8c35922b9969996cfc31deb60`  
		Last Modified: Wed, 09 Dec 2020 16:33:37 GMT  
		Size: 62.0 MB (62008519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6f58facb3659bb3697cd51471f37ec5e30d4b0ddd0a28de875b8b667b5f8c9`  
		Last Modified: Fri, 18 Dec 2020 09:28:44 GMT  
		Size: 75.3 MB (75279152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99440d163a7e19ab703177ad8ad4c8731175746fd791c83708de5653c87006dc`  
		Last Modified: Fri, 18 Dec 2020 10:11:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c354c82d452f3b648e7f2068625da343f1c8edd22bec90a6000c7aa160f18001`  
		Last Modified: Fri, 18 Dec 2020 10:13:42 GMT  
		Size: 24.0 MB (23976181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fcd42597092190a86a94cb2e44675a1c126a790909d2c8593705db5486745c5`  
		Last Modified: Fri, 18 Dec 2020 10:13:40 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk8-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:d1a78a2d1db27a1ae5ba0f2c1c542eb69005ac8dc0bd5aabac1c799032c52455
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.4 MB (147407870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c83a43b6845d302cd70e876ed55a2c9dab0aefe82dbac5a0e1510cb6a09e0669`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Dec 2020 22:48:34 GMT
ADD file:fef50d3f23c05efa2cb62375be9cc62cd47bb605bd119f813fa1c7f529d9d27c in / 
# Thu, 17 Dec 2020 22:48:39 GMT
CMD ["/bin/bash"]
# Thu, 17 Dec 2020 23:06:25 GMT
ARG version=1.8.0_275.b01-1
# Thu, 17 Dec 2020 23:06:58 GMT
# ARGS: version=1.8.0_275.b01-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 17 Dec 2020 23:06:59 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 23:07:00 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Fri, 18 Dec 2020 18:15:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 18 Dec 2020 18:15:52 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 18:15:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 18 Dec 2020 18:15:56 GMT
WORKDIR /usr/local/tomcat
# Fri, 18 Dec 2020 18:15:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 18:15:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 18:22:52 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 18 Dec 2020 18:22:53 GMT
ENV TOMCAT_MAJOR=8
# Fri, 18 Dec 2020 18:22:53 GMT
ENV TOMCAT_VERSION=8.5.61
# Fri, 18 Dec 2020 18:22:54 GMT
ENV TOMCAT_SHA512=55d7d0442a3c1bae7e470ba75c7473a8deeaf33c60ff66cecdc136ae0b0e852b871940c5deb720d501b444ccb00f0b8520b1930cbf564c2f46ceaf1e0367d41b
# Fri, 18 Dec 2020 18:23:47 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 18 Dec 2020 18:23:50 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 18 Dec 2020 18:23:51 GMT
EXPOSE 8080
# Fri, 18 Dec 2020 18:23:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ee4590ce5e19453a11908348603e8da0375a376105f9b2e130afce2344f42677`  
		Last Modified: Wed, 09 Dec 2020 22:47:33 GMT  
		Size: 63.7 MB (63675700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda0d28738ebf400b9e9d08508b79c6c8f7bcf27a4a9c5639355711317bb9da2`  
		Last Modified: Thu, 17 Dec 2020 23:08:57 GMT  
		Size: 59.4 MB (59352245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d849b0bccb0bf5db217627fb186675ceebfe0c07c217771ded5816c479ab172`  
		Last Modified: Fri, 18 Dec 2020 18:28:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c8e902c850a360556905ffb95d76ff96d010349f0234a5c37f6b7443f56a0`  
		Last Modified: Fri, 18 Dec 2020 18:30:28 GMT  
		Size: 24.4 MB (24379621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed84559b62fc7617979aafd61832da84bc329da06ca741175a5b4158c5456a8`  
		Last Modified: Fri, 18 Dec 2020 18:30:23 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
