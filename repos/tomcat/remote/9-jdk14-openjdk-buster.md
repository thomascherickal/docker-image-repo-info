## `tomcat:9-jdk14-openjdk-buster`

```console
$ docker pull tomcat@sha256:d37339c2730de08af4da98c5a57490236c3c599bf21fc921a0ab6e7a49f2a7f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `tomcat:9-jdk14-openjdk-buster` - linux; amd64

```console
$ docker pull tomcat@sha256:9c43162a512a3d65df59622dd4c76c447e2ba79016d4b69198ef26beb9755191
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.4 MB (345415344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365f18a644d90c94787b4665fd458fc779362dbfbb9d8435ddcff8468cd47603`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 15 May 2020 06:28:12 GMT
ADD file:fb54c709daa205bf9d04eb3d90ba068db4c34dfe3b6ec0d7691f677286120903 in / 
# Fri, 15 May 2020 06:28:13 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:32:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:32:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:32:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:59:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:59:27 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 21:00:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Fri, 15 May 2020 21:00:48 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 21:00:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 15 May 2020 21:00:50 GMT
ENV JAVA_VERSION=14.0.1
# Fri, 22 May 2020 01:24:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk14.0.1/664493ef4a6946b186ff29eb326336a2/7/GPL/openjdk-14.0.1_linux-x64_bin.tar.gz; 			downloadSha256=22ce248e0bd69f23028625bede9d1b3080935b68d011eaaf9e241f84d6b9c4cc; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 22 May 2020 01:24:15 GMT
CMD ["jshell"]
# Fri, 22 May 2020 02:27:32 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 22 May 2020 02:27:32 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 May 2020 02:27:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 22 May 2020 02:27:33 GMT
WORKDIR /usr/local/tomcat
# Fri, 22 May 2020 02:27:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 22 May 2020 02:27:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 22 May 2020 02:30:46 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 22 May 2020 02:30:46 GMT
ENV TOMCAT_MAJOR=9
# Fri, 22 May 2020 02:30:47 GMT
ENV TOMCAT_VERSION=9.0.35
# Fri, 22 May 2020 02:30:47 GMT
ENV TOMCAT_SHA512=0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98
# Fri, 22 May 2020 02:31:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 22 May 2020 02:31:13 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 22 May 2020 02:31:13 GMT
EXPOSE 8080
# Fri, 22 May 2020 02:31:13 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:376057ac6fa17f65688c56977118e2e764b27c348b3f70637fa829cd2a12b200`  
		Last Modified: Fri, 15 May 2020 06:37:20 GMT  
		Size: 50.4 MB (50391294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a63a0a859d859478f30461786a49c2fca3ae7d89ab5b5ce3c81c54951d30f88`  
		Last Modified: Fri, 15 May 2020 17:50:44 GMT  
		Size: 7.8 MB (7812354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496548a8c952b37bdf149ab3654f9085d721ee126b8c73b16860778be5137f5e`  
		Last Modified: Fri, 15 May 2020 17:50:49 GMT  
		Size: 10.0 MB (9996284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2adae3950d4d0f11875568c325d3d542d1f2e2d9b49bdd740bb57fcfc1f6478f`  
		Last Modified: Fri, 15 May 2020 17:51:06 GMT  
		Size: 51.8 MB (51827083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e77013fe29f244314ba9ced8c62b5615de673a1413327ce0d5c27edc88e7363`  
		Last Modified: Fri, 15 May 2020 21:06:51 GMT  
		Size: 13.9 MB (13920351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb9bf9dc6ad362cc8903a38a20a32b41efc2340b83fece9e92f4fcf31ee3145`  
		Last Modified: Fri, 15 May 2020 21:07:57 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1080f9ff870502738bda533d612ec318875f409fcdf8a69768f404e154e886ef`  
		Last Modified: Fri, 22 May 2020 01:28:27 GMT  
		Size: 199.3 MB (199262792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bba1c8b909edc07b768b6ec31d001ef288c99deddaf18c5ee7ad93cd86d470`  
		Last Modified: Fri, 22 May 2020 02:36:43 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b1bbd4f0d85c89b1e9c2dbbc40a626547b6b5ef45803f2e1a0f1e157c86eb`  
		Last Modified: Fri, 22 May 2020 02:37:09 GMT  
		Size: 12.2 MB (12204706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e69a3372a2cff9cf959c1350e2abfeceed0df0b716e073f8cb4d3b1a73d98c`  
		Last Modified: Fri, 22 May 2020 02:37:08 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
