## `tomcat:9-jdk11-corretto`

```console
$ docker pull tomcat@sha256:17f808ea3f6a9a26f85319a845b718b28cc0ea5ce4d17befbef4fa312dcedaa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk11-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:303b3a864ee5492a9c1a54843edb2e2c9a96a1c4f35c91e076f2e9ca11f41acc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.4 MB (233401093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87519ab786f736cfea830fcca342b3863a730df6c04d4214c8bc99846cb01048`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 18 Dec 2020 07:04:34 GMT
ADD file:63bb1089f29109498e6000d9884216288b7b1b9093e0c247b99df2a8ba64d601 in / 
# Fri, 18 Dec 2020 07:04:35 GMT
CMD ["/bin/bash"]
# Fri, 18 Dec 2020 09:26:54 GMT
ARG version=11.0.9.12-1
# Fri, 18 Dec 2020 09:27:11 GMT
# ARGS: version=11.0.9.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 18 Dec 2020 09:27:11 GMT
ENV LANG=C.UTF-8
# Fri, 18 Dec 2020 09:27:11 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 18 Dec 2020 09:58:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 18 Dec 2020 09:58:50 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 09:58:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 18 Dec 2020 09:58:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 18 Dec 2020 09:58:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 09:58:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 10:02:49 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 18 Dec 2020 10:02:49 GMT
ENV TOMCAT_MAJOR=9
# Fri, 18 Dec 2020 10:02:50 GMT
ENV TOMCAT_VERSION=9.0.41
# Fri, 18 Dec 2020 10:02:50 GMT
ENV TOMCAT_SHA512=b6450e590a37c5bccf049b1176c441f0964796995e80d4c7c7d9fb74f9ad817107c303b6b83ed3d71c9251b2b8acf334b90a4abdf9deea122e338643cece0766
# Fri, 18 Dec 2020 10:03:20 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 18 Dec 2020 10:03:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 18 Dec 2020 10:03:23 GMT
EXPOSE 8080
# Fri, 18 Dec 2020 10:03:23 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b6f03d5d6f5a93eede753139822eca5ce4a921a8c35922b9969996cfc31deb60`  
		Last Modified: Wed, 09 Dec 2020 16:33:37 GMT  
		Size: 62.0 MB (62008519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa4d5051eccba8a34b0c5943e7d3af1b699630442bcab5c4e6327140c73b25f`  
		Last Modified: Fri, 18 Dec 2020 09:29:06 GMT  
		Size: 146.5 MB (146467196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9153a320ee49c5280b1386c4b8ad06f5096b2e29c7f5ea7a59303cc7c8f289f`  
		Last Modified: Fri, 18 Dec 2020 10:11:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c067ffee87a007060d22001b74a4d3371c3993c90831561dea1c1301c9c018`  
		Last Modified: Fri, 18 Dec 2020 10:12:22 GMT  
		Size: 24.9 MB (24925107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206ffd86a5a3522ac5dfc6970c315b339a55cd439afea545e570135fa8aa707`  
		Last Modified: Fri, 18 Dec 2020 10:12:19 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk11-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:6a96e0924a62c419685d4c93b84c61b9cae1bee4783b831e50423475eca2f2fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.5 MB (233501337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a6b63bc56d2c376f5294317979dfc4bee1854b9c7bfc04337489adcee9fa5a9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Dec 2020 22:48:34 GMT
ADD file:fef50d3f23c05efa2cb62375be9cc62cd47bb605bd119f813fa1c7f529d9d27c in / 
# Thu, 17 Dec 2020 22:48:39 GMT
CMD ["/bin/bash"]
# Thu, 17 Dec 2020 23:07:06 GMT
ARG version=11.0.9.12-1
# Thu, 17 Dec 2020 23:07:34 GMT
# ARGS: version=11.0.9.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 17 Dec 2020 23:07:36 GMT
ENV LANG=C.UTF-8
# Thu, 17 Dec 2020 23:07:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Fri, 18 Dec 2020 18:13:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 18 Dec 2020 18:14:00 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 18:14:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 18 Dec 2020 18:14:04 GMT
WORKDIR /usr/local/tomcat
# Fri, 18 Dec 2020 18:14:04 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 18:14:05 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 18 Dec 2020 18:18:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 18 Dec 2020 18:18:20 GMT
ENV TOMCAT_MAJOR=9
# Fri, 18 Dec 2020 18:18:21 GMT
ENV TOMCAT_VERSION=9.0.41
# Fri, 18 Dec 2020 18:18:21 GMT
ENV TOMCAT_SHA512=b6450e590a37c5bccf049b1176c441f0964796995e80d4c7c7d9fb74f9ad817107c303b6b83ed3d71c9251b2b8acf334b90a4abdf9deea122e338643cece0766
# Fri, 18 Dec 2020 18:19:19 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| xargs -rt readlink -e 			| sort -u 			| xargs -rt rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 18 Dec 2020 18:19:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 18 Dec 2020 18:19:25 GMT
EXPOSE 8080
# Fri, 18 Dec 2020 18:19:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ee4590ce5e19453a11908348603e8da0375a376105f9b2e130afce2344f42677`  
		Last Modified: Wed, 09 Dec 2020 22:47:33 GMT  
		Size: 63.7 MB (63675700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f87068084c62f6785078d6926dbd1770554b01e03da0bd3aadf6343dae011f`  
		Last Modified: Thu, 17 Dec 2020 23:09:37 GMT  
		Size: 144.5 MB (144497469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc54358091442109012230cbce6c0113f2ed2d9a5666922af99d8b317dc4f5a1`  
		Last Modified: Fri, 18 Dec 2020 18:28:12 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095db7941f05c0f8a2530e13e0cdbf2bb86915a99815f6f37c6d954cf63354a3`  
		Last Modified: Fri, 18 Dec 2020 18:29:22 GMT  
		Size: 25.3 MB (25327863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e34779928771f3b3f2f837ff0d584b6dbc973b9d2c822601d98451c83ff33a`  
		Last Modified: Fri, 18 Dec 2020 18:29:17 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
