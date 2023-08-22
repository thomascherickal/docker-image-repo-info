## `tomcat:8-jdk11-corretto-al2`

```console
$ docker pull tomcat@sha256:221699fa722fbcae5acded05d7b9e8b5ddf55e54712da36c4a03087090a58e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:8-jdk11-corretto-al2` - linux; amd64

```console
$ docker pull tomcat@sha256:1b276880316e7495615e750f630fb2198e25f95444618db610bfe990a27cb1ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226231302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97c2184eca1cac8b4d26450dfc3302acaf9aa16e33b0055c4e7f5a37293d5b59`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:52 GMT
COPY dir:74433340f66bb20aa9bebf7ee91eaada91d987f210fbb253d98f2ee60012726f in / 
# Tue, 22 Aug 2023 20:19:52 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:28:14 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:28:38 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 22 Aug 2023 21:28:39 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:28:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 22 Aug 2023 22:32:13 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 22 Aug 2023 22:32:13 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Aug 2023 22:32:13 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 22 Aug 2023 22:32:13 GMT
WORKDIR /usr/local/tomcat
# Tue, 22 Aug 2023 22:32:13 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 22:32:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 22:35:01 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 22 Aug 2023 22:35:01 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Aug 2023 22:35:01 GMT
ENV TOMCAT_VERSION=8.5.92
# Tue, 22 Aug 2023 22:35:01 GMT
ENV TOMCAT_SHA512=faab13a29531a800d38b2602ff76c0041277ffbfb25b938bbefb84ef6ad3ffa26d2c2645cd233eb0d819bcca9887aaeb44df6c044852160d000e5084b1addc2f
# Tue, 22 Aug 2023 22:35:39 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Tue, 22 Aug 2023 22:35:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Aug 2023 22:35:41 GMT
EXPOSE 8080
# Tue, 22 Aug 2023 22:35:41 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:8cd2389cb7276ab6d8d1154ee827bc715858f6827bdde1e9b5499a2eb3b76dc4`  
		Last Modified: Wed, 16 Aug 2023 14:05:30 GMT  
		Size: 62.5 MB (62492616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4562f11cda981b481331917db7dd8a91c272feeb7686875ced2618cee48f3f7`  
		Last Modified: Tue, 22 Aug 2023 21:39:35 GMT  
		Size: 147.8 MB (147829797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539663fd71956e527bacf9639c1c16e36bb7bc3fdad8834525c72e846dea4e7`  
		Last Modified: Tue, 22 Aug 2023 22:39:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966add39eb07b09f46b9f6336d08e2b7950ca35fbae681aa9b70bf65c08bcfd3`  
		Last Modified: Tue, 22 Aug 2023 22:40:35 GMT  
		Size: 15.9 MB (15908583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92f316c4bb0d4d29d67722492c18804bc2b8a6dc5ecc3a77ac43f3f8739dc6a`  
		Last Modified: Tue, 22 Aug 2023 22:40:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jdk11-corretto-al2` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:541ad43d2380fee3d3fd3c420e6928be2b622ccd63dcda2e6d6e6b42ecb69e97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.9 MB (224869832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a907f9c32fbbc887d23087e3b169d08cc92e5447757e8f9ddd4ed9d94cbb23db`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:53 GMT
COPY dir:e20aef745ed6033815440b78b98680b9989b365a1e5e12e6f94169e6de7e94c3 in / 
# Tue, 22 Aug 2023 19:39:54 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:08:10 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:08:29 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 22 Aug 2023 21:08:31 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:08:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Tue, 22 Aug 2023 21:46:10 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 22 Aug 2023 21:46:10 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Aug 2023 21:46:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 22 Aug 2023 21:46:10 GMT
WORKDIR /usr/local/tomcat
# Tue, 22 Aug 2023 21:46:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 21:46:10 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 22 Aug 2023 21:48:21 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 22 Aug 2023 21:48:21 GMT
ENV TOMCAT_MAJOR=8
# Tue, 22 Aug 2023 21:48:21 GMT
ENV TOMCAT_VERSION=8.5.92
# Tue, 22 Aug 2023 21:48:21 GMT
ENV TOMCAT_SHA512=faab13a29531a800d38b2602ff76c0041277ffbfb25b938bbefb84ef6ad3ffa26d2c2645cd233eb0d819bcca9887aaeb44df6c044852160d000e5084b1addc2f
# Tue, 22 Aug 2023 21:48:54 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Tue, 22 Aug 2023 21:48:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 22 Aug 2023 21:48:55 GMT
EXPOSE 8080
# Tue, 22 Aug 2023 21:48:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3e86c88b00180fc8094116a7111cfe1c0e88e04a6c513618fbde52ee5d97a51a`  
		Last Modified: Wed, 16 Aug 2023 18:15:18 GMT  
		Size: 64.1 MB (64127623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04be7a5022112b6506828c4f917e5090807e3ba67ed4385a10a57a868045e4c`  
		Last Modified: Tue, 22 Aug 2023 21:17:12 GMT  
		Size: 144.9 MB (144930471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca03eda65cf980af6ff8cc035872adc365b8ceee0121f23611c562abfd0547e`  
		Last Modified: Tue, 22 Aug 2023 21:52:18 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4730c85efc79bd23a635e852a0f028a7bcdff40928871c9027fa5d9963409a02`  
		Last Modified: Tue, 22 Aug 2023 21:53:32 GMT  
		Size: 15.8 MB (15811434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767dc1936a0923b63b23b2aa497bd0b469b28ffee5f50cffa36bf2d41098ed5`  
		Last Modified: Tue, 22 Aug 2023 21:53:31 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
