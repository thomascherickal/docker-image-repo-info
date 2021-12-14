<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `convertigo`

-	[`convertigo:7.9`](#convertigo79)
-	[`convertigo:7.9.7`](#convertigo797)
-	[`convertigo:latest`](#convertigolatest)

## `convertigo:7.9`

```console
$ docker pull convertigo@sha256:bd21d6ac291fd7259d25f9a094a0a0a19ed63dcb34f074959a98f42f381761e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `convertigo:7.9` - linux; amd64

```console
$ docker pull convertigo@sha256:dee61c2380267082c1757bc073e1cb5a62c06e87dd1dd6ff69e1cdbf06d77d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.3 MB (437259508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955e61c9685f6822af07fcd66d44b8e7285640c211c60eb86b7f541806adbd0c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:30 GMT
ADD file:aea313ae50ce6474a3df142b34d4dcba4e7e0186ea6fe55389cb2ea903b9ebbb in / 
# Tue, 12 Oct 2021 01:20:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:42:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:30:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 12 Oct 2021 16:30:49 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:30:49 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:30:49 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 12 Oct 2021 16:31:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 12 Oct 2021 16:31:02 GMT
CMD ["jshell"]
# Wed, 13 Oct 2021 13:58:47 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 13 Oct 2021 13:58:47 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 13:58:48 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 13 Oct 2021 13:58:48 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Oct 2021 13:58:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 13 Oct 2021 13:58:48 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 13 Oct 2021 14:20:20 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 13 Oct 2021 14:20:20 GMT
ENV TOMCAT_MAJOR=9
# Wed, 13 Oct 2021 14:20:20 GMT
ENV TOMCAT_VERSION=9.0.54
# Wed, 13 Oct 2021 14:20:20 GMT
ENV TOMCAT_SHA512=83430f24d42186ce2ff51eeef2f7a5517048f37d9050c45cac1e3dba8926d61a1f7f5aba122a34a11ac1dbdd3c1f6d98671841047df139394d43751263de57c3
# Wed, 13 Oct 2021 14:20:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 13 Oct 2021 14:20:48 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Oct 2021 14:20:48 GMT
EXPOSE 8080
# Wed, 13 Oct 2021 14:20:48 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Oct 2021 16:52:00 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 13 Oct 2021 16:52:00 GMT
ENV SWT_GTK3=0
# Wed, 13 Oct 2021 16:52:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 13 Oct 2021 16:52:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 13 Oct 2021 16:52:01 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Oct 2021 16:52:05 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     sudo     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 16:52:06 GMT
ENV GOSU_VERSION=1.12
# Wed, 13 Oct 2021 16:52:06 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 13 Oct 2021 16:52:06 GMT
ENV TINI_VERSION=0.19.0
# Wed, 13 Oct 2021 16:52:06 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 13 Oct 2021 16:52:21 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 13 Oct 2021 16:52:22 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Wed, 13 Oct 2021 16:52:23 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Fri, 22 Oct 2021 18:51:21 GMT
ENV CONVERTIGO_VERSION=7.9.6
# Fri, 22 Oct 2021 18:51:21 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.9.6/convertigo-7.9.6.war
# Fri, 22 Oct 2021 18:51:22 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Fri, 22 Oct 2021 18:51:37 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Fri, 22 Oct 2021 18:51:37 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Fri, 22 Oct 2021 18:51:38 GMT
COPY file:ba6487fa7ec71ffccfe3babd0fb02dea602edf66ffef39f9ab084bdb887562ab in / 
# Fri, 22 Oct 2021 18:51:38 GMT
WORKDIR /workspace
# Fri, 22 Oct 2021 18:51:39 GMT
VOLUME [/workspace]
# Fri, 22 Oct 2021 18:51:39 GMT
EXPOSE 28080
# Fri, 22 Oct 2021 18:51:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:51:40 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:bb7d5a84853b217ac05783963f12b034243070c1c9c8d2e60ada47444f3cce04`  
		Last Modified: Tue, 12 Oct 2021 01:25:37 GMT  
		Size: 54.9 MB (54917520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02b617c6a8c415a175f44d7e2c5d3b521059f2a6112c5f022e005a44a759f2d`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 5.2 MB (5153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e17419b7ee61bbd89c2f0d2833a99cf45e594257d15cb567e4cf7771ce34a`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 10.9 MB (10871935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d2d81226a43a97871acd5afb7e8aabfad4d6b62ae1709c870df3ee230bc3f5`  
		Last Modified: Tue, 12 Oct 2021 15:53:13 GMT  
		Size: 54.6 MB (54567761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae81fdbbf50b4f75c539f7e4ab9fa83b3fbad9f297ed467c5b05cae3a83872`  
		Last Modified: Tue, 12 Oct 2021 16:42:23 GMT  
		Size: 14.1 MB (14071834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8599b41b2126b88acab21fe05ba39f0c5e0460888a5802a6f01364d174e1a894`  
		Last Modified: Tue, 12 Oct 2021 16:47:51 GMT  
		Size: 184.9 MB (184917431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0265ed527e0a2d6a80207c67db71d5ee448d994032d02b003b5ac86e98a80bab`  
		Last Modified: Wed, 13 Oct 2021 14:59:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8cb15ba3e1704f41d31bbaabe400fe82b236467ffec47787416adfe803e280`  
		Last Modified: Wed, 13 Oct 2021 15:15:56 GMT  
		Size: 12.5 MB (12520349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818a96a178f2ed136ffd4d0c74cc5e52e19a8404f9f61f20c88ff5faff8d94ab`  
		Last Modified: Wed, 13 Oct 2021 15:15:55 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd112ceb86f46712e07b8e3a9ef5f661f3ac0d8f6547e86bda901d0bfb2e8189`  
		Last Modified: Wed, 13 Oct 2021 16:52:50 GMT  
		Size: 2.3 MB (2254050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daa7ff6f117459609e7832801cdfbdbe10586444dd02b9f2e1dd62b2ca29d50`  
		Last Modified: Wed, 13 Oct 2021 16:52:50 GMT  
		Size: 970.4 KB (970354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafe172bdcfbaef6d7bca6814910bf6d97553d53afa8bbf3903e82e8f9e99b94`  
		Last Modified: Wed, 13 Oct 2021 16:52:47 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9d592c69e42daa6af96a5f10527613dd7b8fa0c13680bec1793102a4cb6c`  
		Last Modified: Wed, 13 Oct 2021 16:52:47 GMT  
		Size: 27.5 KB (27510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acea0286906650512214195c73804dc02be6eb85281b5f824954e33d03faf8c5`  
		Last Modified: Fri, 22 Oct 2021 18:52:03 GMT  
		Size: 97.0 MB (96980875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013c201ce81426068fda0857b78408afa6dc52f71809f3d8a04a5f6d26991fae`  
		Last Modified: Fri, 22 Oct 2021 18:51:54 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9582ee77a4bfcc7cdba3bcbc049ca127893af6a567f07ec9d9461c1163863327`  
		Last Modified: Fri, 22 Oct 2021 18:51:54 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.9.7`

**does not exist** (yet?)

## `convertigo:latest`

```console
$ docker pull convertigo@sha256:bd21d6ac291fd7259d25f9a094a0a0a19ed63dcb34f074959a98f42f381761e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `convertigo:latest` - linux; amd64

```console
$ docker pull convertigo@sha256:dee61c2380267082c1757bc073e1cb5a62c06e87dd1dd6ff69e1cdbf06d77d6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.3 MB (437259508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955e61c9685f6822af07fcd66d44b8e7285640c211c60eb86b7f541806adbd0c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:30 GMT
ADD file:aea313ae50ce6474a3df142b34d4dcba4e7e0186ea6fe55389cb2ea903b9ebbb in / 
# Tue, 12 Oct 2021 01:20:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:42:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:42:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:42:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				binutils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:30:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 12 Oct 2021 16:30:49 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 16:30:49 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:30:49 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 12 Oct 2021 16:31:02 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 12 Oct 2021 16:31:02 GMT
CMD ["jshell"]
# Wed, 13 Oct 2021 13:58:47 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 13 Oct 2021 13:58:47 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 13:58:48 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 13 Oct 2021 13:58:48 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Oct 2021 13:58:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 13 Oct 2021 13:58:48 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 13 Oct 2021 14:20:20 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 13 Oct 2021 14:20:20 GMT
ENV TOMCAT_MAJOR=9
# Wed, 13 Oct 2021 14:20:20 GMT
ENV TOMCAT_VERSION=9.0.54
# Wed, 13 Oct 2021 14:20:20 GMT
ENV TOMCAT_SHA512=83430f24d42186ce2ff51eeef2f7a5517048f37d9050c45cac1e3dba8926d61a1f7f5aba122a34a11ac1dbdd3c1f6d98671841047df139394d43751263de57c3
# Wed, 13 Oct 2021 14:20:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Wed, 13 Oct 2021 14:20:48 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 13 Oct 2021 14:20:48 GMT
EXPOSE 8080
# Wed, 13 Oct 2021 14:20:48 GMT
CMD ["catalina.sh" "run"]
# Wed, 13 Oct 2021 16:52:00 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 13 Oct 2021 16:52:00 GMT
ENV SWT_GTK3=0
# Wed, 13 Oct 2021 16:52:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 13 Oct 2021 16:52:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 13 Oct 2021 16:52:01 GMT
WORKDIR /usr/local/tomcat
# Wed, 13 Oct 2021 16:52:05 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     sudo     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 16:52:06 GMT
ENV GOSU_VERSION=1.12
# Wed, 13 Oct 2021 16:52:06 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 13 Oct 2021 16:52:06 GMT
ENV TINI_VERSION=0.19.0
# Wed, 13 Oct 2021 16:52:06 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 13 Oct 2021 16:52:21 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 13 Oct 2021 16:52:22 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Wed, 13 Oct 2021 16:52:23 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Fri, 22 Oct 2021 18:51:21 GMT
ENV CONVERTIGO_VERSION=7.9.6
# Fri, 22 Oct 2021 18:51:21 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.9.6/convertigo-7.9.6.war
# Fri, 22 Oct 2021 18:51:22 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Fri, 22 Oct 2021 18:51:37 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Fri, 22 Oct 2021 18:51:37 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Fri, 22 Oct 2021 18:51:38 GMT
COPY file:ba6487fa7ec71ffccfe3babd0fb02dea602edf66ffef39f9ab084bdb887562ab in / 
# Fri, 22 Oct 2021 18:51:38 GMT
WORKDIR /workspace
# Fri, 22 Oct 2021 18:51:39 GMT
VOLUME [/workspace]
# Fri, 22 Oct 2021 18:51:39 GMT
EXPOSE 28080
# Fri, 22 Oct 2021 18:51:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:51:40 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:bb7d5a84853b217ac05783963f12b034243070c1c9c8d2e60ada47444f3cce04`  
		Last Modified: Tue, 12 Oct 2021 01:25:37 GMT  
		Size: 54.9 MB (54917520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02b617c6a8c415a175f44d7e2c5d3b521059f2a6112c5f022e005a44a759f2d`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 5.2 MB (5153273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e17419b7ee61bbd89c2f0d2833a99cf45e594257d15cb567e4cf7771ce34a`  
		Last Modified: Tue, 12 Oct 2021 15:52:48 GMT  
		Size: 10.9 MB (10871935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d2d81226a43a97871acd5afb7e8aabfad4d6b62ae1709c870df3ee230bc3f5`  
		Last Modified: Tue, 12 Oct 2021 15:53:13 GMT  
		Size: 54.6 MB (54567761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae81fdbbf50b4f75c539f7e4ab9fa83b3fbad9f297ed467c5b05cae3a83872`  
		Last Modified: Tue, 12 Oct 2021 16:42:23 GMT  
		Size: 14.1 MB (14071834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8599b41b2126b88acab21fe05ba39f0c5e0460888a5802a6f01364d174e1a894`  
		Last Modified: Tue, 12 Oct 2021 16:47:51 GMT  
		Size: 184.9 MB (184917431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0265ed527e0a2d6a80207c67db71d5ee448d994032d02b003b5ac86e98a80bab`  
		Last Modified: Wed, 13 Oct 2021 14:59:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8cb15ba3e1704f41d31bbaabe400fe82b236467ffec47787416adfe803e280`  
		Last Modified: Wed, 13 Oct 2021 15:15:56 GMT  
		Size: 12.5 MB (12520349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818a96a178f2ed136ffd4d0c74cc5e52e19a8404f9f61f20c88ff5faff8d94ab`  
		Last Modified: Wed, 13 Oct 2021 15:15:55 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd112ceb86f46712e07b8e3a9ef5f661f3ac0d8f6547e86bda901d0bfb2e8189`  
		Last Modified: Wed, 13 Oct 2021 16:52:50 GMT  
		Size: 2.3 MB (2254050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daa7ff6f117459609e7832801cdfbdbe10586444dd02b9f2e1dd62b2ca29d50`  
		Last Modified: Wed, 13 Oct 2021 16:52:50 GMT  
		Size: 970.4 KB (970354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cafe172bdcfbaef6d7bca6814910bf6d97553d53afa8bbf3903e82e8f9e99b94`  
		Last Modified: Wed, 13 Oct 2021 16:52:47 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be9d592c69e42daa6af96a5f10527613dd7b8fa0c13680bec1793102a4cb6c`  
		Last Modified: Wed, 13 Oct 2021 16:52:47 GMT  
		Size: 27.5 KB (27510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acea0286906650512214195c73804dc02be6eb85281b5f824954e33d03faf8c5`  
		Last Modified: Fri, 22 Oct 2021 18:52:03 GMT  
		Size: 97.0 MB (96980875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013c201ce81426068fda0857b78408afa6dc52f71809f3d8a04a5f6d26991fae`  
		Last Modified: Fri, 22 Oct 2021 18:51:54 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9582ee77a4bfcc7cdba3bcbc049ca127893af6a567f07ec9d9461c1163863327`  
		Last Modified: Fri, 22 Oct 2021 18:51:54 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
