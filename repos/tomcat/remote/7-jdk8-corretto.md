## `tomcat:7-jdk8-corretto`

```console
$ docker pull tomcat@sha256:378215d52485694bad7ae8ebbfff1f652f85dc5d05149b94b6f4a18a747d6fc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:7-jdk8-corretto` - linux; amd64

```console
$ docker pull tomcat@sha256:a51c47a4a5cab13e016285dc13c1599c7b6432b5360e6644bf1cc6627a2e00dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198057887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efe82f828a8ea8a360edbdfeab75448989a33b1c4fe4e2f185c657cc0b3a838`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Apr 2020 06:46:32 GMT
ADD file:119ae574c5d5b6e59e83ecadbe4c8dc4e7b535508e63704e74939df696c9b9a1 in / 
# Wed, 01 Apr 2020 06:46:33 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 13:48:10 GMT
ARG rpm_x64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.x86_64.rpm
# Wed, 01 Apr 2020 13:48:10 GMT
ARG path_x64=https://corretto.aws/downloads/resources/8.242.08.1
# Wed, 01 Apr 2020 13:48:10 GMT
ARG key_x64=6DC3636DAE534049C8B94623A122542AB04F24E3
# Wed, 01 Apr 2020 13:48:10 GMT
ARG rpm_aarch64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.aarch64.rpm
# Wed, 01 Apr 2020 13:48:10 GMT
ARG path_aarch64=https://corretto.aws/downloads/resources/8.242.08.1
# Wed, 01 Apr 2020 13:48:11 GMT
ARG key_aarch64=6DC3636DAE534049C8B94623A122542AB04F24E3
# Wed, 01 Apr 2020 13:48:29 GMT
# ARGS: key_aarch64=6DC3636DAE534049C8B94623A122542AB04F24E3 key_x64=6DC3636DAE534049C8B94623A122542AB04F24E3 path_aarch64=https://corretto.aws/downloads/resources/8.242.08.1 path_x64=https://corretto.aws/downloads/resources/8.242.08.1 rpm_aarch64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.aarch64.rpm rpm_x64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.x86_64.rpm
RUN set -eux;     case "$(uname -p)" in         x86_64) rpm=$rpm_x64; path=$path_x64; key=$key_x64 ;;         aarch64) rpm=$rpm_aarch64; path=$path_aarch64; key=$key_aarch64 ;;         *) echo >&2 "Unsupported architecture $(uname -p)."; exit 1 ;;     esac;         curl -O $path/$rpm     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key     && gpg --armor --export $key > corretto.asc     && rpm --import corretto.asc     && rpm -K $rpm     && rpm -i $rpm     && rm -r $GNUPGHOME corretto.asc $rpm     && yum install -y fontconfig     && yum clean all
# Wed, 01 Apr 2020 13:48:29 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 01 Apr 2020 14:07:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 01 Apr 2020 14:07:27 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 14:07:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 01 Apr 2020 14:07:28 GMT
WORKDIR /usr/local/tomcat
# Wed, 01 Apr 2020 14:07:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 14:07:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 14:11:34 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 01 Apr 2020 14:13:32 GMT
ENV TOMCAT_MAJOR=7
# Wed, 01 Apr 2020 14:13:32 GMT
ENV TOMCAT_VERSION=7.0.103
# Wed, 01 Apr 2020 14:13:32 GMT
ENV TOMCAT_SHA512=3a02bf074fd5a00e751b1229cffdf7c7d9ee52ab825ddecb1e5b766d40999f08be5d3758704333a922c593b139bce51feb8b33924731aacf3acebba8beb5cce8
# Wed, 01 Apr 2020 14:15:12 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if curl -fL -o "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| sort -u 			| xargs -r rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 01 Apr 2020 14:15:14 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 01 Apr 2020 14:15:14 GMT
EXPOSE 8080
# Wed, 01 Apr 2020 14:15:14 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a8d577519c9fb37ef239a77026a16c019d20cce14b25867f57a44459b3bbf387`  
		Last Modified: Wed, 01 Apr 2020 06:48:00 GMT  
		Size: 61.7 MB (61655014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4ad584aa484a0420ddb045725aaf2dbfe7319ee40021e1a55cae65ce104b4d`  
		Last Modified: Wed, 01 Apr 2020 13:49:17 GMT  
		Size: 121.6 MB (121591683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb197178d15578b084ea66266c751b8ac14a080e2076cc13de830c0de736792f`  
		Last Modified: Wed, 01 Apr 2020 14:16:51 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7a586a46a4aba5819106a44b723e42095f112897da2e8b9e4e9c2a65a0a10f`  
		Last Modified: Wed, 01 Apr 2020 14:17:19 GMT  
		Size: 14.8 MB (14810920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8ee903d9dc906ffe6103c4aa879abc0ca7fe30692355b16b72f3198d027cde`  
		Last Modified: Wed, 01 Apr 2020 14:17:17 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:7-jdk8-corretto` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:c4ed2f54619cd1b6e5f8d65c5b537268c511d240dec293a11ae2f44704481b29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182714007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3dc5627c16475256341ce1dd1d72148dbf016bac7f75fc84a81254a2a48aff9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Apr 2020 05:22:43 GMT
ADD file:40b8f329ad6d591029e1a4cde76c1d097315b136796d31bb9d3df35183423c14 in / 
# Wed, 01 Apr 2020 05:22:46 GMT
CMD ["/bin/bash"]
# Wed, 01 Apr 2020 08:29:02 GMT
ARG rpm_x64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.x86_64.rpm
# Wed, 01 Apr 2020 08:29:02 GMT
ARG path_x64=https://corretto.aws/downloads/resources/8.242.08.1
# Wed, 01 Apr 2020 08:29:03 GMT
ARG key_x64=6DC3636DAE534049C8B94623A122542AB04F24E3
# Wed, 01 Apr 2020 08:29:03 GMT
ARG rpm_aarch64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.aarch64.rpm
# Wed, 01 Apr 2020 08:29:04 GMT
ARG path_aarch64=https://corretto.aws/downloads/resources/8.242.08.1
# Wed, 01 Apr 2020 08:29:04 GMT
ARG key_aarch64=6DC3636DAE534049C8B94623A122542AB04F24E3
# Wed, 01 Apr 2020 08:29:27 GMT
# ARGS: key_aarch64=6DC3636DAE534049C8B94623A122542AB04F24E3 key_x64=6DC3636DAE534049C8B94623A122542AB04F24E3 path_aarch64=https://corretto.aws/downloads/resources/8.242.08.1 path_x64=https://corretto.aws/downloads/resources/8.242.08.1 rpm_aarch64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.aarch64.rpm rpm_x64=java-1.8.0-amazon-corretto-devel-1.8.0_242.b08-1.x86_64.rpm
RUN set -eux;     case "$(uname -p)" in         x86_64) rpm=$rpm_x64; path=$path_x64; key=$key_x64 ;;         aarch64) rpm=$rpm_aarch64; path=$path_aarch64; key=$key_aarch64 ;;         *) echo >&2 "Unsupported architecture $(uname -p)."; exit 1 ;;     esac;         curl -O $path/$rpm     && export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys $key     && gpg --armor --export $key > corretto.asc     && rpm --import corretto.asc     && rpm -K $rpm     && rpm -i $rpm     && rm -r $GNUPGHOME corretto.asc $rpm     && yum install -y fontconfig     && yum clean all
# Wed, 01 Apr 2020 08:29:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Wed, 01 Apr 2020 08:51:34 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 01 Apr 2020 08:51:36 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 08:51:40 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 01 Apr 2020 08:51:40 GMT
WORKDIR /usr/local/tomcat
# Wed, 01 Apr 2020 08:51:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:51:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:54:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 01 Apr 2020 08:57:32 GMT
ENV TOMCAT_MAJOR=7
# Wed, 01 Apr 2020 08:57:33 GMT
ENV TOMCAT_VERSION=7.0.103
# Wed, 01 Apr 2020 08:57:34 GMT
ENV TOMCAT_SHA512=3a02bf074fd5a00e751b1229cffdf7c7d9ee52ab825ddecb1e5b766d40999f08be5d3758704333a922c593b139bce51feb8b33924731aacf3acebba8beb5cce8
# Wed, 01 Apr 2020 08:58:50 GMT
RUN set -eux; 		if ! command -v yumdb > /dev/null; then 		yum install -y yum-utils; 		yumdb set reason dep yum-utils; 	fi; 	if [ -f /etc/oracle-release ]; then 		yumdb set reason user filesystem; 	fi; 	_yum_install_temporary() { ( set -eu +x; 		local pkg todo=''; 		for pkg; do 			if ! rpm --query "$pkg" > /dev/null 2>&1; then 				todo="$todo $pkg"; 			fi; 		done; 		if [ -n "$todo" ]; then 			set -x; 			yum install -y $todo; 			yumdb set reason dep $todo; 		fi; 	) }; 	_yum_install_temporary gzip tar; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if curl -fL -o "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	_yum_install_temporary 		apr-devel 		gcc 		make 		openssl-devel 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		deps="$( 		find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 			| awk '/=>/ && $(NF-1) != "=>" { print $(NF-1) }' 			| sort -u 			| xargs -r rpm --query --whatprovides 			| sort -u 	)"; 	[ -z "$deps" ] || yumdb set reason user $deps; 		yum autoremove -y; 	yum clean all; 	rm -rf /var/cache/yum; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 01 Apr 2020 08:58:54 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 01 Apr 2020 08:58:55 GMT
EXPOSE 8080
# Wed, 01 Apr 2020 08:58:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:01d0a3bd5b98a6512409a10e5e5b065e87b794f924f3f9f7662939925aac631b`  
		Last Modified: Wed, 01 Apr 2020 05:24:01 GMT  
		Size: 63.1 MB (63072580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b897bb90f24638d350f41e113472509d7732f6a6d4f27763cf180b28a4f8c6`  
		Last Modified: Wed, 01 Apr 2020 08:30:57 GMT  
		Size: 105.0 MB (104974349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f0a013a8ec044e74bd2a62b7f1d68dd524cc182f3a640e6b9342b7571c719`  
		Last Modified: Wed, 01 Apr 2020 08:59:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825b922059beb5f81671004b54dfdf82c90ac22033466b48b324f35cac2286a3`  
		Last Modified: Wed, 01 Apr 2020 09:00:25 GMT  
		Size: 14.7 MB (14666740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d54d261a58f56a87325408de14fd50510395c5ead4f0d23c07c1b8002c56dd4`  
		Last Modified: Wed, 01 Apr 2020 09:00:22 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
