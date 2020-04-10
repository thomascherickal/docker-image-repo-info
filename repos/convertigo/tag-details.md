<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `convertigo`

-	[`convertigo:7.7`](#convertigo77)
-	[`convertigo:7.7.0`](#convertigo770)
-	[`convertigo:latest`](#convertigolatest)

## `convertigo:7.7`

```console
$ docker pull convertigo@sha256:36f62865a0a17a6342583eb45b61baf62274e00c0da9714d50021ba4612d68c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.7` - linux; amd64

```console
$ docker pull convertigo@sha256:10b3cce999a5d774db1ee3ee60cc62398141dcce4961715d47adb00925b841c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429121710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4abfb20549393bf7c2aadf2439aafd81e7166b2b89d0192978788a4305882001`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 31 Mar 2020 01:20:44 GMT
ADD file:c027885123a178148eb4f51f10f4924740859f1f6e941e55580517f6d234e935 in / 
# Tue, 31 Mar 2020 01:20:45 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:56:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 01:57:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 21:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 21:33:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 21:33:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 21:33:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 21:33:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 31 Mar 2020 21:33:41 GMT
ENV JAVA_VERSION=11.0.6
# Tue, 31 Mar 2020 21:33:42 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Tue, 31 Mar 2020 21:33:42 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Tue, 31 Mar 2020 21:33:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Tue, 31 Mar 2020 21:33:54 GMT
CMD ["jshell"]
# Wed, 01 Apr 2020 08:44:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 01 Apr 2020 08:44:40 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 08:44:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 01 Apr 2020 08:44:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 01 Apr 2020 08:44:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:44:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:44:42 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 01 Apr 2020 08:44:42 GMT
ENV TOMCAT_MAJOR=9
# Thu, 09 Apr 2020 23:25:05 GMT
ENV TOMCAT_VERSION=9.0.34
# Thu, 09 Apr 2020 23:25:05 GMT
ENV TOMCAT_SHA512=9cb32f8807c0e8d2457d52ac032bb496ae7921e1ea0a0c8e6082bf8da60bb57c317a3f2376589962123dd803fdd2816ff960339cb851d9859b2241165fbc278e
# Thu, 09 Apr 2020 23:25:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 09 Apr 2020 23:25:32 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 09 Apr 2020 23:25:32 GMT
EXPOSE 8080
# Thu, 09 Apr 2020 23:25:33 GMT
CMD ["catalina.sh" "run"]
# Fri, 10 Apr 2020 00:08:16 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Fri, 10 Apr 2020 00:08:16 GMT
ENV SWT_GTK3=0
# Fri, 10 Apr 2020 00:08:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 10 Apr 2020 00:08:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 10 Apr 2020 00:08:17 GMT
WORKDIR /usr/local/tomcat
# Fri, 10 Apr 2020 00:08:21 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Fri, 10 Apr 2020 00:08:21 GMT
ENV GOSU_VERSION=1.11
# Fri, 10 Apr 2020 00:08:21 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Fri, 10 Apr 2020 00:08:21 GMT
ENV TINI_VERSION=0.18.0
# Fri, 10 Apr 2020 00:08:22 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Fri, 10 Apr 2020 00:08:29 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Fri, 10 Apr 2020 00:08:29 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Fri, 10 Apr 2020 00:08:30 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Fri, 10 Apr 2020 00:08:30 GMT
ENV CONVERTIGO_VERSION=7.7.0
# Fri, 10 Apr 2020 00:08:31 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.7.0/convertigo-7.7.0.war
# Fri, 10 Apr 2020 00:08:31 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Fri, 10 Apr 2020 00:08:36 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Fri, 10 Apr 2020 00:08:36 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Fri, 10 Apr 2020 00:08:36 GMT
COPY file:50df0fa3f88bad82c9cf37b6054755b485e39ccdd9250b2906dc40869fcdd4e8 in / 
# Fri, 10 Apr 2020 00:08:36 GMT
WORKDIR /workspace
# Fri, 10 Apr 2020 00:08:37 GMT
VOLUME [/workspace]
# Fri, 10 Apr 2020 00:08:37 GMT
EXPOSE 28080
# Fri, 10 Apr 2020 00:08:37 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 10 Apr 2020 00:08:37 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:f15005b0235fa8bd31cc6988c4f2758016fe412d696e81aecf73e52be079f19e`  
		Last Modified: Tue, 31 Mar 2020 01:26:22 GMT  
		Size: 50.4 MB (50382041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ebfd3d2fd0de99b1c63aa36a507bf5555481d06e571d84ed84440d30671494`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 7.8 MB (7812166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b998346ba308e3362a85c7bf7faed28d0277c68203696134192fe812f809abb2`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 10.0 MB (9996302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01ec562c947a8ca1b168415da6a4a8f8920808f9b5d6f420ef8fa9af249b1f1`  
		Last Modified: Tue, 31 Mar 2020 02:10:13 GMT  
		Size: 51.8 MB (51790297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c11ae3efe806bf739f69b5ff7592d353b64c422d5b029aa3131551019f1608`  
		Last Modified: Tue, 31 Mar 2020 21:36:39 GMT  
		Size: 5.3 MB (5284627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65829cc6c71f2c75c0efe03c3c77a1bac1c9746af44ef5b03d3bf53985ef62a`  
		Last Modified: Tue, 31 Mar 2020 21:36:38 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98eacc09bf1eb5c963722c31c0bad10622f0cd8483f8826e833d403b2dea549`  
		Last Modified: Tue, 31 Mar 2020 21:37:02 GMT  
		Size: 196.1 MB (196068020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12b9c976670e39e48ec69a1af4e2fcd9e26f13a30e24dc2ba9f2790f83e00f3`  
		Last Modified: Wed, 01 Apr 2020 08:54:40 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a47f54db4cd943353f814e817ff28229b3fff6138feda9a34adf440ed5a1e7`  
		Last Modified: Thu, 09 Apr 2020 23:47:42 GMT  
		Size: 12.2 MB (12158323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c872760f50c9da13bf15661b05a4826d31896aa5efe142f8774d3eb8c4bf157`  
		Last Modified: Thu, 09 Apr 2020 23:47:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f4403ee975b759e8bc2b8d755e2b25e23312ff4ef0c00ba5b00829048149f1`  
		Last Modified: Fri, 10 Apr 2020 00:08:48 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dca8ca9941da56dc51b5216581eb138979dcf4904b982cf8b7ae595b2e8e28b`  
		Last Modified: Fri, 10 Apr 2020 00:08:48 GMT  
		Size: 910.1 KB (910085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69346a9b133fedb3507b51ed610967cfa2f68722b471c1d5c5fffac129d200c`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 4.3 KB (4293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e254636d2d86163b090ee42964b5827a932c796e6e828f1829a6507fe3b296`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 27.3 KB (27282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273ebfb9566fa414c58f494eb9752a5b7201d08837bd0c3ce62197c4b24eade6`  
		Last Modified: Fri, 10 Apr 2020 00:08:54 GMT  
		Size: 94.7 MB (94685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e44f30fc8eb02ddef37e531a2b976a5786412b34fc3a8994986957ee6f6fc1`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac1d8a06f9824a1d736379c0d7ee0e5595bfc985b0e75c54bbd1ae3e32569af`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:7.7.0`

```console
$ docker pull convertigo@sha256:36f62865a0a17a6342583eb45b61baf62274e00c0da9714d50021ba4612d68c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:7.7.0` - linux; amd64

```console
$ docker pull convertigo@sha256:10b3cce999a5d774db1ee3ee60cc62398141dcce4961715d47adb00925b841c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429121710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4abfb20549393bf7c2aadf2439aafd81e7166b2b89d0192978788a4305882001`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 31 Mar 2020 01:20:44 GMT
ADD file:c027885123a178148eb4f51f10f4924740859f1f6e941e55580517f6d234e935 in / 
# Tue, 31 Mar 2020 01:20:45 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:56:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 01:57:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 21:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 21:33:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 21:33:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 21:33:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 21:33:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 31 Mar 2020 21:33:41 GMT
ENV JAVA_VERSION=11.0.6
# Tue, 31 Mar 2020 21:33:42 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Tue, 31 Mar 2020 21:33:42 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Tue, 31 Mar 2020 21:33:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Tue, 31 Mar 2020 21:33:54 GMT
CMD ["jshell"]
# Wed, 01 Apr 2020 08:44:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 01 Apr 2020 08:44:40 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 08:44:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 01 Apr 2020 08:44:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 01 Apr 2020 08:44:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:44:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:44:42 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 01 Apr 2020 08:44:42 GMT
ENV TOMCAT_MAJOR=9
# Thu, 09 Apr 2020 23:25:05 GMT
ENV TOMCAT_VERSION=9.0.34
# Thu, 09 Apr 2020 23:25:05 GMT
ENV TOMCAT_SHA512=9cb32f8807c0e8d2457d52ac032bb496ae7921e1ea0a0c8e6082bf8da60bb57c317a3f2376589962123dd803fdd2816ff960339cb851d9859b2241165fbc278e
# Thu, 09 Apr 2020 23:25:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 09 Apr 2020 23:25:32 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 09 Apr 2020 23:25:32 GMT
EXPOSE 8080
# Thu, 09 Apr 2020 23:25:33 GMT
CMD ["catalina.sh" "run"]
# Fri, 10 Apr 2020 00:08:16 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Fri, 10 Apr 2020 00:08:16 GMT
ENV SWT_GTK3=0
# Fri, 10 Apr 2020 00:08:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 10 Apr 2020 00:08:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 10 Apr 2020 00:08:17 GMT
WORKDIR /usr/local/tomcat
# Fri, 10 Apr 2020 00:08:21 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Fri, 10 Apr 2020 00:08:21 GMT
ENV GOSU_VERSION=1.11
# Fri, 10 Apr 2020 00:08:21 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Fri, 10 Apr 2020 00:08:21 GMT
ENV TINI_VERSION=0.18.0
# Fri, 10 Apr 2020 00:08:22 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Fri, 10 Apr 2020 00:08:29 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Fri, 10 Apr 2020 00:08:29 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Fri, 10 Apr 2020 00:08:30 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Fri, 10 Apr 2020 00:08:30 GMT
ENV CONVERTIGO_VERSION=7.7.0
# Fri, 10 Apr 2020 00:08:31 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.7.0/convertigo-7.7.0.war
# Fri, 10 Apr 2020 00:08:31 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Fri, 10 Apr 2020 00:08:36 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Fri, 10 Apr 2020 00:08:36 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Fri, 10 Apr 2020 00:08:36 GMT
COPY file:50df0fa3f88bad82c9cf37b6054755b485e39ccdd9250b2906dc40869fcdd4e8 in / 
# Fri, 10 Apr 2020 00:08:36 GMT
WORKDIR /workspace
# Fri, 10 Apr 2020 00:08:37 GMT
VOLUME [/workspace]
# Fri, 10 Apr 2020 00:08:37 GMT
EXPOSE 28080
# Fri, 10 Apr 2020 00:08:37 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 10 Apr 2020 00:08:37 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:f15005b0235fa8bd31cc6988c4f2758016fe412d696e81aecf73e52be079f19e`  
		Last Modified: Tue, 31 Mar 2020 01:26:22 GMT  
		Size: 50.4 MB (50382041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ebfd3d2fd0de99b1c63aa36a507bf5555481d06e571d84ed84440d30671494`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 7.8 MB (7812166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b998346ba308e3362a85c7bf7faed28d0277c68203696134192fe812f809abb2`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 10.0 MB (9996302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01ec562c947a8ca1b168415da6a4a8f8920808f9b5d6f420ef8fa9af249b1f1`  
		Last Modified: Tue, 31 Mar 2020 02:10:13 GMT  
		Size: 51.8 MB (51790297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c11ae3efe806bf739f69b5ff7592d353b64c422d5b029aa3131551019f1608`  
		Last Modified: Tue, 31 Mar 2020 21:36:39 GMT  
		Size: 5.3 MB (5284627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65829cc6c71f2c75c0efe03c3c77a1bac1c9746af44ef5b03d3bf53985ef62a`  
		Last Modified: Tue, 31 Mar 2020 21:36:38 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98eacc09bf1eb5c963722c31c0bad10622f0cd8483f8826e833d403b2dea549`  
		Last Modified: Tue, 31 Mar 2020 21:37:02 GMT  
		Size: 196.1 MB (196068020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12b9c976670e39e48ec69a1af4e2fcd9e26f13a30e24dc2ba9f2790f83e00f3`  
		Last Modified: Wed, 01 Apr 2020 08:54:40 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a47f54db4cd943353f814e817ff28229b3fff6138feda9a34adf440ed5a1e7`  
		Last Modified: Thu, 09 Apr 2020 23:47:42 GMT  
		Size: 12.2 MB (12158323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c872760f50c9da13bf15661b05a4826d31896aa5efe142f8774d3eb8c4bf157`  
		Last Modified: Thu, 09 Apr 2020 23:47:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f4403ee975b759e8bc2b8d755e2b25e23312ff4ef0c00ba5b00829048149f1`  
		Last Modified: Fri, 10 Apr 2020 00:08:48 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dca8ca9941da56dc51b5216581eb138979dcf4904b982cf8b7ae595b2e8e28b`  
		Last Modified: Fri, 10 Apr 2020 00:08:48 GMT  
		Size: 910.1 KB (910085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69346a9b133fedb3507b51ed610967cfa2f68722b471c1d5c5fffac129d200c`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 4.3 KB (4293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e254636d2d86163b090ee42964b5827a932c796e6e828f1829a6507fe3b296`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 27.3 KB (27282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273ebfb9566fa414c58f494eb9752a5b7201d08837bd0c3ce62197c4b24eade6`  
		Last Modified: Fri, 10 Apr 2020 00:08:54 GMT  
		Size: 94.7 MB (94685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e44f30fc8eb02ddef37e531a2b976a5786412b34fc3a8994986957ee6f6fc1`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac1d8a06f9824a1d736379c0d7ee0e5595bfc985b0e75c54bbd1ae3e32569af`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:latest`

```console
$ docker pull convertigo@sha256:36f62865a0a17a6342583eb45b61baf62274e00c0da9714d50021ba4612d68c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `convertigo:latest` - linux; amd64

```console
$ docker pull convertigo@sha256:10b3cce999a5d774db1ee3ee60cc62398141dcce4961715d47adb00925b841c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.1 MB (429121710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4abfb20549393bf7c2aadf2439aafd81e7166b2b89d0192978788a4305882001`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 31 Mar 2020 01:20:44 GMT
ADD file:c027885123a178148eb4f51f10f4924740859f1f6e941e55580517f6d234e935 in / 
# Tue, 31 Mar 2020 01:20:45 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:56:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 01:57:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 21:33:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 21:33:40 GMT
ENV LANG=C.UTF-8
# Tue, 31 Mar 2020 21:33:40 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 31 Mar 2020 21:33:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 21:33:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 31 Mar 2020 21:33:41 GMT
ENV JAVA_VERSION=11.0.6
# Tue, 31 Mar 2020 21:33:42 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_
# Tue, 31 Mar 2020 21:33:42 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Tue, 31 Mar 2020 21:33:54 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac --version; 	java --version
# Tue, 31 Mar 2020 21:33:54 GMT
CMD ["jshell"]
# Wed, 01 Apr 2020 08:44:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 01 Apr 2020 08:44:40 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 08:44:41 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 01 Apr 2020 08:44:41 GMT
WORKDIR /usr/local/tomcat
# Wed, 01 Apr 2020 08:44:41 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:44:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 01 Apr 2020 08:44:42 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 01 Apr 2020 08:44:42 GMT
ENV TOMCAT_MAJOR=9
# Thu, 09 Apr 2020 23:25:05 GMT
ENV TOMCAT_VERSION=9.0.34
# Thu, 09 Apr 2020 23:25:05 GMT
ENV TOMCAT_SHA512=9cb32f8807c0e8d2457d52ac032bb496ae7921e1ea0a0c8e6082bf8da60bb57c317a3f2376589962123dd803fdd2816ff960339cb851d9859b2241165fbc278e
# Thu, 09 Apr 2020 23:25:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 09 Apr 2020 23:25:32 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 09 Apr 2020 23:25:32 GMT
EXPOSE 8080
# Thu, 09 Apr 2020 23:25:33 GMT
CMD ["catalina.sh" "run"]
# Fri, 10 Apr 2020 00:08:16 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Fri, 10 Apr 2020 00:08:16 GMT
ENV SWT_GTK3=0
# Fri, 10 Apr 2020 00:08:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 10 Apr 2020 00:08:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 10 Apr 2020 00:08:17 GMT
WORKDIR /usr/local/tomcat
# Fri, 10 Apr 2020 00:08:21 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     unzip   && rm -rf /var/lib/apt/lists/*
# Fri, 10 Apr 2020 00:08:21 GMT
ENV GOSU_VERSION=1.11
# Fri, 10 Apr 2020 00:08:21 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Fri, 10 Apr 2020 00:08:21 GMT
ENV TINI_VERSION=0.18.0
# Fri, 10 Apr 2020 00:08:22 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Fri, 10 Apr 2020 00:08:29 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture)"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture).asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Fri, 10 Apr 2020 00:08:29 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace
# Fri, 10 Apr 2020 00:08:30 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Fri, 10 Apr 2020 00:08:30 GMT
ENV CONVERTIGO_VERSION=7.7.0
# Fri, 10 Apr 2020 00:08:31 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/7.7.0/convertigo-7.7.0.war
# Fri, 10 Apr 2020 00:08:31 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Fri, 10 Apr 2020 00:08:36 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Fri, 10 Apr 2020 00:08:36 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Fri, 10 Apr 2020 00:08:36 GMT
COPY file:50df0fa3f88bad82c9cf37b6054755b485e39ccdd9250b2906dc40869fcdd4e8 in / 
# Fri, 10 Apr 2020 00:08:36 GMT
WORKDIR /workspace
# Fri, 10 Apr 2020 00:08:37 GMT
VOLUME [/workspace]
# Fri, 10 Apr 2020 00:08:37 GMT
EXPOSE 28080
# Fri, 10 Apr 2020 00:08:37 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 10 Apr 2020 00:08:37 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:f15005b0235fa8bd31cc6988c4f2758016fe412d696e81aecf73e52be079f19e`  
		Last Modified: Tue, 31 Mar 2020 01:26:22 GMT  
		Size: 50.4 MB (50382041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ebfd3d2fd0de99b1c63aa36a507bf5555481d06e571d84ed84440d30671494`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 7.8 MB (7812166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b998346ba308e3362a85c7bf7faed28d0277c68203696134192fe812f809abb2`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 10.0 MB (9996302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01ec562c947a8ca1b168415da6a4a8f8920808f9b5d6f420ef8fa9af249b1f1`  
		Last Modified: Tue, 31 Mar 2020 02:10:13 GMT  
		Size: 51.8 MB (51790297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c11ae3efe806bf739f69b5ff7592d353b64c422d5b029aa3131551019f1608`  
		Last Modified: Tue, 31 Mar 2020 21:36:39 GMT  
		Size: 5.3 MB (5284627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65829cc6c71f2c75c0efe03c3c77a1bac1c9746af44ef5b03d3bf53985ef62a`  
		Last Modified: Tue, 31 Mar 2020 21:36:38 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98eacc09bf1eb5c963722c31c0bad10622f0cd8483f8826e833d403b2dea549`  
		Last Modified: Tue, 31 Mar 2020 21:37:02 GMT  
		Size: 196.1 MB (196068020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12b9c976670e39e48ec69a1af4e2fcd9e26f13a30e24dc2ba9f2790f83e00f3`  
		Last Modified: Wed, 01 Apr 2020 08:54:40 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a47f54db4cd943353f814e817ff28229b3fff6138feda9a34adf440ed5a1e7`  
		Last Modified: Thu, 09 Apr 2020 23:47:42 GMT  
		Size: 12.2 MB (12158323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c872760f50c9da13bf15661b05a4826d31896aa5efe142f8774d3eb8c4bf157`  
		Last Modified: Thu, 09 Apr 2020 23:47:41 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f4403ee975b759e8bc2b8d755e2b25e23312ff4ef0c00ba5b00829048149f1`  
		Last Modified: Fri, 10 Apr 2020 00:08:48 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dca8ca9941da56dc51b5216581eb138979dcf4904b982cf8b7ae595b2e8e28b`  
		Last Modified: Fri, 10 Apr 2020 00:08:48 GMT  
		Size: 910.1 KB (910085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69346a9b133fedb3507b51ed610967cfa2f68722b471c1d5c5fffac129d200c`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 4.3 KB (4293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e254636d2d86163b090ee42964b5827a932c796e6e828f1829a6507fe3b296`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 27.3 KB (27282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273ebfb9566fa414c58f494eb9752a5b7201d08837bd0c3ce62197c4b24eade6`  
		Last Modified: Fri, 10 Apr 2020 00:08:54 GMT  
		Size: 94.7 MB (94685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e44f30fc8eb02ddef37e531a2b976a5786412b34fc3a8994986957ee6f6fc1`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac1d8a06f9824a1d736379c0d7ee0e5595bfc985b0e75c54bbd1ae3e32569af`  
		Last Modified: Fri, 10 Apr 2020 00:08:47 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
