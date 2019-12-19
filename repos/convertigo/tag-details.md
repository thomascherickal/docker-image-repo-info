<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `convertigo`

-	[`convertigo:7.6`](#convertigo76)
-	[`convertigo:7.6.6`](#convertigo766)
-	[`convertigo:7.6.6-openj9`](#convertigo766-openj9)
-	[`convertigo:7.6.6-slim`](#convertigo766-slim)
-	[`convertigo:7.6-openj9`](#convertigo76-openj9)
-	[`convertigo:7.6-slim`](#convertigo76-slim)
-	[`convertigo:latest`](#convertigolatest)
-	[`convertigo:openj9`](#convertigoopenj9)
-	[`convertigo:slim`](#convertigoslim)

## `convertigo:7.6`

```console
$ docker pull convertigo@sha256:c76c6abe359dfcd995e958ee23a52a349b8807257f11639a577af221a1c9f39d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.6` - linux; amd64

```console
$ docker pull convertigo@sha256:630a90c96c97f1f7b82663aede586d205a0ed831eea38c9d57bdba4d2fe91ee7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319412221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9986a2fd85029426575472a0236f4093197a6dba3a21c9e4eb84973a4588b020`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:33:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:33:06 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 14:34:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sat, 23 Nov 2019 14:34:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 14:34:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_VERSION=8u232
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_URL_VERSION=8u232b09
# Sat, 23 Nov 2019 14:34:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 23 Nov 2019 16:34:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 23 Nov 2019 16:34:55 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 16:34:56 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 23 Nov 2019 16:34:56 GMT
WORKDIR /usr/local/tomcat
# Sat, 23 Nov 2019 16:34:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 23 Nov 2019 16:34:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 23 Nov 2019 16:36:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 23 Nov 2019 16:37:30 GMT
ENV TOMCAT_MAJOR=7
# Wed, 18 Dec 2019 01:08:44 GMT
ENV TOMCAT_VERSION=7.0.99
# Wed, 18 Dec 2019 01:08:45 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Wed, 18 Dec 2019 01:09:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 18 Dec 2019 01:09:26 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 Dec 2019 01:09:27 GMT
EXPOSE 8080
# Wed, 18 Dec 2019 01:09:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 18 Dec 2019 02:16:59 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 18 Dec 2019 02:16:59 GMT
ENV SWT_GTK3=0
# Wed, 18 Dec 2019 02:16:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 18 Dec 2019 02:17:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 18 Dec 2019 02:17:00 GMT
WORKDIR /usr/local/tomcat
# Wed, 18 Dec 2019 02:17:04 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 02:17:04 GMT
ENV GOSU_VERSION=1.11
# Wed, 18 Dec 2019 02:17:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 18 Dec 2019 02:17:05 GMT
ENV TINI_VERSION=0.18.0
# Wed, 18 Dec 2019 02:17:05 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 18 Dec 2019 02:17:08 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 18 Dec 2019 02:17:09 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Wed, 18 Dec 2019 02:17:10 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Wed, 18 Dec 2019 02:17:10 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Wed, 18 Dec 2019 02:17:10 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Wed, 18 Dec 2019 02:17:11 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Wed, 18 Dec 2019 02:17:18 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Wed, 18 Dec 2019 02:17:18 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Wed, 18 Dec 2019 02:17:18 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Wed, 18 Dec 2019 02:17:18 GMT
WORKDIR /workspace
# Wed, 18 Dec 2019 02:17:18 GMT
VOLUME [/workspace]
# Wed, 18 Dec 2019 02:17:19 GMT
EXPOSE 28080
# Wed, 18 Dec 2019 02:17:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 18 Dec 2019 02:17:19 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b8714e12252c8e30fe9516a8faad25304c538faec9028f46be3968fc4019eb`  
		Last Modified: Sat, 23 Nov 2019 14:36:38 GMT  
		Size: 4.9 MB (4935448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b12da521a3f59151151c374fe154d71a118abddbda8586a1c4ba409b84e7d8`  
		Last Modified: Sat, 23 Nov 2019 14:37:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38df533772dd0403b864aaf3c8f11695dcc54d7e9414b93d6454899fdfc6d7`  
		Last Modified: Sat, 23 Nov 2019 14:37:29 GMT  
		Size: 104.2 MB (104167822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4144d55bbb47c20b373d5f1d427d791de8cfda56d3dfe50e76e40f03d69b2fa3`  
		Last Modified: Sat, 23 Nov 2019 16:39:08 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deca9573f6432e90cc0c5bbe95732f49f4ce56964acc281cd984d8d9a0f14ff`  
		Last Modified: Wed, 18 Dec 2019 02:00:36 GMT  
		Size: 10.5 MB (10506039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6784e1f4b81286ceb35e6f2a74b3de9a0008fc243d101a22cd982c8dea1c1ce`  
		Last Modified: Wed, 18 Dec 2019 02:00:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad80e4895f030b24d54ef5571c9dcf07b06f918294d424c9ac94887512886f61`  
		Last Modified: Wed, 18 Dec 2019 02:18:21 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ad94f8473909725d900f508e9fac63ae906eb8dcaf4118a066a54275de6ad2`  
		Last Modified: Wed, 18 Dec 2019 02:18:21 GMT  
		Size: 910.1 KB (910111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539fc3cc1de2c5258e3a3a84b32f506346bde1776b0452e46e933c679b68d479`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 4.3 KB (4278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3414478a34c0a02ee3c06cd10b2b464e170858a8b0ec187a2714cb2590f3c4`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 26.8 KB (26787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4e966890083fa994ad65b77f280e286cd79dbc4f2f6145dd029f12198eff15`  
		Last Modified: Wed, 18 Dec 2019 02:18:29 GMT  
		Size: 88.3 MB (88275804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8eee4ea9bce42c7b3860c2b976579670bf44b4fad1da1c40789bdff8902fae`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae23c93d53a7111718447fa52fcf4f17498dd424c48be1d1271968f03097362`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.6.6`

```console
$ docker pull convertigo@sha256:c76c6abe359dfcd995e958ee23a52a349b8807257f11639a577af221a1c9f39d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.6.6` - linux; amd64

```console
$ docker pull convertigo@sha256:630a90c96c97f1f7b82663aede586d205a0ed831eea38c9d57bdba4d2fe91ee7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319412221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9986a2fd85029426575472a0236f4093197a6dba3a21c9e4eb84973a4588b020`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:33:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:33:06 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 14:34:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sat, 23 Nov 2019 14:34:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 14:34:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_VERSION=8u232
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_URL_VERSION=8u232b09
# Sat, 23 Nov 2019 14:34:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 23 Nov 2019 16:34:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 23 Nov 2019 16:34:55 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 16:34:56 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 23 Nov 2019 16:34:56 GMT
WORKDIR /usr/local/tomcat
# Sat, 23 Nov 2019 16:34:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 23 Nov 2019 16:34:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 23 Nov 2019 16:36:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 23 Nov 2019 16:37:30 GMT
ENV TOMCAT_MAJOR=7
# Wed, 18 Dec 2019 01:08:44 GMT
ENV TOMCAT_VERSION=7.0.99
# Wed, 18 Dec 2019 01:08:45 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Wed, 18 Dec 2019 01:09:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 18 Dec 2019 01:09:26 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 Dec 2019 01:09:27 GMT
EXPOSE 8080
# Wed, 18 Dec 2019 01:09:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 18 Dec 2019 02:16:59 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 18 Dec 2019 02:16:59 GMT
ENV SWT_GTK3=0
# Wed, 18 Dec 2019 02:16:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 18 Dec 2019 02:17:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 18 Dec 2019 02:17:00 GMT
WORKDIR /usr/local/tomcat
# Wed, 18 Dec 2019 02:17:04 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 02:17:04 GMT
ENV GOSU_VERSION=1.11
# Wed, 18 Dec 2019 02:17:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 18 Dec 2019 02:17:05 GMT
ENV TINI_VERSION=0.18.0
# Wed, 18 Dec 2019 02:17:05 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 18 Dec 2019 02:17:08 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 18 Dec 2019 02:17:09 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Wed, 18 Dec 2019 02:17:10 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Wed, 18 Dec 2019 02:17:10 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Wed, 18 Dec 2019 02:17:10 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Wed, 18 Dec 2019 02:17:11 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Wed, 18 Dec 2019 02:17:18 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Wed, 18 Dec 2019 02:17:18 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Wed, 18 Dec 2019 02:17:18 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Wed, 18 Dec 2019 02:17:18 GMT
WORKDIR /workspace
# Wed, 18 Dec 2019 02:17:18 GMT
VOLUME [/workspace]
# Wed, 18 Dec 2019 02:17:19 GMT
EXPOSE 28080
# Wed, 18 Dec 2019 02:17:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 18 Dec 2019 02:17:19 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b8714e12252c8e30fe9516a8faad25304c538faec9028f46be3968fc4019eb`  
		Last Modified: Sat, 23 Nov 2019 14:36:38 GMT  
		Size: 4.9 MB (4935448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b12da521a3f59151151c374fe154d71a118abddbda8586a1c4ba409b84e7d8`  
		Last Modified: Sat, 23 Nov 2019 14:37:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38df533772dd0403b864aaf3c8f11695dcc54d7e9414b93d6454899fdfc6d7`  
		Last Modified: Sat, 23 Nov 2019 14:37:29 GMT  
		Size: 104.2 MB (104167822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4144d55bbb47c20b373d5f1d427d791de8cfda56d3dfe50e76e40f03d69b2fa3`  
		Last Modified: Sat, 23 Nov 2019 16:39:08 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deca9573f6432e90cc0c5bbe95732f49f4ce56964acc281cd984d8d9a0f14ff`  
		Last Modified: Wed, 18 Dec 2019 02:00:36 GMT  
		Size: 10.5 MB (10506039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6784e1f4b81286ceb35e6f2a74b3de9a0008fc243d101a22cd982c8dea1c1ce`  
		Last Modified: Wed, 18 Dec 2019 02:00:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad80e4895f030b24d54ef5571c9dcf07b06f918294d424c9ac94887512886f61`  
		Last Modified: Wed, 18 Dec 2019 02:18:21 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ad94f8473909725d900f508e9fac63ae906eb8dcaf4118a066a54275de6ad2`  
		Last Modified: Wed, 18 Dec 2019 02:18:21 GMT  
		Size: 910.1 KB (910111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539fc3cc1de2c5258e3a3a84b32f506346bde1776b0452e46e933c679b68d479`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 4.3 KB (4278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3414478a34c0a02ee3c06cd10b2b464e170858a8b0ec187a2714cb2590f3c4`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 26.8 KB (26787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4e966890083fa994ad65b77f280e286cd79dbc4f2f6145dd029f12198eff15`  
		Last Modified: Wed, 18 Dec 2019 02:18:29 GMT  
		Size: 88.3 MB (88275804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8eee4ea9bce42c7b3860c2b976579670bf44b4fad1da1c40789bdff8902fae`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae23c93d53a7111718447fa52fcf4f17498dd424c48be1d1271968f03097362`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.6.6-openj9`

```console
$ docker pull convertigo@sha256:957ef78f6ecde54a40a493ae17627e02507e94b87e03231db7208b68e7fff81c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.6.6-openj9` - linux; amd64

```console
$ docker pull convertigo@sha256:9206f7423a573ab0c634ef4f0661c828ca48d6acb8a1f6202ee90ef92c0656ed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259524812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f086fb58e5ad0437874768daf85b7666ed42bafce42acc08174d8c6824e2f48b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:43:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 19 Dec 2019 06:44:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:45:32 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Thu, 19 Dec 2019 06:45:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='c746f26d37bc982d8a6ae76139f9e797205e4243b8f944eb3961f3ac9e69521e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_ppc64le_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        s390x)          ESUM='6348ccfc7764fde558a461e36de4342ac0f480d17c76dfc1bc9b6e1477f9dc5b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_s390x_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        amd64|x86_64)          ESUM='abea758c7e102f3c4a3be8757ee0ce039a70e2d498c160400dfb83c6f7004dbf';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_x64_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:45:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:45:41 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 19 Dec 2019 09:59:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:59:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:59:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:59:01 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:59:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:59:01 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:02:44 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_MAJOR=7
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_VERSION=7.0.99
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Thu, 19 Dec 2019 10:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:04:47 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:04:47 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:04:48 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:30:07 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 19 Dec 2019 11:30:07 GMT
ENV SWT_GTK3=0
# Thu, 19 Dec 2019 11:30:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 11:30:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 11:30:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 11:30:16 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:30:17 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 11:30:17 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 19 Dec 2019 11:30:17 GMT
ENV TINI_VERSION=0.18.0
# Thu, 19 Dec 2019 11:30:17 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 19 Dec 2019 11:30:19 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 19 Dec 2019 11:30:20 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Thu, 19 Dec 2019 11:30:21 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 19 Dec 2019 11:30:21 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Thu, 19 Dec 2019 11:30:21 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Thu, 19 Dec 2019 11:30:22 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 19 Dec 2019 11:30:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 19 Dec 2019 11:30:27 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Thu, 19 Dec 2019 11:30:27 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Thu, 19 Dec 2019 11:30:27 GMT
WORKDIR /workspace
# Thu, 19 Dec 2019 11:30:28 GMT
VOLUME [/workspace]
# Thu, 19 Dec 2019 11:30:28 GMT
EXPOSE 28080
# Thu, 19 Dec 2019 11:30:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:30:28 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ff21ce7d875874bffbded53d145025fc53273ed43e60390bfb159ce785b0aa`  
		Last Modified: Thu, 19 Dec 2019 06:47:19 GMT  
		Size: 13.3 MB (13323051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98228726cf4e543f070f7948b8a1513c6ba5ab7868aa0798fa4c07b27584635`  
		Last Modified: Thu, 19 Dec 2019 06:49:11 GMT  
		Size: 116.5 MB (116540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2c6eb7ae14aa46119e71bd76cf1f34d47e8bfe8f1c48b87f16e4b5a8d8a44`  
		Last Modified: Thu, 19 Dec 2019 10:05:54 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8365a757ce8137f1dbb2d4fc2702c0d843a9f1f86d2354aac6997a6516d78d2`  
		Last Modified: Thu, 19 Dec 2019 10:06:38 GMT  
		Size: 10.6 MB (10570591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84008f6e939a9b738e558be70e3177e1d77d47bc29550aaef91392c4766d4739`  
		Last Modified: Thu, 19 Dec 2019 10:06:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d1e79c0451fefd37dc57170b2e677fbe975d489aaf3f65ed133e795d1dc45`  
		Last Modified: Thu, 19 Dec 2019 11:30:41 GMT  
		Size: 3.1 MB (3145992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b241b0b827643d49ad7c465dbcca697eb5f874b459263f2570a79832c8be1a4`  
		Last Modified: Thu, 19 Dec 2019 11:30:41 GMT  
		Size: 910.0 KB (910029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a85315ec145819eff954cb12f5fd45fb38c3cbdadf778e2748020a1b3517132`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 4.6 KB (4608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8902b38e1df43741e86c3ae67fd17280a6f94c607054b935ca6176a88924ddef`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 26.8 KB (26768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c036842f7853ca602b0c3c2f6eb8f7a18b6f6205badaec7582bf523c759ae6a`  
		Last Modified: Thu, 19 Dec 2019 11:30:47 GMT  
		Size: 88.3 MB (88275811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df541108e281f234aac619f39d5cbe688d1d4ec78558059f713c6316ca4840d9`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eb5b5a1b8dcb91d8fc43276a5c3bbe7e0fce2c9b1fe9c87fea974ce55000d0`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.6.6-slim`

```console
$ docker pull convertigo@sha256:84a3bcbc4d5b1165d20c915943f7a145180a4aed828603c9a2d3ab67907d69b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.6.6-slim` - linux; amd64

```console
$ docker pull convertigo@sha256:c41129e357ae8247d4bef163b6357172c9a21e01a4074aa4f03cd48a55f0b4c3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.4 MB (240418803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:559599fc3be6e43407fd1f91f3190f32dae663b6f66e0bfefb7170068a1c8885`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 19:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 19:14:45 GMT
ENV LANG=C.UTF-8
# Fri, 22 Nov 2019 19:17:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 22 Nov 2019 19:17:21 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 19:17:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_VERSION=8u232
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_URL_VERSION=8u232b09
# Fri, 22 Nov 2019 19:17:38 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 22 Nov 2019 22:44:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 22 Nov 2019 22:44:17 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 22:44:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 22 Nov 2019 22:44:18 GMT
WORKDIR /usr/local/tomcat
# Fri, 22 Nov 2019 22:44:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 22 Nov 2019 22:44:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 22 Nov 2019 22:46:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 22 Nov 2019 22:47:28 GMT
ENV TOMCAT_MAJOR=7
# Wed, 18 Dec 2019 01:09:38 GMT
ENV TOMCAT_VERSION=7.0.99
# Wed, 18 Dec 2019 01:09:38 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Wed, 18 Dec 2019 01:55:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 18 Dec 2019 01:55:50 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 Dec 2019 01:55:50 GMT
EXPOSE 8080
# Wed, 18 Dec 2019 01:55:50 GMT
CMD ["catalina.sh" "run"]
# Wed, 18 Dec 2019 02:17:23 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 18 Dec 2019 02:17:23 GMT
ENV SWT_GTK3=0
# Wed, 18 Dec 2019 02:17:23 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 18 Dec 2019 02:17:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 18 Dec 2019 02:17:24 GMT
WORKDIR /usr/local/tomcat
# Wed, 18 Dec 2019 02:17:31 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 02:17:31 GMT
ENV GOSU_VERSION=1.11
# Wed, 18 Dec 2019 02:17:32 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 18 Dec 2019 02:17:32 GMT
ENV TINI_VERSION=0.18.0
# Wed, 18 Dec 2019 02:17:32 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 18 Dec 2019 02:17:34 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 18 Dec 2019 02:17:35 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Wed, 18 Dec 2019 02:17:35 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Wed, 18 Dec 2019 02:17:41 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Wed, 18 Dec 2019 02:17:41 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Wed, 18 Dec 2019 02:17:41 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Wed, 18 Dec 2019 02:17:41 GMT
WORKDIR /workspace
# Wed, 18 Dec 2019 02:17:42 GMT
VOLUME [/workspace]
# Wed, 18 Dec 2019 02:17:42 GMT
EXPOSE 28080
# Wed, 18 Dec 2019 02:17:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 18 Dec 2019 02:17:42 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dc2bdcfe193ce54affa45170354ca76667c40f8cf536b6282dd379e17e24a`  
		Last Modified: Fri, 22 Nov 2019 19:19:08 GMT  
		Size: 3.2 MB (3249119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a806caa98c159f2c9254dabd60e04352b5c8b46d2e6cc9bd8f7bfc037a4e0b`  
		Last Modified: Fri, 22 Nov 2019 19:21:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5943b75c9747aebea25c3fc4bf3d4b4247101176b78ada93d08446dd33f94a0`  
		Last Modified: Fri, 22 Nov 2019 19:21:41 GMT  
		Size: 104.4 MB (104425948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d036bf1b384d6cddf3f1f57b9074d17d6c5d5d142471c63951c3fb7605dbc9`  
		Last Modified: Fri, 22 Nov 2019 22:49:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24c49bbca7a82b1b61cc4c2f27c5a2201b01456a3a98a918e7310ee84041967`  
		Last Modified: Wed, 18 Dec 2019 02:00:50 GMT  
		Size: 10.6 MB (10627739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5364727b9eb8c619c3f089508caccaacc88c1945b426b58779d01ecf9d23d3`  
		Last Modified: Wed, 18 Dec 2019 02:00:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e978d1d04ff84885234fce69dd5c96f1c4a96819fd428d481c8939df7593c25e`  
		Last Modified: Wed, 18 Dec 2019 02:18:39 GMT  
		Size: 5.8 MB (5804209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c150b799e57ad5eca58fbdc22b23f61db56bcab317a49cb4b4fb3728f1eb029`  
		Last Modified: Wed, 18 Dec 2019 02:18:37 GMT  
		Size: 910.1 KB (910076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fa8067fad712950b3a28f8fe1db3dee6b616902aeefa138cd22316473a2a15`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 4.3 KB (4277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1446835a60b437b63b05098b4613a58eac7f0b3b9980221ab353f1a2e918665f`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 26.8 KB (26766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d829d2bec0530fcb07f6d4b8385952dd35eded456f0e06a41fd247f9c0555b4`  
		Last Modified: Wed, 18 Dec 2019 02:18:43 GMT  
		Size: 88.3 MB (88275827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cbe117219f35147a5f976a14a2de8103d2bc584d82d1a0aefb3a0624a05774`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5675557825083e74a819893eb15a740570501e8ce83ccd781019802a948f4a`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.6-openj9`

```console
$ docker pull convertigo@sha256:957ef78f6ecde54a40a493ae17627e02507e94b87e03231db7208b68e7fff81c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.6-openj9` - linux; amd64

```console
$ docker pull convertigo@sha256:9206f7423a573ab0c634ef4f0661c828ca48d6acb8a1f6202ee90ef92c0656ed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259524812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f086fb58e5ad0437874768daf85b7666ed42bafce42acc08174d8c6824e2f48b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:43:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 19 Dec 2019 06:44:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:45:32 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Thu, 19 Dec 2019 06:45:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='c746f26d37bc982d8a6ae76139f9e797205e4243b8f944eb3961f3ac9e69521e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_ppc64le_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        s390x)          ESUM='6348ccfc7764fde558a461e36de4342ac0f480d17c76dfc1bc9b6e1477f9dc5b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_s390x_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        amd64|x86_64)          ESUM='abea758c7e102f3c4a3be8757ee0ce039a70e2d498c160400dfb83c6f7004dbf';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_x64_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:45:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:45:41 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 19 Dec 2019 09:59:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:59:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:59:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:59:01 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:59:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:59:01 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:02:44 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_MAJOR=7
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_VERSION=7.0.99
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Thu, 19 Dec 2019 10:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:04:47 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:04:47 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:04:48 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:30:07 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 19 Dec 2019 11:30:07 GMT
ENV SWT_GTK3=0
# Thu, 19 Dec 2019 11:30:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 11:30:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 11:30:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 11:30:16 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:30:17 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 11:30:17 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 19 Dec 2019 11:30:17 GMT
ENV TINI_VERSION=0.18.0
# Thu, 19 Dec 2019 11:30:17 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 19 Dec 2019 11:30:19 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 19 Dec 2019 11:30:20 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Thu, 19 Dec 2019 11:30:21 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 19 Dec 2019 11:30:21 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Thu, 19 Dec 2019 11:30:21 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Thu, 19 Dec 2019 11:30:22 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 19 Dec 2019 11:30:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 19 Dec 2019 11:30:27 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Thu, 19 Dec 2019 11:30:27 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Thu, 19 Dec 2019 11:30:27 GMT
WORKDIR /workspace
# Thu, 19 Dec 2019 11:30:28 GMT
VOLUME [/workspace]
# Thu, 19 Dec 2019 11:30:28 GMT
EXPOSE 28080
# Thu, 19 Dec 2019 11:30:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:30:28 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ff21ce7d875874bffbded53d145025fc53273ed43e60390bfb159ce785b0aa`  
		Last Modified: Thu, 19 Dec 2019 06:47:19 GMT  
		Size: 13.3 MB (13323051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98228726cf4e543f070f7948b8a1513c6ba5ab7868aa0798fa4c07b27584635`  
		Last Modified: Thu, 19 Dec 2019 06:49:11 GMT  
		Size: 116.5 MB (116540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2c6eb7ae14aa46119e71bd76cf1f34d47e8bfe8f1c48b87f16e4b5a8d8a44`  
		Last Modified: Thu, 19 Dec 2019 10:05:54 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8365a757ce8137f1dbb2d4fc2702c0d843a9f1f86d2354aac6997a6516d78d2`  
		Last Modified: Thu, 19 Dec 2019 10:06:38 GMT  
		Size: 10.6 MB (10570591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84008f6e939a9b738e558be70e3177e1d77d47bc29550aaef91392c4766d4739`  
		Last Modified: Thu, 19 Dec 2019 10:06:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d1e79c0451fefd37dc57170b2e677fbe975d489aaf3f65ed133e795d1dc45`  
		Last Modified: Thu, 19 Dec 2019 11:30:41 GMT  
		Size: 3.1 MB (3145992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b241b0b827643d49ad7c465dbcca697eb5f874b459263f2570a79832c8be1a4`  
		Last Modified: Thu, 19 Dec 2019 11:30:41 GMT  
		Size: 910.0 KB (910029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a85315ec145819eff954cb12f5fd45fb38c3cbdadf778e2748020a1b3517132`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 4.6 KB (4608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8902b38e1df43741e86c3ae67fd17280a6f94c607054b935ca6176a88924ddef`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 26.8 KB (26768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c036842f7853ca602b0c3c2f6eb8f7a18b6f6205badaec7582bf523c759ae6a`  
		Last Modified: Thu, 19 Dec 2019 11:30:47 GMT  
		Size: 88.3 MB (88275811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df541108e281f234aac619f39d5cbe688d1d4ec78558059f713c6316ca4840d9`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eb5b5a1b8dcb91d8fc43276a5c3bbe7e0fce2c9b1fe9c87fea974ce55000d0`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.6-slim`

```console
$ docker pull convertigo@sha256:84a3bcbc4d5b1165d20c915943f7a145180a4aed828603c9a2d3ab67907d69b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.6-slim` - linux; amd64

```console
$ docker pull convertigo@sha256:c41129e357ae8247d4bef163b6357172c9a21e01a4074aa4f03cd48a55f0b4c3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.4 MB (240418803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:559599fc3be6e43407fd1f91f3190f32dae663b6f66e0bfefb7170068a1c8885`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 19:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 19:14:45 GMT
ENV LANG=C.UTF-8
# Fri, 22 Nov 2019 19:17:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 22 Nov 2019 19:17:21 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 19:17:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_VERSION=8u232
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_URL_VERSION=8u232b09
# Fri, 22 Nov 2019 19:17:38 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 22 Nov 2019 22:44:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 22 Nov 2019 22:44:17 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 22:44:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 22 Nov 2019 22:44:18 GMT
WORKDIR /usr/local/tomcat
# Fri, 22 Nov 2019 22:44:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 22 Nov 2019 22:44:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 22 Nov 2019 22:46:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 22 Nov 2019 22:47:28 GMT
ENV TOMCAT_MAJOR=7
# Wed, 18 Dec 2019 01:09:38 GMT
ENV TOMCAT_VERSION=7.0.99
# Wed, 18 Dec 2019 01:09:38 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Wed, 18 Dec 2019 01:55:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 18 Dec 2019 01:55:50 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 Dec 2019 01:55:50 GMT
EXPOSE 8080
# Wed, 18 Dec 2019 01:55:50 GMT
CMD ["catalina.sh" "run"]
# Wed, 18 Dec 2019 02:17:23 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 18 Dec 2019 02:17:23 GMT
ENV SWT_GTK3=0
# Wed, 18 Dec 2019 02:17:23 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 18 Dec 2019 02:17:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 18 Dec 2019 02:17:24 GMT
WORKDIR /usr/local/tomcat
# Wed, 18 Dec 2019 02:17:31 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 02:17:31 GMT
ENV GOSU_VERSION=1.11
# Wed, 18 Dec 2019 02:17:32 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 18 Dec 2019 02:17:32 GMT
ENV TINI_VERSION=0.18.0
# Wed, 18 Dec 2019 02:17:32 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 18 Dec 2019 02:17:34 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 18 Dec 2019 02:17:35 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Wed, 18 Dec 2019 02:17:35 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Wed, 18 Dec 2019 02:17:41 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Wed, 18 Dec 2019 02:17:41 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Wed, 18 Dec 2019 02:17:41 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Wed, 18 Dec 2019 02:17:41 GMT
WORKDIR /workspace
# Wed, 18 Dec 2019 02:17:42 GMT
VOLUME [/workspace]
# Wed, 18 Dec 2019 02:17:42 GMT
EXPOSE 28080
# Wed, 18 Dec 2019 02:17:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 18 Dec 2019 02:17:42 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dc2bdcfe193ce54affa45170354ca76667c40f8cf536b6282dd379e17e24a`  
		Last Modified: Fri, 22 Nov 2019 19:19:08 GMT  
		Size: 3.2 MB (3249119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a806caa98c159f2c9254dabd60e04352b5c8b46d2e6cc9bd8f7bfc037a4e0b`  
		Last Modified: Fri, 22 Nov 2019 19:21:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5943b75c9747aebea25c3fc4bf3d4b4247101176b78ada93d08446dd33f94a0`  
		Last Modified: Fri, 22 Nov 2019 19:21:41 GMT  
		Size: 104.4 MB (104425948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d036bf1b384d6cddf3f1f57b9074d17d6c5d5d142471c63951c3fb7605dbc9`  
		Last Modified: Fri, 22 Nov 2019 22:49:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24c49bbca7a82b1b61cc4c2f27c5a2201b01456a3a98a918e7310ee84041967`  
		Last Modified: Wed, 18 Dec 2019 02:00:50 GMT  
		Size: 10.6 MB (10627739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5364727b9eb8c619c3f089508caccaacc88c1945b426b58779d01ecf9d23d3`  
		Last Modified: Wed, 18 Dec 2019 02:00:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e978d1d04ff84885234fce69dd5c96f1c4a96819fd428d481c8939df7593c25e`  
		Last Modified: Wed, 18 Dec 2019 02:18:39 GMT  
		Size: 5.8 MB (5804209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c150b799e57ad5eca58fbdc22b23f61db56bcab317a49cb4b4fb3728f1eb029`  
		Last Modified: Wed, 18 Dec 2019 02:18:37 GMT  
		Size: 910.1 KB (910076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fa8067fad712950b3a28f8fe1db3dee6b616902aeefa138cd22316473a2a15`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 4.3 KB (4277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1446835a60b437b63b05098b4613a58eac7f0b3b9980221ab353f1a2e918665f`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 26.8 KB (26766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d829d2bec0530fcb07f6d4b8385952dd35eded456f0e06a41fd247f9c0555b4`  
		Last Modified: Wed, 18 Dec 2019 02:18:43 GMT  
		Size: 88.3 MB (88275827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cbe117219f35147a5f976a14a2de8103d2bc584d82d1a0aefb3a0624a05774`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5675557825083e74a819893eb15a740570501e8ce83ccd781019802a948f4a`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:latest`

```console
$ docker pull convertigo@sha256:c76c6abe359dfcd995e958ee23a52a349b8807257f11639a577af221a1c9f39d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:latest` - linux; amd64

```console
$ docker pull convertigo@sha256:630a90c96c97f1f7b82663aede586d205a0ed831eea38c9d57bdba4d2fe91ee7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.4 MB (319412221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9986a2fd85029426575472a0236f4093197a6dba3a21c9e4eb84973a4588b020`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:12:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:13:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:33:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 14:33:06 GMT
ENV LANG=C.UTF-8
# Sat, 23 Nov 2019 14:34:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Sat, 23 Nov 2019 14:34:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 14:34:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_VERSION=8u232
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_
# Sat, 23 Nov 2019 14:34:05 GMT
ENV JAVA_URL_VERSION=8u232b09
# Sat, 23 Nov 2019 14:34:16 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Sat, 23 Nov 2019 16:34:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 23 Nov 2019 16:34:55 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 16:34:56 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 23 Nov 2019 16:34:56 GMT
WORKDIR /usr/local/tomcat
# Sat, 23 Nov 2019 16:34:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 23 Nov 2019 16:34:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 23 Nov 2019 16:36:43 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 23 Nov 2019 16:37:30 GMT
ENV TOMCAT_MAJOR=7
# Wed, 18 Dec 2019 01:08:44 GMT
ENV TOMCAT_VERSION=7.0.99
# Wed, 18 Dec 2019 01:08:45 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Wed, 18 Dec 2019 01:09:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 18 Dec 2019 01:09:26 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 Dec 2019 01:09:27 GMT
EXPOSE 8080
# Wed, 18 Dec 2019 01:09:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 18 Dec 2019 02:16:59 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 18 Dec 2019 02:16:59 GMT
ENV SWT_GTK3=0
# Wed, 18 Dec 2019 02:16:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 18 Dec 2019 02:17:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 18 Dec 2019 02:17:00 GMT
WORKDIR /usr/local/tomcat
# Wed, 18 Dec 2019 02:17:04 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 02:17:04 GMT
ENV GOSU_VERSION=1.11
# Wed, 18 Dec 2019 02:17:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 18 Dec 2019 02:17:05 GMT
ENV TINI_VERSION=0.18.0
# Wed, 18 Dec 2019 02:17:05 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 18 Dec 2019 02:17:08 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 18 Dec 2019 02:17:09 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Wed, 18 Dec 2019 02:17:10 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Wed, 18 Dec 2019 02:17:10 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Wed, 18 Dec 2019 02:17:10 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Wed, 18 Dec 2019 02:17:11 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Wed, 18 Dec 2019 02:17:18 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Wed, 18 Dec 2019 02:17:18 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Wed, 18 Dec 2019 02:17:18 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Wed, 18 Dec 2019 02:17:18 GMT
WORKDIR /workspace
# Wed, 18 Dec 2019 02:17:18 GMT
VOLUME [/workspace]
# Wed, 18 Dec 2019 02:17:19 GMT
EXPOSE 28080
# Wed, 18 Dec 2019 02:17:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 18 Dec 2019 02:17:19 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada5d61ae65dc038b4ba788ae5124c2587d0ebe83d3534733677216547b65cbd`  
		Last Modified: Sat, 23 Nov 2019 00:20:40 GMT  
		Size: 10.8 MB (10796925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8427fdf429235414d0ea4757fd45fd81f09fd2ba3106e13796a8250f0a04a23`  
		Last Modified: Sat, 23 Nov 2019 00:20:39 GMT  
		Size: 4.3 MB (4340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f025bafc4ab87c34cee7bfc43340fa7904dfe6d29a266537f2026cee3a76adfd`  
		Last Modified: Sat, 23 Nov 2019 00:20:56 GMT  
		Size: 50.1 MB (50065503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b8714e12252c8e30fe9516a8faad25304c538faec9028f46be3968fc4019eb`  
		Last Modified: Sat, 23 Nov 2019 14:36:38 GMT  
		Size: 4.9 MB (4935448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b12da521a3f59151151c374fe154d71a118abddbda8586a1c4ba409b84e7d8`  
		Last Modified: Sat, 23 Nov 2019 14:37:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38df533772dd0403b864aaf3c8f11695dcc54d7e9414b93d6454899fdfc6d7`  
		Last Modified: Sat, 23 Nov 2019 14:37:29 GMT  
		Size: 104.2 MB (104167822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4144d55bbb47c20b373d5f1d427d791de8cfda56d3dfe50e76e40f03d69b2fa3`  
		Last Modified: Sat, 23 Nov 2019 16:39:08 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6deca9573f6432e90cc0c5bbe95732f49f4ce56964acc281cd984d8d9a0f14ff`  
		Last Modified: Wed, 18 Dec 2019 02:00:36 GMT  
		Size: 10.5 MB (10506039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6784e1f4b81286ceb35e6f2a74b3de9a0008fc243d101a22cd982c8dea1c1ce`  
		Last Modified: Wed, 18 Dec 2019 02:00:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad80e4895f030b24d54ef5571c9dcf07b06f918294d424c9ac94887512886f61`  
		Last Modified: Wed, 18 Dec 2019 02:18:21 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ad94f8473909725d900f508e9fac63ae906eb8dcaf4118a066a54275de6ad2`  
		Last Modified: Wed, 18 Dec 2019 02:18:21 GMT  
		Size: 910.1 KB (910111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539fc3cc1de2c5258e3a3a84b32f506346bde1776b0452e46e933c679b68d479`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 4.3 KB (4278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3414478a34c0a02ee3c06cd10b2b464e170858a8b0ec187a2714cb2590f3c4`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 26.8 KB (26787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4e966890083fa994ad65b77f280e286cd79dbc4f2f6145dd029f12198eff15`  
		Last Modified: Wed, 18 Dec 2019 02:18:29 GMT  
		Size: 88.3 MB (88275804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8eee4ea9bce42c7b3860c2b976579670bf44b4fad1da1c40789bdff8902fae`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae23c93d53a7111718447fa52fcf4f17498dd424c48be1d1271968f03097362`  
		Last Modified: Wed, 18 Dec 2019 02:18:20 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:openj9`

```console
$ docker pull convertigo@sha256:957ef78f6ecde54a40a493ae17627e02507e94b87e03231db7208b68e7fff81c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:openj9` - linux; amd64

```console
$ docker pull convertigo@sha256:9206f7423a573ab0c634ef4f0661c828ca48d6acb8a1f6202ee90ef92c0656ed
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259524812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f086fb58e5ad0437874768daf85b7666ed42bafce42acc08174d8c6824e2f48b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 06:43:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 19 Dec 2019 06:44:09 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 06:45:32 GMT
ENV JAVA_VERSION=jdk8u232-b09_openj9-0.17.0
# Thu, 19 Dec 2019 06:45:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='c746f26d37bc982d8a6ae76139f9e797205e4243b8f944eb3961f3ac9e69521e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_ppc64le_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        s390x)          ESUM='6348ccfc7764fde558a461e36de4342ac0f480d17c76dfc1bc9b6e1477f9dc5b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_s390x_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        amd64|x86_64)          ESUM='abea758c7e102f3c4a3be8757ee0ce039a70e2d498c160400dfb83c6f7004dbf';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09_openj9-0.17.0/OpenJDK8U-jdk_x64_linux_openj9_8u232b09_openj9-0.17.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:45:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:45:41 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+UseContainerSupport -XX:+IdleTuningCompactOnIdle -XX:+IdleTuningGcOnIdle
# Thu, 19 Dec 2019 09:59:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:59:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:59:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:59:01 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:59:01 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:59:01 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:02:44 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_MAJOR=7
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_VERSION=7.0.99
# Thu, 19 Dec 2019 10:04:13 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Thu, 19 Dec 2019 10:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:04:47 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:04:47 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:04:48 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:30:07 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 19 Dec 2019 11:30:07 GMT
ENV SWT_GTK3=0
# Thu, 19 Dec 2019 11:30:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 11:30:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 11:30:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 11:30:16 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:30:17 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 11:30:17 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 19 Dec 2019 11:30:17 GMT
ENV TINI_VERSION=0.18.0
# Thu, 19 Dec 2019 11:30:17 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 19 Dec 2019 11:30:19 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 19 Dec 2019 11:30:20 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Thu, 19 Dec 2019 11:30:21 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 19 Dec 2019 11:30:21 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Thu, 19 Dec 2019 11:30:21 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Thu, 19 Dec 2019 11:30:22 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 19 Dec 2019 11:30:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 19 Dec 2019 11:30:27 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Thu, 19 Dec 2019 11:30:27 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Thu, 19 Dec 2019 11:30:27 GMT
WORKDIR /workspace
# Thu, 19 Dec 2019 11:30:28 GMT
VOLUME [/workspace]
# Thu, 19 Dec 2019 11:30:28 GMT
EXPOSE 28080
# Thu, 19 Dec 2019 11:30:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:30:28 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ff21ce7d875874bffbded53d145025fc53273ed43e60390bfb159ce785b0aa`  
		Last Modified: Thu, 19 Dec 2019 06:47:19 GMT  
		Size: 13.3 MB (13323051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98228726cf4e543f070f7948b8a1513c6ba5ab7868aa0798fa4c07b27584635`  
		Last Modified: Thu, 19 Dec 2019 06:49:11 GMT  
		Size: 116.5 MB (116540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb2c6eb7ae14aa46119e71bd76cf1f34d47e8bfe8f1c48b87f16e4b5a8d8a44`  
		Last Modified: Thu, 19 Dec 2019 10:05:54 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8365a757ce8137f1dbb2d4fc2702c0d843a9f1f86d2354aac6997a6516d78d2`  
		Last Modified: Thu, 19 Dec 2019 10:06:38 GMT  
		Size: 10.6 MB (10570591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84008f6e939a9b738e558be70e3177e1d77d47bc29550aaef91392c4766d4739`  
		Last Modified: Thu, 19 Dec 2019 10:06:36 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d1e79c0451fefd37dc57170b2e677fbe975d489aaf3f65ed133e795d1dc45`  
		Last Modified: Thu, 19 Dec 2019 11:30:41 GMT  
		Size: 3.1 MB (3145992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b241b0b827643d49ad7c465dbcca697eb5f874b459263f2570a79832c8be1a4`  
		Last Modified: Thu, 19 Dec 2019 11:30:41 GMT  
		Size: 910.0 KB (910029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a85315ec145819eff954cb12f5fd45fb38c3cbdadf778e2748020a1b3517132`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 4.6 KB (4608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8902b38e1df43741e86c3ae67fd17280a6f94c607054b935ca6176a88924ddef`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 26.8 KB (26768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c036842f7853ca602b0c3c2f6eb8f7a18b6f6205badaec7582bf523c759ae6a`  
		Last Modified: Thu, 19 Dec 2019 11:30:47 GMT  
		Size: 88.3 MB (88275811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df541108e281f234aac619f39d5cbe688d1d4ec78558059f713c6316ca4840d9`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eb5b5a1b8dcb91d8fc43276a5c3bbe7e0fce2c9b1fe9c87fea974ce55000d0`  
		Last Modified: Thu, 19 Dec 2019 11:30:39 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:slim`

```console
$ docker pull convertigo@sha256:84a3bcbc4d5b1165d20c915943f7a145180a4aed828603c9a2d3ab67907d69b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:slim` - linux; amd64

```console
$ docker pull convertigo@sha256:c41129e357ae8247d4bef163b6357172c9a21e01a4074aa4f03cd48a55f0b4c3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.4 MB (240418803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:559599fc3be6e43407fd1f91f3190f32dae663b6f66e0bfefb7170068a1c8885`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 19:14:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 19:14:45 GMT
ENV LANG=C.UTF-8
# Fri, 22 Nov 2019 19:17:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 22 Nov 2019 19:17:21 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 19:17:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_VERSION=8u232
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_
# Fri, 22 Nov 2019 19:17:22 GMT
ENV JAVA_URL_VERSION=8u232b09
# Fri, 22 Nov 2019 19:17:38 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 22 Nov 2019 22:44:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 22 Nov 2019 22:44:17 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Nov 2019 22:44:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 22 Nov 2019 22:44:18 GMT
WORKDIR /usr/local/tomcat
# Fri, 22 Nov 2019 22:44:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 22 Nov 2019 22:44:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 22 Nov 2019 22:46:20 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 22 Nov 2019 22:47:28 GMT
ENV TOMCAT_MAJOR=7
# Wed, 18 Dec 2019 01:09:38 GMT
ENV TOMCAT_VERSION=7.0.99
# Wed, 18 Dec 2019 01:09:38 GMT
ENV TOMCAT_SHA512=f53fb4fe6e568afe03fcf23043a3125b0c0ad99872146ff150a30333be92e6322b2278bfcfb2cce67112f09c3aa464086442bb8a79280548b179127ed1abbca9
# Wed, 18 Dec 2019 01:55:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Wed, 18 Dec 2019 01:55:50 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 Dec 2019 01:55:50 GMT
EXPOSE 8080
# Wed, 18 Dec 2019 01:55:50 GMT
CMD ["catalina.sh" "run"]
# Wed, 18 Dec 2019 02:17:23 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Wed, 18 Dec 2019 02:17:23 GMT
ENV SWT_GTK3=0
# Wed, 18 Dec 2019 02:17:23 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 18 Dec 2019 02:17:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 18 Dec 2019 02:17:24 GMT
WORKDIR /usr/local/tomcat
# Wed, 18 Dec 2019 02:17:31 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Wed, 18 Dec 2019 02:17:31 GMT
ENV GOSU_VERSION=1.11
# Wed, 18 Dec 2019 02:17:32 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Wed, 18 Dec 2019 02:17:32 GMT
ENV TINI_VERSION=0.18.0
# Wed, 18 Dec 2019 02:17:32 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Wed, 18 Dec 2019 02:17:34 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Wed, 18 Dec 2019 02:17:35 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Wed, 18 Dec 2019 02:17:35 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_VERSION=7.6.6
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.6.6/convertigo-7.6.6.war
# Wed, 18 Dec 2019 02:17:36 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Wed, 18 Dec 2019 02:17:41 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Wed, 18 Dec 2019 02:17:41 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Wed, 18 Dec 2019 02:17:41 GMT
COPY file:e6b379f8474d7997ac4e3cf958fb910b0d2e1bf1d5b2b89d211cbb8438f94b1e in / 
# Wed, 18 Dec 2019 02:17:41 GMT
WORKDIR /workspace
# Wed, 18 Dec 2019 02:17:42 GMT
VOLUME [/workspace]
# Wed, 18 Dec 2019 02:17:42 GMT
EXPOSE 28080
# Wed, 18 Dec 2019 02:17:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 18 Dec 2019 02:17:42 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dc2bdcfe193ce54affa45170354ca76667c40f8cf536b6282dd379e17e24a`  
		Last Modified: Fri, 22 Nov 2019 19:19:08 GMT  
		Size: 3.2 MB (3249119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a806caa98c159f2c9254dabd60e04352b5c8b46d2e6cc9bd8f7bfc037a4e0b`  
		Last Modified: Fri, 22 Nov 2019 19:21:25 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5943b75c9747aebea25c3fc4bf3d4b4247101176b78ada93d08446dd33f94a0`  
		Last Modified: Fri, 22 Nov 2019 19:21:41 GMT  
		Size: 104.4 MB (104425948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d036bf1b384d6cddf3f1f57b9074d17d6c5d5d142471c63951c3fb7605dbc9`  
		Last Modified: Fri, 22 Nov 2019 22:49:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24c49bbca7a82b1b61cc4c2f27c5a2201b01456a3a98a918e7310ee84041967`  
		Last Modified: Wed, 18 Dec 2019 02:00:50 GMT  
		Size: 10.6 MB (10627739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5364727b9eb8c619c3f089508caccaacc88c1945b426b58779d01ecf9d23d3`  
		Last Modified: Wed, 18 Dec 2019 02:00:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e978d1d04ff84885234fce69dd5c96f1c4a96819fd428d481c8939df7593c25e`  
		Last Modified: Wed, 18 Dec 2019 02:18:39 GMT  
		Size: 5.8 MB (5804209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c150b799e57ad5eca58fbdc22b23f61db56bcab317a49cb4b4fb3728f1eb029`  
		Last Modified: Wed, 18 Dec 2019 02:18:37 GMT  
		Size: 910.1 KB (910076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fa8067fad712950b3a28f8fe1db3dee6b616902aeefa138cd22316473a2a15`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 4.3 KB (4277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1446835a60b437b63b05098b4613a58eac7f0b3b9980221ab353f1a2e918665f`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 26.8 KB (26766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d829d2bec0530fcb07f6d4b8385952dd35eded456f0e06a41fd247f9c0555b4`  
		Last Modified: Wed, 18 Dec 2019 02:18:43 GMT  
		Size: 88.3 MB (88275827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cbe117219f35147a5f976a14a2de8103d2bc584d82d1a0aefb3a0624a05774`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5675557825083e74a819893eb15a740570501e8ce83ccd781019802a948f4a`  
		Last Modified: Wed, 18 Dec 2019 02:18:35 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
