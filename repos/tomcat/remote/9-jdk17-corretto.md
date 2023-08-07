## `tomcat:9-jdk17-corretto`

```console
$ docker pull tomcat@sha256:3fe1287550226828fa406816a93c0ec3307e7ad19bed7b674663f669090acc0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:9-jdk17-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:ee2be88bfe3cfd5c9abd5a802a10ffa3d76bfd3eba7c5b8bba5c9a2439507ad5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.4 MB (231369041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a9fe3bce19a54259d5d1ba9052c2ad87519c48519e990d06d5010cde2e032a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 26 Jul 2023 19:20:31 GMT
COPY dir:eb203b2e14f406c161ffae3b2fa7ec59db3f5a04437b6e040395c2bc34835c5f in / 
# Wed, 26 Jul 2023 19:20:31 GMT
CMD ["/bin/bash"]
# Wed, 26 Jul 2023 20:18:57 GMT
ARG version=17.0.8.7-1
# Wed, 26 Jul 2023 20:19:22 GMT
# ARGS: version=17.0.8.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 26 Jul 2023 20:19:22 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jul 2023 20:19:22 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Wed, 26 Jul 2023 21:03:03 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Jul 2023 21:03:03 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jul 2023 21:03:04 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Jul 2023 21:03:04 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Jul 2023 21:03:04 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Jul 2023 21:03:04 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Jul 2023 21:03:04 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Jul 2023 21:03:04 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Jul 2023 21:03:04 GMT
ENV TOMCAT_VERSION=9.0.78
# Wed, 26 Jul 2023 21:03:04 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Wed, 26 Jul 2023 21:03:40 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Wed, 26 Jul 2023 21:03:42 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Jul 2023 21:03:42 GMT
EXPOSE 8080
# Wed, 26 Jul 2023 21:03:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a8d554425610d474f28e23ecfc3224dd78fca045a5c09515dbf51a8606c33d8f`  
		Last Modified: Tue, 25 Jul 2023 11:25:06 GMT  
		Size: 62.5 MB (62451920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331663fb7b989f09106c7cd829c15080f14aa2671e6219eaa7c6979548d1e48`  
		Last Modified: Wed, 26 Jul 2023 20:29:30 GMT  
		Size: 152.1 MB (152112347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368600c4deec010921387fc5cc45be1e712598430acf16f8164c0c94b89578ac`  
		Last Modified: Wed, 26 Jul 2023 21:11:40 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad78eefdd26c164d2956879d8d5b1f9fe99efde2464f067198e2d8cffdfe2ce`  
		Last Modified: Wed, 26 Jul 2023 21:11:41 GMT  
		Size: 16.8 MB (16804472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa9ac0f315435f4c13614f851396a68c242e9e80806b2ee1299793f8e6887b6`  
		Last Modified: Wed, 26 Jul 2023 21:11:40 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jdk17-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:fa1183f9c8cbd980706fd46992b1f3bb3465218e7bfd598f8a1f90db359ba82e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231542456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26befd30f421dc9df5aa48f12fea0c11d3ae5297650c1f319920f1785519871e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:56 GMT
COPY dir:95dabd7a234aac70a826a1e3c0eafa3928b0be72717af1dea469f66b7db891d5 in / 
# Mon, 07 Aug 2023 19:40:57 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:26:46 GMT
ARG version=17.0.8.7-1
# Mon, 07 Aug 2023 20:27:05 GMT
# ARGS: version=17.0.8.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 07 Aug 2023 20:27:07 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:27:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Mon, 07 Aug 2023 21:43:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 07 Aug 2023 21:43:06 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Aug 2023 21:43:06 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 07 Aug 2023 21:43:06 GMT
WORKDIR /usr/local/tomcat
# Mon, 07 Aug 2023 21:43:07 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 07 Aug 2023 21:43:07 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 07 Aug 2023 21:43:07 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Mon, 07 Aug 2023 21:43:07 GMT
ENV TOMCAT_MAJOR=9
# Mon, 07 Aug 2023 21:43:07 GMT
ENV TOMCAT_VERSION=9.0.78
# Mon, 07 Aug 2023 21:43:07 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Mon, 07 Aug 2023 21:43:37 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y --setopt=skip_missing_names_on_install=False yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y --setopt=skip_missing_names_on_install=False $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl11-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt rpm --query --whatprovides 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r yumdb set reason user 	; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Mon, 07 Aug 2023 21:43:38 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 07 Aug 2023 21:43:38 GMT
EXPOSE 8080
# Mon, 07 Aug 2023 21:43:38 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c3b5a1e75067e9d540ad8d844cad5a291a8cce89e1a3ed8e0f362a5736d3030c`  
		Last Modified: Wed, 02 Aug 2023 19:26:38 GMT  
		Size: 64.1 MB (64129548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c69eb4237f8f93689d48b1eb6408a260fd5bab441a8b8116e0f134821135e57`  
		Last Modified: Mon, 07 Aug 2023 20:41:11 GMT  
		Size: 150.7 MB (150657784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315783f542f897053592b1020c14b38b405fc9299602f9215aafe4795417cc23`  
		Last Modified: Mon, 07 Aug 2023 21:50:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7f30200fc949e142efc52f6f04c3ace429031c4c16fbf183acdbfe91a6e8d4`  
		Last Modified: Mon, 07 Aug 2023 21:50:27 GMT  
		Size: 16.8 MB (16754818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a48800f477471c053be43d5679f2d97a62ab93e7103661f8c7c2a1b7ec7ca`  
		Last Modified: Mon, 07 Aug 2023 21:50:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
