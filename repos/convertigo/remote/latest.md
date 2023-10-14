## `convertigo:latest`

```console
$ docker pull convertigo@sha256:748fd1de7d02370d9ab97c830c0cb6778aa63f2bb43ad475abffcab1419bc7b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `convertigo:latest` - linux; amd64

```console
$ docker pull convertigo@sha256:b101768cf6e0f0b691f73445e96d3e1e39bf3e96bdac7d6149373b9cbc852108
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.5 MB (306484868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6598579f00f8f8b0d6fe2d3b9dc5904c431d8f971ec65df765e2578b6591ed14`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:50:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:50:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:50:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 05:53:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:53:21 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Fri, 13 Oct 2023 05:53:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 05:53:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 05:53:32 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 05:53:32 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 05:53:32 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 10:30:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 13 Oct 2023 10:30:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:30:02 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 13 Oct 2023 10:30:02 GMT
WORKDIR /usr/local/tomcat
# Fri, 13 Oct 2023 10:30:02 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 10:30:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 10:30:03 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 13 Oct 2023 10:30:03 GMT
ENV TOMCAT_MAJOR=9
# Sat, 14 Oct 2023 02:44:44 GMT
ENV TOMCAT_VERSION=9.0.82
# Sat, 14 Oct 2023 02:44:44 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Sat, 14 Oct 2023 02:45:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 14 Oct 2023 02:45:35 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 14 Oct 2023 02:45:36 GMT
EXPOSE 8080
# Sat, 14 Oct 2023 02:45:36 GMT
ENTRYPOINT []
# Sat, 14 Oct 2023 02:45:36 GMT
CMD ["catalina.sh" "run"]
# Sat, 14 Oct 2023 03:44:31 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Sat, 14 Oct 2023 03:44:31 GMT
ENV SWT_GTK3=0
# Sat, 14 Oct 2023 03:44:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 14 Oct 2023 03:44:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 14 Oct 2023 03:44:32 GMT
WORKDIR /usr/local/tomcat
# Sat, 14 Oct 2023 03:44:43 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     gosu     sudo     tini     unzip   && apt-get remove -y --purge wget libfreetype6   && apt-get autoremove -y   && rm -rf /var/lib/apt/lists/*
# Sat, 14 Oct 2023 03:44:44 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace     && chown -R convertigo:convertigo /workspace     && chmod -R 777 /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Sat, 14 Oct 2023 03:44:45 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n        <Valve className="org.apache.catalina.valves.ErrorReportValve"  errorCode.404="webapps/convertigo/404.html" errorCode.0="webapps/convertigo/error.html" showReport="false" showServerInfo="false" />\n      </Host>,'         -e 's,</Service>,<!--SSL<Connector port="28443" protocol="org.apache.coyote.http11.Http11AprProtocol" SSLEnabled="true" maxThreads="64000" relaxedQueryChars="{}[]|">\n      <UpgradeProtocol className="org.apache.coyote.http2.Http2Protocol" />\n      <SSLHostConfig>\n        <Certificate certificateKeyFile="/certs/key.pem"\n                     certificateFile="/certs/cert.pem"\n                     certificateChainFile="/certs/chain.pem"\n                     type="RSA" />\n      </SSLHostConfig>\n    </Connector>SSL-->\n  </Service>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*     && chmod 777 conf/context.xml conf/server.xml
# Sat, 14 Oct 2023 03:44:45 GMT
ENV CONVERTIGO_VERSION=8.2.3
# Sat, 14 Oct 2023 03:44:45 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/8.2.3/convertigo-8.2.3.war
# Sat, 14 Oct 2023 03:44:45 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Sat, 14 Oct 2023 03:44:51 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && mkdir /certs && chmod 777 /certs     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && chmod 777 WEB-INF/web.xml WEB-INF/lib WEB-INF/classes         && rm -rf /tmp/*)
# Sat, 14 Oct 2023 03:44:52 GMT
COPY file:a8c73db31af1c6589d48a2342d8673de69087696e5f19812fc67f887368ccae8 in webapps/ROOT/index.html 
# Sat, 14 Oct 2023 03:44:52 GMT
COPY file:f9f666c95ba08499a7e3e81d2fbe010226895813dbaabe692cf6db96a33c02ad in / 
# Sat, 14 Oct 2023 03:44:52 GMT
WORKDIR /workspace
# Sat, 14 Oct 2023 03:44:52 GMT
VOLUME [/workspace]
# Sat, 14 Oct 2023 03:44:52 GMT
EXPOSE 28080
# Sat, 14 Oct 2023 03:44:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 14 Oct 2023 03:44:52 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03dd46c3c6b33dd978f9acbcc939fe709970154e88a034c575cd59c77e47dc70`  
		Last Modified: Fri, 13 Oct 2023 05:58:58 GMT  
		Size: 20.7 MB (20661122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7246c026383675823396ae4684eb7db7a2b93a92d7da0df34286eb74a3fe74c`  
		Last Modified: Fri, 13 Oct 2023 05:59:08 GMT  
		Size: 144.8 MB (144778046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2279deef4bab9acbf4f98cb77598280c64fd29d1814c7b8e49908c66067dc43`  
		Last Modified: Fri, 13 Oct 2023 05:58:55 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3725b10eb36cb593f7c65aa7ab34b61e5f82e6580a82df0b14fc89cdcd1838`  
		Last Modified: Fri, 13 Oct 2023 05:58:55 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cc218029704feefb2c17f642fabeec2cf8525fe566f99a29a5d9dcf21e2c57`  
		Last Modified: Fri, 13 Oct 2023 10:49:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddef67117cf609cc71c76df16fa668943c7fb8fa0daa6aa7fa0875064444621`  
		Last Modified: Sat, 14 Oct 2023 02:58:02 GMT  
		Size: 12.8 MB (12846215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dfbcb5cd5b62d4114f8b40efa85273263a235ae363cf50b71c7e21110b01d6`  
		Last Modified: Sat, 14 Oct 2023 02:58:01 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb86320f83d138d3c583a9a2f417750208af2ae093cb1dce071dc3d76a4d0589`  
		Last Modified: Sat, 14 Oct 2023 03:45:04 GMT  
		Size: 5.4 MB (5431371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dc37726a9e77796e60eade579fdccecc97351b50c736aab49df9263f211b3a`  
		Last Modified: Sat, 14 Oct 2023 03:45:00 GMT  
		Size: 4.5 KB (4549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a9c5dcc77e467631cf8b120933d994fc3833ae0c8eb8f6c21e50e3f03b2cff`  
		Last Modified: Sat, 14 Oct 2023 03:45:00 GMT  
		Size: 27.9 KB (27934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088d4f8041570bf2b5b2068c62d8c16ab15b33687918e6ccc3e7486f5c70b56d`  
		Last Modified: Sat, 14 Oct 2023 03:45:06 GMT  
		Size: 94.2 MB (94150976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10b98b0b8360d8ca3aff231cb1fd9d0605fe920a74966fbcd1cbad73a3a9e49`  
		Last Modified: Sat, 14 Oct 2023 03:45:00 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099002db44b81344ffc5e661a8dc04e73757777f9121727b133f56c9c7233937`  
		Last Modified: Sat, 14 Oct 2023 03:45:00 GMT  
		Size: 2.3 KB (2323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `convertigo:latest` - linux; arm variant v7

```console
$ docker pull convertigo@sha256:affebd1fbd0df51cbf593e937fae8ce17cd213a6f4b8bda21337421df1d68579
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.2 MB (298243416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d5288f50bc307c86b1f74eb3836b0455e5fc5763457211018daa3ea169d4397`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:15:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 01:15:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 01:15:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 01:18:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:18:29 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Fri, 13 Oct 2023 01:18:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 01:18:47 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 01:18:47 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 01:18:47 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 01:18:47 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 04:23:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 13 Oct 2023 04:23:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 04:23:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 13 Oct 2023 04:23:28 GMT
WORKDIR /usr/local/tomcat
# Fri, 13 Oct 2023 04:23:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 04:23:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 04:23:28 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 13 Oct 2023 04:23:28 GMT
ENV TOMCAT_MAJOR=9
# Sat, 14 Oct 2023 02:15:03 GMT
ENV TOMCAT_VERSION=9.0.82
# Sat, 14 Oct 2023 02:15:03 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Sat, 14 Oct 2023 02:15:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 14 Oct 2023 02:15:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 14 Oct 2023 02:15:57 GMT
EXPOSE 8080
# Sat, 14 Oct 2023 02:15:57 GMT
ENTRYPOINT []
# Sat, 14 Oct 2023 02:15:57 GMT
CMD ["catalina.sh" "run"]
# Sat, 14 Oct 2023 02:53:04 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Sat, 14 Oct 2023 02:53:05 GMT
ENV SWT_GTK3=0
# Sat, 14 Oct 2023 02:53:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 14 Oct 2023 02:53:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 14 Oct 2023 02:53:05 GMT
WORKDIR /usr/local/tomcat
# Sat, 14 Oct 2023 02:53:16 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     gosu     sudo     tini     unzip   && apt-get remove -y --purge wget libfreetype6   && apt-get autoremove -y   && rm -rf /var/lib/apt/lists/*
# Sat, 14 Oct 2023 02:53:17 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace     && chown -R convertigo:convertigo /workspace     && chmod -R 777 /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Sat, 14 Oct 2023 02:53:17 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n        <Valve className="org.apache.catalina.valves.ErrorReportValve"  errorCode.404="webapps/convertigo/404.html" errorCode.0="webapps/convertigo/error.html" showReport="false" showServerInfo="false" />\n      </Host>,'         -e 's,</Service>,<!--SSL<Connector port="28443" protocol="org.apache.coyote.http11.Http11AprProtocol" SSLEnabled="true" maxThreads="64000" relaxedQueryChars="{}[]|">\n      <UpgradeProtocol className="org.apache.coyote.http2.Http2Protocol" />\n      <SSLHostConfig>\n        <Certificate certificateKeyFile="/certs/key.pem"\n                     certificateFile="/certs/cert.pem"\n                     certificateChainFile="/certs/chain.pem"\n                     type="RSA" />\n      </SSLHostConfig>\n    </Connector>SSL-->\n  </Service>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*     && chmod 777 conf/context.xml conf/server.xml
# Sat, 14 Oct 2023 02:53:17 GMT
ENV CONVERTIGO_VERSION=8.2.3
# Sat, 14 Oct 2023 02:53:17 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/8.2.3/convertigo-8.2.3.war
# Sat, 14 Oct 2023 02:53:17 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Sat, 14 Oct 2023 02:53:25 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && mkdir /certs && chmod 777 /certs     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && chmod 777 WEB-INF/web.xml WEB-INF/lib WEB-INF/classes         && rm -rf /tmp/*)
# Sat, 14 Oct 2023 02:53:25 GMT
COPY file:a8c73db31af1c6589d48a2342d8673de69087696e5f19812fc67f887368ccae8 in webapps/ROOT/index.html 
# Sat, 14 Oct 2023 02:53:25 GMT
COPY file:f9f666c95ba08499a7e3e81d2fbe010226895813dbaabe692cf6db96a33c02ad in / 
# Sat, 14 Oct 2023 02:53:25 GMT
WORKDIR /workspace
# Sat, 14 Oct 2023 02:53:25 GMT
VOLUME [/workspace]
# Sat, 14 Oct 2023 02:53:26 GMT
EXPOSE 28080
# Sat, 14 Oct 2023 02:53:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 14 Oct 2023 02:53:26 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1527106f17a5b629b350869074ec790617e95a6e7701e167ea159107d7c5b2f2`  
		Last Modified: Fri, 13 Oct 2023 01:23:19 GMT  
		Size: 20.0 MB (19961731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d4ba893d75d76994ccd65f3cf50819ebb586e88f54562166206506cc436898`  
		Last Modified: Fri, 13 Oct 2023 01:23:33 GMT  
		Size: 142.1 MB (142063765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30df131d60cdee394f3def01c2b49ee63131bc634084ffeecc04c077d2e2c1a1`  
		Last Modified: Fri, 13 Oct 2023 01:23:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197b7c34747a7107db9a1f242a283d070f5a79a4f8e24ea95d746d882453e114`  
		Last Modified: Fri, 13 Oct 2023 01:23:15 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38291bb37ac14576dece7fcdc4ceed3cb0b143adfce00cd419f035316e60f675`  
		Last Modified: Fri, 13 Oct 2023 04:37:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ec41f1848557156a6396b31ac01fa0986c879f101177b9b1a3a6531553de57`  
		Last Modified: Sat, 14 Oct 2023 02:22:50 GMT  
		Size: 12.8 MB (12768052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7432276fa568c04006ef61a371afc6e6eeae8d8a8080b591afb475478d1687dc`  
		Last Modified: Sat, 14 Oct 2023 02:22:49 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d61b72a852707079c6bffc834a7ee9f39ff097fadb5e2c70239ffb118bb86d8`  
		Last Modified: Sat, 14 Oct 2023 02:53:36 GMT  
		Size: 4.7 MB (4670265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b46557e6148d19f2383ba7a7709b76b1796c6e7db8772d4ad1d8c962975c1b`  
		Last Modified: Sat, 14 Oct 2023 02:53:33 GMT  
		Size: 4.5 KB (4538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2836b09fd751087d8955fcbb7c199cc4a71f7f6057c5a93f1140638edbadbeb9`  
		Last Modified: Sat, 14 Oct 2023 02:53:33 GMT  
		Size: 27.9 KB (27936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72823b91cdc67d98bc6d69d9c51675f121508272c132933d2706fdf83dd84404`  
		Last Modified: Sat, 14 Oct 2023 02:53:40 GMT  
		Size: 94.2 MB (94150976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5150564aa83a8d00bbd8d77b5df609088aac459ddbfb732b4c6bd788b95af2`  
		Last Modified: Sat, 14 Oct 2023 02:53:33 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ca67b97621cd0a6863f594c972759bf803f770240014d9b4d34f3c5ff5889a`  
		Last Modified: Sat, 14 Oct 2023 02:53:33 GMT  
		Size: 2.3 KB (2322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `convertigo:latest` - linux; arm64 variant v8

```console
$ docker pull convertigo@sha256:041f2cc143756c5786f0d8e8922be622249c56b40cde9ae0d6a5ea45a3baff76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.4 MB (304441963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62aaa0818d37e4e77c368752aaf58d8378c564d23f692e5c86cfa2e9e9c616d2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 02:48:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:48:12 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Fri, 13 Oct 2023 02:48:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 02:48:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 02:48:23 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 02:48:23 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 02:48:23 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 11:06:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 13 Oct 2023 11:06:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 11:06:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 13 Oct 2023 11:06:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 13 Oct 2023 11:06:51 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 11:06:51 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 11:06:51 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 13 Oct 2023 11:06:51 GMT
ENV TOMCAT_MAJOR=9
# Sat, 14 Oct 2023 03:09:04 GMT
ENV TOMCAT_VERSION=9.0.82
# Sat, 14 Oct 2023 03:09:04 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Sat, 14 Oct 2023 03:09:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 1777 logs temp work; 		catalina.sh version
# Sat, 14 Oct 2023 03:09:47 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 14 Oct 2023 03:09:48 GMT
EXPOSE 8080
# Sat, 14 Oct 2023 03:09:48 GMT
ENTRYPOINT []
# Sat, 14 Oct 2023 03:09:48 GMT
CMD ["catalina.sh" "run"]
# Sat, 14 Oct 2023 04:02:21 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Sat, 14 Oct 2023 04:02:22 GMT
ENV SWT_GTK3=0
# Sat, 14 Oct 2023 04:02:22 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 14 Oct 2023 04:02:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 14 Oct 2023 04:02:22 GMT
WORKDIR /usr/local/tomcat
# Sat, 14 Oct 2023 04:02:32 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     gosu     sudo     tini     unzip   && apt-get remove -y --purge wget libfreetype6   && apt-get autoremove -y   && rm -rf /var/lib/apt/lists/*
# Sat, 14 Oct 2023 04:02:33 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace     && chown -R convertigo:convertigo /workspace     && chmod -R 777 /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Sat, 14 Oct 2023 04:02:33 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n        <Valve className="org.apache.catalina.valves.ErrorReportValve"  errorCode.404="webapps/convertigo/404.html" errorCode.0="webapps/convertigo/error.html" showReport="false" showServerInfo="false" />\n      </Host>,'         -e 's,</Service>,<!--SSL<Connector port="28443" protocol="org.apache.coyote.http11.Http11AprProtocol" SSLEnabled="true" maxThreads="64000" relaxedQueryChars="{}[]|">\n      <UpgradeProtocol className="org.apache.coyote.http2.Http2Protocol" />\n      <SSLHostConfig>\n        <Certificate certificateKeyFile="/certs/key.pem"\n                     certificateFile="/certs/cert.pem"\n                     certificateChainFile="/certs/chain.pem"\n                     type="RSA" />\n      </SSLHostConfig>\n    </Connector>SSL-->\n  </Service>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*     && chmod 777 conf/context.xml conf/server.xml
# Sat, 14 Oct 2023 04:02:33 GMT
ENV CONVERTIGO_VERSION=8.2.3
# Sat, 14 Oct 2023 04:02:33 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/8.2.3/convertigo-8.2.3.war
# Sat, 14 Oct 2023 04:02:33 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Sat, 14 Oct 2023 04:02:40 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && mkdir /certs && chmod 777 /certs     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && chmod 777 WEB-INF/web.xml WEB-INF/lib WEB-INF/classes         && rm -rf /tmp/*)
# Sat, 14 Oct 2023 04:02:40 GMT
COPY file:a8c73db31af1c6589d48a2342d8673de69087696e5f19812fc67f887368ccae8 in webapps/ROOT/index.html 
# Sat, 14 Oct 2023 04:02:40 GMT
COPY file:f9f666c95ba08499a7e3e81d2fbe010226895813dbaabe692cf6db96a33c02ad in / 
# Sat, 14 Oct 2023 04:02:40 GMT
WORKDIR /workspace
# Sat, 14 Oct 2023 04:02:40 GMT
VOLUME [/workspace]
# Sat, 14 Oct 2023 04:02:40 GMT
EXPOSE 28080
# Sat, 14 Oct 2023 04:02:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 14 Oct 2023 04:02:41 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7791071f3db6ce25c9e5311ee87076d7972356105e381a64f6e64ccd42fd71b`  
		Last Modified: Fri, 13 Oct 2023 02:52:56 GMT  
		Size: 21.4 MB (21378380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee0e92c0a265376d312447f52945a3e1087c5758d93fcae7da7cad8d620ab18`  
		Last Modified: Fri, 13 Oct 2023 02:53:03 GMT  
		Size: 143.6 MB (143554268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b41500ac7c2de84799ba7e742c611628faef0b70fed3e1ca2b1abc7ffc0af33`  
		Last Modified: Fri, 13 Oct 2023 02:52:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b785c8b7db0588308e97d2d5268e2369afaca9eee273e6e7cbfe1543b8c9359b`  
		Last Modified: Fri, 13 Oct 2023 02:52:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0e0539364e506434d159e223c40b5acd76c6682a6f0584d5bce46fe6a658f1`  
		Last Modified: Fri, 13 Oct 2023 11:24:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9843f0233ebbf441a56c75f11e7fa31fe9612b2288e7c0d41760bf70498f0ed`  
		Last Modified: Sat, 14 Oct 2023 03:20:16 GMT  
		Size: 12.9 MB (12862104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b62fc5770e0c4a901a871b6e837a200390cc1504f107ed3fe28840a10c4eda`  
		Last Modified: Sat, 14 Oct 2023 03:20:14 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee43e656951682540da08f088c57d0cbfdc0daf60324a4820bcbde6ad1c7ac7`  
		Last Modified: Sat, 14 Oct 2023 04:02:53 GMT  
		Size: 5.3 MB (5260260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22fe5ecff85509ab2da8a838042e40cf41165477acbb364057220321502e81a`  
		Last Modified: Sat, 14 Oct 2023 04:02:50 GMT  
		Size: 4.6 KB (4560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e429cc9853e48c7cb7a77298ea381909154110885b5291f033efa6dfad84b8`  
		Last Modified: Sat, 14 Oct 2023 04:02:50 GMT  
		Size: 27.9 KB (27939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054ab4f8f6e67fd4cddfca0e6632efa455e0e57fbbdf5dda43cba6a984c3fe97`  
		Last Modified: Sat, 14 Oct 2023 04:02:57 GMT  
		Size: 94.2 MB (94150968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e6a5c5c57ab63762a6174fefe3efe138d3b5bc2dc40b10ac4541bc53939fb6`  
		Last Modified: Sat, 14 Oct 2023 04:02:50 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92280716f73e5ce6491dd154581c4bbbc58e6cfe819b6929e434602f09c8d7c`  
		Last Modified: Sat, 14 Oct 2023 04:02:50 GMT  
		Size: 2.3 KB (2322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
