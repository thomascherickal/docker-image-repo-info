<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `convertigo`

-	[`convertigo:8.0`](#convertigo80)
-	[`convertigo:8.0.2`](#convertigo802)
-	[`convertigo:latest`](#convertigolatest)

## `convertigo:8.0`

```console
$ docker pull convertigo@sha256:e1d71354d7e895282c1babbc480fe001cf709c0b0aabac01b1e24e133df79449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `convertigo:8.0` - linux; amd64

```console
$ docker pull convertigo@sha256:39fee16f757efef6b90b9fc11568b4175422a3ccf487df7ad1927d5f5d5ce28a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353035598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3333a0c49176fb6be4035e410131d26b8fb5e4ecb8c18c192a866c5e7271422d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:02:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:02:28 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 17:02:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:02:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 17:02:41 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 05:19:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 05:19:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:19:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 05:19:28 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 05:19:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:19:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:24:31 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_MAJOR=9
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_VERSION=9.0.67
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_SHA512=f3c4841754640a21842de9d8ec4674b1a072d42f3ba9d1accea143a61ac4f77b06c789fbcc395c23ed2154ec7e7cd76e6d39743e544f7c6f2022967e8a2334d5
# Thu, 06 Oct 2022 05:25:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 06 Oct 2022 05:25:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 06 Oct 2022 05:25:02 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 05:25:02 GMT
CMD ["catalina.sh" "run"]
# Thu, 06 Oct 2022 09:54:51 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 06 Oct 2022 09:54:51 GMT
ENV SWT_GTK3=0
# Thu, 06 Oct 2022 09:54:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 09:54:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 09:54:52 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 09:55:03 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     sudo     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 09:55:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 06 Oct 2022 09:55:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 06 Oct 2022 09:55:04 GMT
ENV TINI_VERSION=0.19.0
# Thu, 06 Oct 2022 09:55:04 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 06 Oct 2022 09:56:11 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 06 Oct 2022 09:56:11 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Thu, 06 Oct 2022 09:56:12 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_VERSION=8.0.2
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/8.0.2/convertigo-8.0.2.war
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 06 Oct 2022 09:56:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 06 Oct 2022 09:56:57 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Thu, 06 Oct 2022 09:56:57 GMT
COPY file:4ad3aea0c0d804794214363082a62ec38380e1ab5e72b5b3fd619030091384c6 in / 
# Thu, 06 Oct 2022 09:56:57 GMT
WORKDIR /workspace
# Thu, 06 Oct 2022 09:56:57 GMT
VOLUME [/workspace]
# Thu, 06 Oct 2022 09:56:57 GMT
EXPOSE 28080
# Thu, 06 Oct 2022 09:56:57 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 09:56:57 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d22208b60b954bd6e09e29c05404ffe32c8235a504053cf31cf6a197edeece`  
		Last Modified: Wed, 05 Oct 2022 17:09:41 GMT  
		Size: 20.1 MB (20104176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d0a4a95f9ec2d1f831538497ba1a653c9468c8bb0e001a2f39ea2481fcb8e0`  
		Last Modified: Wed, 05 Oct 2022 17:09:52 GMT  
		Size: 192.1 MB (192146085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f1490693c6fb5c391bddcaf065d8e85cbc9a41b3fa5b44a08d77f42e1bbd31`  
		Last Modified: Wed, 05 Oct 2022 17:09:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a0e39e56b4605e06f061cfe80897d740adfedbe2bd32bdda3d5b50d531ff1`  
		Last Modified: Thu, 06 Oct 2022 05:40:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ba5f7d4ed631679273613857d5e4ada5782796eb108ee2d66f825774c2cb18`  
		Last Modified: Thu, 06 Oct 2022 05:44:49 GMT  
		Size: 12.7 MB (12718294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89acf6d4bf9a5c5bc0adea23c0dbe47a9f1f1a44ad651b443260a4c23adccd44`  
		Last Modified: Thu, 06 Oct 2022 05:44:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52803a12fa8e3da0e659035745a421916d555b85af202401a41910e1e618dbf`  
		Last Modified: Thu, 06 Oct 2022 09:57:23 GMT  
		Size: 4.4 MB (4397160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98eda955d39d200d66c889b8471de009670ab25ee9fd81cf4188ebd30d78bc3`  
		Last Modified: Thu, 06 Oct 2022 09:57:23 GMT  
		Size: 938.7 KB (938672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77132e1d2bdb94fa798c3b883c60f0a170b44688dd7776974d28b724f94704d`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 4.6 KB (4584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17002aef77c534bb598190fc2ca1f7615dfe957bf3c479a89d04b4df3b76b647`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 27.6 KB (27554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f0fa447e6d4ee16f3b862beca5d1c793f47aacb5eceac4d5ec37026a4499de`  
		Last Modified: Thu, 06 Oct 2022 09:57:26 GMT  
		Size: 94.1 MB (94122200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09a5d596d2b2d8001c5c42eef0ebff142d5c914fc18e40170d848cd93183c8`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b4c8f1df6423f9eb638f3934b7748595569d762be6cd7a690088a46cf78445`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 1.5 KB (1490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:8.0.2`

```console
$ docker pull convertigo@sha256:e1d71354d7e895282c1babbc480fe001cf709c0b0aabac01b1e24e133df79449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `convertigo:8.0.2` - linux; amd64

```console
$ docker pull convertigo@sha256:39fee16f757efef6b90b9fc11568b4175422a3ccf487df7ad1927d5f5d5ce28a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353035598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3333a0c49176fb6be4035e410131d26b8fb5e4ecb8c18c192a866c5e7271422d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:02:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:02:28 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 17:02:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:02:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 17:02:41 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 05:19:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 05:19:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:19:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 05:19:28 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 05:19:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:19:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:24:31 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_MAJOR=9
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_VERSION=9.0.67
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_SHA512=f3c4841754640a21842de9d8ec4674b1a072d42f3ba9d1accea143a61ac4f77b06c789fbcc395c23ed2154ec7e7cd76e6d39743e544f7c6f2022967e8a2334d5
# Thu, 06 Oct 2022 05:25:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 06 Oct 2022 05:25:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 06 Oct 2022 05:25:02 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 05:25:02 GMT
CMD ["catalina.sh" "run"]
# Thu, 06 Oct 2022 09:54:51 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 06 Oct 2022 09:54:51 GMT
ENV SWT_GTK3=0
# Thu, 06 Oct 2022 09:54:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 09:54:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 09:54:52 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 09:55:03 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     sudo     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 09:55:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 06 Oct 2022 09:55:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 06 Oct 2022 09:55:04 GMT
ENV TINI_VERSION=0.19.0
# Thu, 06 Oct 2022 09:55:04 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 06 Oct 2022 09:56:11 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 06 Oct 2022 09:56:11 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Thu, 06 Oct 2022 09:56:12 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_VERSION=8.0.2
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/8.0.2/convertigo-8.0.2.war
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 06 Oct 2022 09:56:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 06 Oct 2022 09:56:57 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Thu, 06 Oct 2022 09:56:57 GMT
COPY file:4ad3aea0c0d804794214363082a62ec38380e1ab5e72b5b3fd619030091384c6 in / 
# Thu, 06 Oct 2022 09:56:57 GMT
WORKDIR /workspace
# Thu, 06 Oct 2022 09:56:57 GMT
VOLUME [/workspace]
# Thu, 06 Oct 2022 09:56:57 GMT
EXPOSE 28080
# Thu, 06 Oct 2022 09:56:57 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 09:56:57 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d22208b60b954bd6e09e29c05404ffe32c8235a504053cf31cf6a197edeece`  
		Last Modified: Wed, 05 Oct 2022 17:09:41 GMT  
		Size: 20.1 MB (20104176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d0a4a95f9ec2d1f831538497ba1a653c9468c8bb0e001a2f39ea2481fcb8e0`  
		Last Modified: Wed, 05 Oct 2022 17:09:52 GMT  
		Size: 192.1 MB (192146085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f1490693c6fb5c391bddcaf065d8e85cbc9a41b3fa5b44a08d77f42e1bbd31`  
		Last Modified: Wed, 05 Oct 2022 17:09:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a0e39e56b4605e06f061cfe80897d740adfedbe2bd32bdda3d5b50d531ff1`  
		Last Modified: Thu, 06 Oct 2022 05:40:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ba5f7d4ed631679273613857d5e4ada5782796eb108ee2d66f825774c2cb18`  
		Last Modified: Thu, 06 Oct 2022 05:44:49 GMT  
		Size: 12.7 MB (12718294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89acf6d4bf9a5c5bc0adea23c0dbe47a9f1f1a44ad651b443260a4c23adccd44`  
		Last Modified: Thu, 06 Oct 2022 05:44:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52803a12fa8e3da0e659035745a421916d555b85af202401a41910e1e618dbf`  
		Last Modified: Thu, 06 Oct 2022 09:57:23 GMT  
		Size: 4.4 MB (4397160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98eda955d39d200d66c889b8471de009670ab25ee9fd81cf4188ebd30d78bc3`  
		Last Modified: Thu, 06 Oct 2022 09:57:23 GMT  
		Size: 938.7 KB (938672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77132e1d2bdb94fa798c3b883c60f0a170b44688dd7776974d28b724f94704d`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 4.6 KB (4584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17002aef77c534bb598190fc2ca1f7615dfe957bf3c479a89d04b4df3b76b647`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 27.6 KB (27554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f0fa447e6d4ee16f3b862beca5d1c793f47aacb5eceac4d5ec37026a4499de`  
		Last Modified: Thu, 06 Oct 2022 09:57:26 GMT  
		Size: 94.1 MB (94122200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09a5d596d2b2d8001c5c42eef0ebff142d5c914fc18e40170d848cd93183c8`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b4c8f1df6423f9eb638f3934b7748595569d762be6cd7a690088a46cf78445`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 1.5 KB (1490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `convertigo:latest`

```console
$ docker pull convertigo@sha256:e1d71354d7e895282c1babbc480fe001cf709c0b0aabac01b1e24e133df79449
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `convertigo:latest` - linux; amd64

```console
$ docker pull convertigo@sha256:39fee16f757efef6b90b9fc11568b4175422a3ccf487df7ad1927d5f5d5ce28a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353035598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3333a0c49176fb6be4035e410131d26b8fb5e4ecb8c18c192a866c5e7271422d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["convertigo"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:02:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:02:28 GMT
ENV JAVA_VERSION=jdk-17.0.4.1+1
# Wed, 05 Oct 2022 17:02:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3c7460de77421284b38b4e57cb1bd584a6cef55c34fc51a12270620544de2b8a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        armhf|arm)          ESUM='efba97cd38af8f43b61f09cb5041f81d92ecd005dcd51c81678fbcf4f24d8461';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cbedd0a1428b3058d156e99e8e9bc8769e0d633736d6776a4c4d9136648f2fd1';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='fdc82f4b06c880762503b0cb40e25f46cf8190d06011b3b768f4091d3334ef7f';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5fbf8b62c44f10be2efab97c5f5dbf15b74fae31e451ec10abbc74e54a04ff44';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.4.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.4.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:02:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 05 Oct 2022 17:02:41 GMT
CMD ["jshell"]
# Thu, 06 Oct 2022 05:19:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 05:19:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:19:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 05:19:28 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 05:19:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:19:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:24:31 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_MAJOR=9
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_VERSION=9.0.67
# Thu, 06 Oct 2022 05:24:31 GMT
ENV TOMCAT_SHA512=f3c4841754640a21842de9d8ec4674b1a072d42f3ba9d1accea143a61ac4f77b06c789fbcc395c23ed2154ec7e7cd76e6d39743e544f7c6f2022967e8a2334d5
# Thu, 06 Oct 2022 05:25:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		dirmngr 		gnupg 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://downloads.apache.org/$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if curl -fL -o "$f" "$distUrl" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl 		; 		nproc="$(nproc)"; 		make -j "$nproc"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| tee "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt" 		| xargs -r apt-mark manual 	; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 06 Oct 2022 05:25:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 06 Oct 2022 05:25:02 GMT
EXPOSE 8080
# Thu, 06 Oct 2022 05:25:02 GMT
CMD ["catalina.sh" "run"]
# Thu, 06 Oct 2022 09:54:51 GMT
MAINTAINER Nicolas Albert nicolasa@convertigo.com
# Thu, 06 Oct 2022 09:54:51 GMT
ENV SWT_GTK3=0
# Thu, 06 Oct 2022 09:54:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 09:54:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 09:54:52 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 09:55:03 GMT
RUN apt-get update -y   && apt-get install -y --no-install-recommends     ca-certificates     curl     dirmngr     gnupg     sudo     unzip   && rm -rf /var/lib/apt/lists/*
# Thu, 06 Oct 2022 09:55:03 GMT
ENV GOSU_VERSION=1.14
# Thu, 06 Oct 2022 09:55:04 GMT
ENV GOSU_GPG_KEYS=B42F6819007F00F88E364FD4036A9C25BF357DD4
# Thu, 06 Oct 2022 09:55:04 GMT
ENV TINI_VERSION=0.19.0
# Thu, 06 Oct 2022 09:55:04 GMT
ENV TINI_GPG_KEYS=6380DC428747F6C393FEACA59A84159D7001A4E5
# Thu, 06 Oct 2022 09:56:11 GMT
RUN export GNUPGHOME="$(mktemp -d)"   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$GOSU_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GOSU_GPG_KEYS" )   && curl -o /usr/local/bin/gosu -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/gosu.asc -fSL "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu   && rm /usr/local/bin/gosu.asc   && chmod +x /usr/local/bin/gosu   && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver pgp.mit.edu --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$TINI_GPG_KEYS"   || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$TINI_GPG_KEYS" )   && curl -o /usr/local/bin/tini -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }')"   && curl -o /usr/local/bin/tini.asc -fSL "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$(dpkg --print-architecture | awk -F- '{ print $NF }').asc"   && gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini   && rm /usr/local/bin/tini.asc   && chmod +x /usr/local/bin/tini   && rm -rf /tmp/*
# Thu, 06 Oct 2022 09:56:11 GMT
RUN useradd -s /bin/false -m convertigo     && mkdir -p /workspace/lib /workspace/classes     && chown -R convertigo:convertigo /workspace     && echo "convertigo ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/convertigo     && chmod 0440 /etc/sudoers.d/convertigo
# Thu, 06 Oct 2022 09:56:12 GMT
RUN sed -i.bak         -e '/protocol="AJP/d'         -e '/AprLifecycleListener/d'         -e '/JasperListener/d'         -e 's/port="8080"/port="28080" maxThreads="64000" relaxedQueryChars="{}[]|"/'         -e 's,</Host>,  <Valve className="org.apache.catalina.valves.RemoteIpValve" />\n      </Host>,'         conf/server.xml     && sed -i.bak         -e 's,<Context>,<Context sessionCookiePath="/">,'         -e 's,</Context>,<Manager pathname="" /><CookieProcessor sameSiteCookies="unset" /></Context>,'         conf/context.xml     && rm -rf webapps/* bin/*.bat conf/server.xml.bak /tmp/*     && mkdir webapps/ROOT     && chown -R convertigo:convertigo conf temp work logs     && chmod -w conf/*
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_VERSION=8.0.2
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_WAR_URL=https://github.com/convertigo/convertigo/releases/download/8.0.2/convertigo-8.0.2.war
# Thu, 06 Oct 2022 09:56:12 GMT
ENV CONVERTIGO_GPG_KEYS=6A7779BB78FE368DF74B708FD4DA8FBEB64BF75F
# Thu, 06 Oct 2022 09:56:56 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && ( gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver pgp.mit.edu --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$CONVERTIGO_GPG_KEYS"     || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$CONVERTIGO_GPG_KEYS" )     && curl -fSL -o /tmp/convertigo.war $CONVERTIGO_WAR_URL     && curl -fSL -o /tmp/convertigo.war.asc $CONVERTIGO_WAR_URL.asc     && gpg --batch --verify /tmp/convertigo.war.asc /tmp/convertigo.war     && mkdir -p webapps/ROOT webapps/convertigo     && (cd webapps/convertigo         && unzip -q /tmp/convertigo.war         && (chmod -f a+x WEB-INF/xvnc/* || true)         && (test "$(dpkg --print-architecture)" != "i386" && rm -rf WEB-INF/xulrunner WEB-INF/xvnc WEB-INF/lib/swt_* || true)         && rm -rf /tmp/*)
# Thu, 06 Oct 2022 09:56:57 GMT
COPY file:394d5b837e94d77b6fb87e0ca8bd50995186aaed1c5f3ab5bc0b482f0f769cc3 in webapps/ROOT/index.html 
# Thu, 06 Oct 2022 09:56:57 GMT
COPY file:4ad3aea0c0d804794214363082a62ec38380e1ab5e72b5b3fd619030091384c6 in / 
# Thu, 06 Oct 2022 09:56:57 GMT
WORKDIR /workspace
# Thu, 06 Oct 2022 09:56:57 GMT
VOLUME [/workspace]
# Thu, 06 Oct 2022 09:56:57 GMT
EXPOSE 28080
# Thu, 06 Oct 2022 09:56:57 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 09:56:57 GMT
CMD ["convertigo"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d22208b60b954bd6e09e29c05404ffe32c8235a504053cf31cf6a197edeece`  
		Last Modified: Wed, 05 Oct 2022 17:09:41 GMT  
		Size: 20.1 MB (20104176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d0a4a95f9ec2d1f831538497ba1a653c9468c8bb0e001a2f39ea2481fcb8e0`  
		Last Modified: Wed, 05 Oct 2022 17:09:52 GMT  
		Size: 192.1 MB (192146085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f1490693c6fb5c391bddcaf065d8e85cbc9a41b3fa5b44a08d77f42e1bbd31`  
		Last Modified: Wed, 05 Oct 2022 17:09:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a0e39e56b4605e06f061cfe80897d740adfedbe2bd32bdda3d5b50d531ff1`  
		Last Modified: Thu, 06 Oct 2022 05:40:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ba5f7d4ed631679273613857d5e4ada5782796eb108ee2d66f825774c2cb18`  
		Last Modified: Thu, 06 Oct 2022 05:44:49 GMT  
		Size: 12.7 MB (12718294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89acf6d4bf9a5c5bc0adea23c0dbe47a9f1f1a44ad651b443260a4c23adccd44`  
		Last Modified: Thu, 06 Oct 2022 05:44:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52803a12fa8e3da0e659035745a421916d555b85af202401a41910e1e618dbf`  
		Last Modified: Thu, 06 Oct 2022 09:57:23 GMT  
		Size: 4.4 MB (4397160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98eda955d39d200d66c889b8471de009670ab25ee9fd81cf4188ebd30d78bc3`  
		Last Modified: Thu, 06 Oct 2022 09:57:23 GMT  
		Size: 938.7 KB (938672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77132e1d2bdb94fa798c3b883c60f0a170b44688dd7776974d28b724f94704d`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 4.6 KB (4584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17002aef77c534bb598190fc2ca1f7615dfe957bf3c479a89d04b4df3b76b647`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 27.6 KB (27554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f0fa447e6d4ee16f3b862beca5d1c793f47aacb5eceac4d5ec37026a4499de`  
		Last Modified: Thu, 06 Oct 2022 09:57:26 GMT  
		Size: 94.1 MB (94122200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09a5d596d2b2d8001c5c42eef0ebff142d5c914fc18e40170d848cd93183c8`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b4c8f1df6423f9eb638f3934b7748595569d762be6cd7a690088a46cf78445`  
		Last Modified: Thu, 06 Oct 2022 09:57:20 GMT  
		Size: 1.5 KB (1490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
