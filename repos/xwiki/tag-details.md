<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `xwiki`

-	[`xwiki:11`](#xwiki11)
-	[`xwiki:11.10`](#xwiki1110)
-	[`xwiki:11.10.3`](#xwiki11103)
-	[`xwiki:11.10.3-mysql-tomcat`](#xwiki11103-mysql-tomcat)
-	[`xwiki:11.10.3-postgres-tomcat`](#xwiki11103-postgres-tomcat)
-	[`xwiki:11.10-mysql-tomcat`](#xwiki1110-mysql-tomcat)
-	[`xwiki:11.10-postgres-tomcat`](#xwiki1110-postgres-tomcat)
-	[`xwiki:11-mysql-tomcat`](#xwiki11-mysql-tomcat)
-	[`xwiki:11-postgres-tomcat`](#xwiki11-postgres-tomcat)
-	[`xwiki:12`](#xwiki12)
-	[`xwiki:12.1`](#xwiki121)
-	[`xwiki:12.1-mysql-tomcat`](#xwiki121-mysql-tomcat)
-	[`xwiki:12.1-postgres-tomcat`](#xwiki121-postgres-tomcat)
-	[`xwiki:12-mysql-tomcat`](#xwiki12-mysql-tomcat)
-	[`xwiki:12-postgres-tomcat`](#xwiki12-postgres-tomcat)
-	[`xwiki:latest`](#xwikilatest)
-	[`xwiki:lts`](#xwikilts)
-	[`xwiki:lts-mysql`](#xwikilts-mysql)
-	[`xwiki:lts-mysql-tomcat`](#xwikilts-mysql-tomcat)
-	[`xwiki:lts-postgres`](#xwikilts-postgres)
-	[`xwiki:lts-postgres-tomcat`](#xwikilts-postgres-tomcat)
-	[`xwiki:mysql-tomcat`](#xwikimysql-tomcat)
-	[`xwiki:postgres-tomcat`](#xwikipostgres-tomcat)
-	[`xwiki:stable`](#xwikistable)
-	[`xwiki:stable-mysql`](#xwikistable-mysql)
-	[`xwiki:stable-mysql-tomcat`](#xwikistable-mysql-tomcat)
-	[`xwiki:stable-postgres`](#xwikistable-postgres)
-	[`xwiki:stable-postgres-tomcat`](#xwikistable-postgres-tomcat)

## `xwiki:11`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10.3`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10.3` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10.3-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10.3-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10.3-postgres-tomcat`

```console
$ docker pull xwiki@sha256:3f081f18dfff082babce9a5c3cc77d59df31f6281bc3fd31c36b03299b3b909d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:11.10.3-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:46d3c8e694064e7bb93d840d300c0cabc2abd6e6cb369a3e7a77dc7914c2acb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.5 MB (714529454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590e399cc38636563448f123fefd6f8167037db28c781d97e323e90edce54159`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:03:52 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:03:53 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:03:54 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:03:54 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:03:54 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:03:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:03:55 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697365c9160268e8c46cf3a9be16f0810f5fbd2c33508fad8cd48564c5efddf0`  
		Last Modified: Sat, 22 Feb 2020 03:08:13 GMT  
		Size: 284.9 MB (284905218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc33b73670622eca429847c6c68b5d3b1f5cb1be497c2ee6d2af78070c75a3`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 618.9 KB (618866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77812c483bf46c33730444783af358a085d226e13aa94340ed5d3c1fd571cb8a`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d99bc09121ea9015f27ea12a0562710e51c0729d05775503bf9ad721858ecd5`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e0775a5ac9f52d07af5069b0c265dc6386b03382e4d5431cb08da700e3e250`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a8b1cc62d68c583b06a1e36752496db63127d737e678f3882c3ae6ed6e40f`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:11.10.3-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:1d9e5e66947115a6e98df8e3d03a7cc6fd9d0fbde343aa4655268141e8996181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **705.4 MB (705449202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7346d3741c32b35141c6ce2b40c78baa57d087dc8bef2a4b105e7fd575f52fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:56:29 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 00:57:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:57:08 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:57:08 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:57:09 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:57:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:57:11 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:57:11 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:57:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:57:12 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087640a88cbeb399dc9cc3e322af444ead00b558b48820ce6496c34652825fa`  
		Last Modified: Sat, 22 Feb 2020 00:59:02 GMT  
		Size: 284.9 MB (284905267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e6ed223cf1dece4db4d7a919b0d7eeafd874d0c051793c3c22e53af26679c`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 618.9 KB (618861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12c06f2c922548b3e4d5e188bff8606fb49ca7869393e8a52e2ec0cb387cdac`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cd2d2d224f6e7bcbcf9a5922fea546cc006b05ea11e830d8f02d336a9491f2`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695767dc54e00fb51bee1751b00c2e0fd6bb4ecc5838fd2b298af0a91b747b2a`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c55b20fbc6779dd52bc6dbd3ef635d3a739e72292e175c5b4c0d7a83ad5307`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10-postgres-tomcat`

```console
$ docker pull xwiki@sha256:3f081f18dfff082babce9a5c3cc77d59df31f6281bc3fd31c36b03299b3b909d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:11.10-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:46d3c8e694064e7bb93d840d300c0cabc2abd6e6cb369a3e7a77dc7914c2acb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.5 MB (714529454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590e399cc38636563448f123fefd6f8167037db28c781d97e323e90edce54159`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:03:52 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:03:53 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:03:54 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:03:54 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:03:54 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:03:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:03:55 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697365c9160268e8c46cf3a9be16f0810f5fbd2c33508fad8cd48564c5efddf0`  
		Last Modified: Sat, 22 Feb 2020 03:08:13 GMT  
		Size: 284.9 MB (284905218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc33b73670622eca429847c6c68b5d3b1f5cb1be497c2ee6d2af78070c75a3`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 618.9 KB (618866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77812c483bf46c33730444783af358a085d226e13aa94340ed5d3c1fd571cb8a`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d99bc09121ea9015f27ea12a0562710e51c0729d05775503bf9ad721858ecd5`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e0775a5ac9f52d07af5069b0c265dc6386b03382e4d5431cb08da700e3e250`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a8b1cc62d68c583b06a1e36752496db63127d737e678f3882c3ae6ed6e40f`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:11.10-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:1d9e5e66947115a6e98df8e3d03a7cc6fd9d0fbde343aa4655268141e8996181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **705.4 MB (705449202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7346d3741c32b35141c6ce2b40c78baa57d087dc8bef2a4b105e7fd575f52fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:56:29 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 00:57:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:57:08 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:57:08 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:57:09 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:57:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:57:11 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:57:11 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:57:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:57:12 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087640a88cbeb399dc9cc3e322af444ead00b558b48820ce6496c34652825fa`  
		Last Modified: Sat, 22 Feb 2020 00:59:02 GMT  
		Size: 284.9 MB (284905267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e6ed223cf1dece4db4d7a919b0d7eeafd874d0c051793c3c22e53af26679c`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 618.9 KB (618861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12c06f2c922548b3e4d5e188bff8606fb49ca7869393e8a52e2ec0cb387cdac`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cd2d2d224f6e7bcbcf9a5922fea546cc006b05ea11e830d8f02d336a9491f2`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695767dc54e00fb51bee1751b00c2e0fd6bb4ecc5838fd2b298af0a91b747b2a`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c55b20fbc6779dd52bc6dbd3ef635d3a739e72292e175c5b4c0d7a83ad5307`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11-postgres-tomcat`

```console
$ docker pull xwiki@sha256:3f081f18dfff082babce9a5c3cc77d59df31f6281bc3fd31c36b03299b3b909d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:11-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:46d3c8e694064e7bb93d840d300c0cabc2abd6e6cb369a3e7a77dc7914c2acb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.5 MB (714529454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590e399cc38636563448f123fefd6f8167037db28c781d97e323e90edce54159`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:03:52 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:03:53 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:03:54 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:03:54 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:03:54 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:03:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:03:55 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697365c9160268e8c46cf3a9be16f0810f5fbd2c33508fad8cd48564c5efddf0`  
		Last Modified: Sat, 22 Feb 2020 03:08:13 GMT  
		Size: 284.9 MB (284905218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc33b73670622eca429847c6c68b5d3b1f5cb1be497c2ee6d2af78070c75a3`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 618.9 KB (618866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77812c483bf46c33730444783af358a085d226e13aa94340ed5d3c1fd571cb8a`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d99bc09121ea9015f27ea12a0562710e51c0729d05775503bf9ad721858ecd5`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e0775a5ac9f52d07af5069b0c265dc6386b03382e4d5431cb08da700e3e250`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a8b1cc62d68c583b06a1e36752496db63127d737e678f3882c3ae6ed6e40f`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:11-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:1d9e5e66947115a6e98df8e3d03a7cc6fd9d0fbde343aa4655268141e8996181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **705.4 MB (705449202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7346d3741c32b35141c6ce2b40c78baa57d087dc8bef2a4b105e7fd575f52fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:56:29 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 00:57:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:57:08 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:57:08 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:57:09 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:57:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:57:11 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:57:11 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:57:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:57:12 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087640a88cbeb399dc9cc3e322af444ead00b558b48820ce6496c34652825fa`  
		Last Modified: Sat, 22 Feb 2020 00:59:02 GMT  
		Size: 284.9 MB (284905267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e6ed223cf1dece4db4d7a919b0d7eeafd874d0c051793c3c22e53af26679c`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 618.9 KB (618861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12c06f2c922548b3e4d5e188bff8606fb49ca7869393e8a52e2ec0cb387cdac`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cd2d2d224f6e7bcbcf9a5922fea546cc006b05ea11e830d8f02d336a9491f2`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695767dc54e00fb51bee1751b00c2e0fd6bb4ecc5838fd2b298af0a91b747b2a`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c55b20fbc6779dd52bc6dbd3ef635d3a739e72292e175c5b4c0d7a83ad5307`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:12`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:12` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:12.1`

```console
$ docker pull xwiki@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `xwiki:12.1-mysql-tomcat`

```console
$ docker pull xwiki@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `xwiki:12.1-postgres-tomcat`

```console
$ docker pull xwiki@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `xwiki:12-mysql-tomcat`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:12-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:12-postgres-tomcat`

```console
$ docker pull xwiki@sha256:b51df5810e3a576a28166f0ac6f53fd90ce2bcd1b0acc5bda5cab8e8fabd1576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:12-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:c44f9501658ceb7ced33cac2c438803d4d9a0418a7fcaec2194ac51a3140944c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.1 MB (716059759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87bd3ab7608b7f943856be1b9df17c7882596fa09f57ae798988a400a0db3960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:06:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:06:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:06:48 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:06:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:06:50 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:06:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:06:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073bdd9fba63d16e4c4d96e179e75edd0ba465b0b94d0590677bacf971218d2`  
		Last Modified: Sat, 22 Feb 2020 03:09:27 GMT  
		Size: 286.4 MB (286435486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a3b1f300b360bc616f72369184b302037feea2bd37c07b5bba15148dccecd0`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 618.9 KB (618858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b67426f20531d9523c4008f393441bbb12ae00eb108f2ca3e519c412a4c14`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e91337311f973295e74b723be9a90ff0959a64e9bf0f0a785de42669f65ad`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 2.5 KB (2480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e2e880f40ef91dae116dd555b97d085ad74f2be5a58418cb1730ce628e4d7`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7f1474721410c56ce931c3a58d6bee19c22524ac77dacfa8dd8afa81a8f12`  
		Last Modified: Sat, 22 Feb 2020 03:09:08 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:12-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:5b2cec72bfb4f00a40fe2ff6e4505005a189eb5cfa878fcbf85ef764e4e5a7fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **707.0 MB (706979598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad457aa7b09deb31a97d59b3513877ce486f6cd2299670cfda339ec533baa88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:57:23 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 00:57:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:58:03 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:58:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:58:04 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:58:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:58:06 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:58:07 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:58:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:58:08 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eda1534ca6cc45731380d5f44da51975869bcb60b12b30b4deb62d856b9a7`  
		Last Modified: Sat, 22 Feb 2020 01:00:06 GMT  
		Size: 286.4 MB (286435627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a996a313c76499fc79b73550a00066a75027722d0ad19d6bfb7d2f718e47bd9`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 618.9 KB (618854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c1ff703b46b96ad29c9c1b4f569c89204405f11435ad179d23db00c21c469`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca8989f730e7743799d7702767871253bed274f8cf39f0c01827409182225df`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a6c8e6da707a15d03551dac93d989a3bc03452776d430a87e64aa7fd1ae9c8`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 4.3 KB (4310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca00c930e2908b8bc04a76bc3f901733ced827553f8fd5a17475d9446ec776`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:latest`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:latest` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mysql`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts-mysql` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32c0ab0c7bc7f7f584094412ac74accd41f9aca4e9427d533af596bbf94ffa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:28fa2dd159c275b307adf032c71196a46ed26f2e8e949865e901aec02ad23d45
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **715.2 MB (715201240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302e13ed28787c494d06105bbaa56bb7d66f58452afa7f1eb3f642baa91222f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:00:18 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:01:29 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:01:30 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:01:30 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:01:31 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:01:31 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:01:31 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:01:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:01:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492972920cf34cf9f49568f59ba867e77163710936855ba0476d47317d5773a7`  
		Last Modified: Sat, 22 Feb 2020 03:07:30 GMT  
		Size: 284.9 MB (284905253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0da33c4ccd60deb469b66e41e1a6dbc02fd4f7818425945358899616d908d1`  
		Last Modified: Sat, 22 Feb 2020 03:07:10 GMT  
		Size: 955.6 KB (955598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e66ef79fa41daa45e2e3d1998edac3fc54cc7df0d64f34de3dff23d11e80dc`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21497a1b920efca1dbf1e49a9f7b2383cc04c3f4c00a66c548377f9662998bc6`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.3 KB (2332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1e4c2bfce0c6289ff4eee741adb922baa0c34344ce96682e57f87285c7c17`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 4.3 KB (4268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc1dba2a2fa7d635d570838bacb6e77e2872756fd941af7bcb13661116fc880`  
		Last Modified: Sat, 22 Feb 2020 03:07:09 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-postgres`

```console
$ docker pull xwiki@sha256:3f081f18dfff082babce9a5c3cc77d59df31f6281bc3fd31c36b03299b3b909d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:46d3c8e694064e7bb93d840d300c0cabc2abd6e6cb369a3e7a77dc7914c2acb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.5 MB (714529454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590e399cc38636563448f123fefd6f8167037db28c781d97e323e90edce54159`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:03:52 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:03:53 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:03:54 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:03:54 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:03:54 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:03:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:03:55 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697365c9160268e8c46cf3a9be16f0810f5fbd2c33508fad8cd48564c5efddf0`  
		Last Modified: Sat, 22 Feb 2020 03:08:13 GMT  
		Size: 284.9 MB (284905218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc33b73670622eca429847c6c68b5d3b1f5cb1be497c2ee6d2af78070c75a3`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 618.9 KB (618866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77812c483bf46c33730444783af358a085d226e13aa94340ed5d3c1fd571cb8a`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d99bc09121ea9015f27ea12a0562710e51c0729d05775503bf9ad721858ecd5`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e0775a5ac9f52d07af5069b0c265dc6386b03382e4d5431cb08da700e3e250`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a8b1cc62d68c583b06a1e36752496db63127d737e678f3882c3ae6ed6e40f`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:1d9e5e66947115a6e98df8e3d03a7cc6fd9d0fbde343aa4655268141e8996181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **705.4 MB (705449202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7346d3741c32b35141c6ce2b40c78baa57d087dc8bef2a4b105e7fd575f52fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:56:29 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 00:57:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:57:08 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:57:08 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:57:09 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:57:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:57:11 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:57:11 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:57:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:57:12 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087640a88cbeb399dc9cc3e322af444ead00b558b48820ce6496c34652825fa`  
		Last Modified: Sat, 22 Feb 2020 00:59:02 GMT  
		Size: 284.9 MB (284905267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e6ed223cf1dece4db4d7a919b0d7eeafd874d0c051793c3c22e53af26679c`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 618.9 KB (618861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12c06f2c922548b3e4d5e188bff8606fb49ca7869393e8a52e2ec0cb387cdac`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cd2d2d224f6e7bcbcf9a5922fea546cc006b05ea11e830d8f02d336a9491f2`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695767dc54e00fb51bee1751b00c2e0fd6bb4ecc5838fd2b298af0a91b747b2a`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c55b20fbc6779dd52bc6dbd3ef635d3a739e72292e175c5b4c0d7a83ad5307`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-postgres-tomcat`

```console
$ docker pull xwiki@sha256:3f081f18dfff082babce9a5c3cc77d59df31f6281bc3fd31c36b03299b3b909d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:46d3c8e694064e7bb93d840d300c0cabc2abd6e6cb369a3e7a77dc7914c2acb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.5 MB (714529454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590e399cc38636563448f123fefd6f8167037db28c781d97e323e90edce54159`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 03:02:22 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 03:03:52 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:03:53 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:03:53 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:03:54 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:03:54 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:03:54 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:03:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:03:55 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697365c9160268e8c46cf3a9be16f0810f5fbd2c33508fad8cd48564c5efddf0`  
		Last Modified: Sat, 22 Feb 2020 03:08:13 GMT  
		Size: 284.9 MB (284905218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cc33b73670622eca429847c6c68b5d3b1f5cb1be497c2ee6d2af78070c75a3`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 618.9 KB (618866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77812c483bf46c33730444783af358a085d226e13aa94340ed5d3c1fd571cb8a`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d99bc09121ea9015f27ea12a0562710e51c0729d05775503bf9ad721858ecd5`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e0775a5ac9f52d07af5069b0c265dc6386b03382e4d5431cb08da700e3e250`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a8b1cc62d68c583b06a1e36752496db63127d737e678f3882c3ae6ed6e40f`  
		Last Modified: Sat, 22 Feb 2020 03:07:52 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:1d9e5e66947115a6e98df8e3d03a7cc6fd9d0fbde343aa4655268141e8996181
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **705.4 MB (705449202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7346d3741c32b35141c6ce2b40c78baa57d087dc8bef2a4b105e7fd575f52fd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:56:29 GMT
ENV XWIKI_VERSION=11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.3
# Sat, 22 Feb 2020 00:56:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=fc959c8641d772d90a53bc1976e86fab907d290364cd802b7b3e0304dcbf008b
# Sat, 22 Feb 2020 00:57:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:57:08 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:57:08 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:57:09 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:57:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:57:11 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:57:11 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:57:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:57:12 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1087640a88cbeb399dc9cc3e322af444ead00b558b48820ce6496c34652825fa`  
		Last Modified: Sat, 22 Feb 2020 00:59:02 GMT  
		Size: 284.9 MB (284905267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0e6ed223cf1dece4db4d7a919b0d7eeafd874d0c051793c3c22e53af26679c`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 618.9 KB (618861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12c06f2c922548b3e4d5e188bff8606fb49ca7869393e8a52e2ec0cb387cdac`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cd2d2d224f6e7bcbcf9a5922fea546cc006b05ea11e830d8f02d336a9491f2`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695767dc54e00fb51bee1751b00c2e0fd6bb4ecc5838fd2b298af0a91b747b2a`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 4.3 KB (4270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c55b20fbc6779dd52bc6dbd3ef635d3a739e72292e175c5b4c0d7a83ad5307`  
		Last Modified: Sat, 22 Feb 2020 00:58:24 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:mysql-tomcat`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:postgres-tomcat`

```console
$ docker pull xwiki@sha256:b51df5810e3a576a28166f0ac6f53fd90ce2bcd1b0acc5bda5cab8e8fabd1576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:c44f9501658ceb7ced33cac2c438803d4d9a0418a7fcaec2194ac51a3140944c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.1 MB (716059759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87bd3ab7608b7f943856be1b9df17c7882596fa09f57ae798988a400a0db3960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:06:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:06:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:06:48 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:06:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:06:50 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:06:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:06:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073bdd9fba63d16e4c4d96e179e75edd0ba465b0b94d0590677bacf971218d2`  
		Last Modified: Sat, 22 Feb 2020 03:09:27 GMT  
		Size: 286.4 MB (286435486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a3b1f300b360bc616f72369184b302037feea2bd37c07b5bba15148dccecd0`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 618.9 KB (618858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b67426f20531d9523c4008f393441bbb12ae00eb108f2ca3e519c412a4c14`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e91337311f973295e74b723be9a90ff0959a64e9bf0f0a785de42669f65ad`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 2.5 KB (2480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e2e880f40ef91dae116dd555b97d085ad74f2be5a58418cb1730ce628e4d7`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7f1474721410c56ce931c3a58d6bee19c22524ac77dacfa8dd8afa81a8f12`  
		Last Modified: Sat, 22 Feb 2020 03:09:08 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:5b2cec72bfb4f00a40fe2ff6e4505005a189eb5cfa878fcbf85ef764e4e5a7fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **707.0 MB (706979598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad457aa7b09deb31a97d59b3513877ce486f6cd2299670cfda339ec533baa88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:57:23 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 00:57:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:58:03 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:58:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:58:04 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:58:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:58:06 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:58:07 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:58:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:58:08 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eda1534ca6cc45731380d5f44da51975869bcb60b12b30b4deb62d856b9a7`  
		Last Modified: Sat, 22 Feb 2020 01:00:06 GMT  
		Size: 286.4 MB (286435627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a996a313c76499fc79b73550a00066a75027722d0ad19d6bfb7d2f718e47bd9`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 618.9 KB (618854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c1ff703b46b96ad29c9c1b4f569c89204405f11435ad179d23db00c21c469`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca8989f730e7743799d7702767871253bed274f8cf39f0c01827409182225df`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a6c8e6da707a15d03551dac93d989a3bc03452776d430a87e64aa7fd1ae9c8`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 4.3 KB (4310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca00c930e2908b8bc04a76bc3f901733ced827553f8fd5a17475d9446ec776`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:stable` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mysql`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:stable-mysql` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mysql-tomcat`

```console
$ docker pull xwiki@sha256:585b9b5672cbe64c2055d9ea5d3c816f1185eb553ac0345fe9453bff8ca47922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:stable-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:780903a1f3ee73d4a129b77626f32f747fa64bd76cc2e4dde785c795b0b7e296
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.7 MB (716731513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981296b51122c88e2d0c1383cffb39a78312133a3cb05d2e28219adabd506500`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:00:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:04:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:04:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:04:54 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:04:54 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:04:55 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:04:55 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:04:56 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:04:56 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:04:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:04:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051324bb24fce9a3ed3fddaeebd821c5cfc94e9558645a52589f439f9e01c27`  
		Last Modified: Sat, 22 Feb 2020 03:07:41 GMT  
		Size: 179.9 MB (179897896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feba9c0928fb2808001987c38ae8207490a5da838a7cb5c04fe309c18d6bdb6`  
		Last Modified: Sat, 22 Feb 2020 03:08:56 GMT  
		Size: 286.4 MB (286435482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1ba7ff96da974a0e0d611c7a121e80c05985d478b9ff28f68791af22d72a37`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 955.6 KB (955592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ded10cf23f876026067b8be48ed61d6c4bd556206b8ec86864d93391e747b9f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4d5a2c52a1cc7876aaaaab13e194214296bf1a563d70fd6808943bf15cb2f8`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6821a91677cba3b1c2faebbecab59aa666ce04349a550ad91208f023daee0bc1`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f47f60ebca8d80f39d429dcc53f78c83fed44bd214dad6057781f723e57d4f`  
		Last Modified: Sat, 22 Feb 2020 03:08:38 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-postgres`

```console
$ docker pull xwiki@sha256:b51df5810e3a576a28166f0ac6f53fd90ce2bcd1b0acc5bda5cab8e8fabd1576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:c44f9501658ceb7ced33cac2c438803d4d9a0418a7fcaec2194ac51a3140944c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.1 MB (716059759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87bd3ab7608b7f943856be1b9df17c7882596fa09f57ae798988a400a0db3960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:06:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:06:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:06:48 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:06:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:06:50 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:06:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:06:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073bdd9fba63d16e4c4d96e179e75edd0ba465b0b94d0590677bacf971218d2`  
		Last Modified: Sat, 22 Feb 2020 03:09:27 GMT  
		Size: 286.4 MB (286435486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a3b1f300b360bc616f72369184b302037feea2bd37c07b5bba15148dccecd0`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 618.9 KB (618858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b67426f20531d9523c4008f393441bbb12ae00eb108f2ca3e519c412a4c14`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e91337311f973295e74b723be9a90ff0959a64e9bf0f0a785de42669f65ad`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 2.5 KB (2480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e2e880f40ef91dae116dd555b97d085ad74f2be5a58418cb1730ce628e4d7`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7f1474721410c56ce931c3a58d6bee19c22524ac77dacfa8dd8afa81a8f12`  
		Last Modified: Sat, 22 Feb 2020 03:09:08 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:5b2cec72bfb4f00a40fe2ff6e4505005a189eb5cfa878fcbf85ef764e4e5a7fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **707.0 MB (706979598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad457aa7b09deb31a97d59b3513877ce486f6cd2299670cfda339ec533baa88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:57:23 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 00:57:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:58:03 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:58:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:58:04 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:58:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:58:06 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:58:07 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:58:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:58:08 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eda1534ca6cc45731380d5f44da51975869bcb60b12b30b4deb62d856b9a7`  
		Last Modified: Sat, 22 Feb 2020 01:00:06 GMT  
		Size: 286.4 MB (286435627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a996a313c76499fc79b73550a00066a75027722d0ad19d6bfb7d2f718e47bd9`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 618.9 KB (618854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c1ff703b46b96ad29c9c1b4f569c89204405f11435ad179d23db00c21c469`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca8989f730e7743799d7702767871253bed274f8cf39f0c01827409182225df`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a6c8e6da707a15d03551dac93d989a3bc03452776d430a87e64aa7fd1ae9c8`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 4.3 KB (4310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca00c930e2908b8bc04a76bc3f901733ced827553f8fd5a17475d9446ec776`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-postgres-tomcat`

```console
$ docker pull xwiki@sha256:b51df5810e3a576a28166f0ac6f53fd90ce2bcd1b0acc5bda5cab8e8fabd1576
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:c44f9501658ceb7ced33cac2c438803d4d9a0418a7fcaec2194ac51a3140944c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.1 MB (716059759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87bd3ab7608b7f943856be1b9df17c7882596fa09f57ae798988a400a0db3960`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:38:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:39:14 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:39:37 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:39:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:39:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:39:48 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 02:20:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 02:20:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 02:20:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 02:20:59 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 02:21:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:21:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 02:24:31 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 02:24:31 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 02:24:32 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 02:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 02:25:05 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 02:25:05 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 02:25:05 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 02:58:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 03:02:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 03:05:01 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 03:06:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 03:06:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 03:06:48 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 03:06:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 03:06:49 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 03:06:50 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 03:06:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 03:06:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6eb45629ecf6b86562f04def09260db9e15101e2a6974e746e19e5077c1f605`  
		Last Modified: Fri, 21 Feb 2020 22:42:01 GMT  
		Size: 13.3 MB (13324026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1aa556e690a0a1c3635978da9af4e8cc08a8dbe43befe2db5462cb67ee070e`  
		Last Modified: Fri, 21 Feb 2020 22:42:43 GMT  
		Size: 198.1 MB (198075300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4fbbbd9c30fdede2d083b22168b8315c94e3ccac92f1f1d8c4f4b5ae88a958`  
		Last Modified: Sat, 22 Feb 2020 02:29:32 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ae81f9f59b586de809ddc9994f6a30cbf0895fec39fb38474ac54e73ca229`  
		Last Modified: Sat, 22 Feb 2020 02:29:58 GMT  
		Size: 11.3 MB (11304020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b9b780dfb38861b0c5fa5beec1e45957ebb8606d41437da3e9cfb85f967206`  
		Last Modified: Sat, 22 Feb 2020 02:29:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb4dbf2e63da347238386c845e7b0252837b5d0a5bf2e7e1398009ca814f661`  
		Last Modified: Sat, 22 Feb 2020 03:08:24 GMT  
		Size: 179.6 MB (179562730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7073bdd9fba63d16e4c4d96e179e75edd0ba465b0b94d0590677bacf971218d2`  
		Last Modified: Sat, 22 Feb 2020 03:09:27 GMT  
		Size: 286.4 MB (286435486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a3b1f300b360bc616f72369184b302037feea2bd37c07b5bba15148dccecd0`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 618.9 KB (618858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00b67426f20531d9523c4008f393441bbb12ae00eb108f2ca3e519c412a4c14`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e91337311f973295e74b723be9a90ff0959a64e9bf0f0a785de42669f65ad`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 2.5 KB (2480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7e2e880f40ef91dae116dd555b97d085ad74f2be5a58418cb1730ce628e4d7`  
		Last Modified: Sat, 22 Feb 2020 03:09:07 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7f1474721410c56ce931c3a58d6bee19c22524ac77dacfa8dd8afa81a8f12`  
		Last Modified: Sat, 22 Feb 2020 03:09:08 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:5b2cec72bfb4f00a40fe2ff6e4505005a189eb5cfa878fcbf85ef764e4e5a7fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **707.0 MB (706979598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dad457aa7b09deb31a97d59b3513877ce486f6cd2299670cfda339ec533baa88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 21 Feb 2020 21:54:16 GMT
ADD file:d827a0b8f08011678a718254c1220408c7e6c7ab03ae4259b415542309f18578 in / 
# Fri, 21 Feb 2020 21:54:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:54:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:54:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:54:25 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:41:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 21 Feb 2020 22:42:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:42:43 GMT
ENV JAVA_VERSION=jdk-11.0.6+10
# Fri, 21 Feb 2020 22:42:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04b77f6754aed68528f39750c5cfd6a439190206aff216aa081d62a0e1a794fa';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.6_10.tar.gz';          ;;        armhf)          ESUM='ab5b76203e54fe7a5221535f6f407efa43153de029a746f60af3cffb7cb5080b';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.6_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='9247f0271744188489b0dd628cab90e76ca1f22fa3bbcdebd9bfc4f140908df5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.6_10.tar.gz';          ;;        s390x)          ESUM='250fc79db2d6c70e655ff319e2db8ca205858bf82c9f30b040bda0c90cd9f583';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.6_10.tar.gz';          ;;        amd64|x86_64)          ESUM='330d19a2eaa07ed02757d7a785a77bab49f5ee710ea03b4ee2fa220ddd0feffc';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.6_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 21 Feb 2020 22:43:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 Feb 2020 22:43:02 GMT
CMD ["jshell"]
# Sat, 22 Feb 2020 00:29:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 22 Feb 2020 00:29:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Feb 2020 00:29:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 22 Feb 2020 00:29:11 GMT
WORKDIR /usr/local/tomcat
# Sat, 22 Feb 2020 00:29:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:29:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 22 Feb 2020 00:32:55 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Sat, 22 Feb 2020 00:32:55 GMT
ENV TOMCAT_MAJOR=8
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_VERSION=8.5.51
# Sat, 22 Feb 2020 00:32:56 GMT
ENV TOMCAT_SHA512=bb9207d33d7b4408292186523f3556a3d1454ea172b4a6cde6e0028e2f7a5d9408615cb4ccf8d9fdb75a9f8ce227580f56f929a811eb24ef99e26f980e4bcb48
# Sat, 22 Feb 2020 00:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Sat, 22 Feb 2020 00:34:07 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 22 Feb 2020 00:34:07 GMT
EXPOSE 8080
# Sat, 22 Feb 2020 00:34:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 22 Feb 2020 00:54:52 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Sat, 22 Feb 2020 00:56:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:57:23 GMT
ENV XWIKI_VERSION=12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.0
# Sat, 22 Feb 2020 00:57:24 GMT
ENV XWIKI_DOWNLOAD_SHA256=da57110002c76001dc9ca16eb217ea0d6c81a2b4bd3d8ad26a6fc5efe96c776d
# Sat, 22 Feb 2020 00:57:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 22 Feb 2020 00:58:03 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 22 Feb 2020 00:58:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 22 Feb 2020 00:58:04 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 22 Feb 2020 00:58:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 22 Feb 2020 00:58:06 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 22 Feb 2020 00:58:07 GMT
VOLUME [/usr/local/xwiki]
# Sat, 22 Feb 2020 00:58:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 22 Feb 2020 00:58:08 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6695dc10aaa5cd71c433dfb366e84804eb5fbee91eab1e113442040d6ef4c9e0`  
		Last Modified: Fri, 21 Feb 2020 21:56:13 GMT  
		Size: 23.7 MB (23721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72aab8f928deff72c9b5867c93524a60e3f8cf1b7401c88b0ede8dc3c595e828`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 35.2 KB (35197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e83b6447acdea2afff1a10052ebc551d15bfd1d2a93a202699f7a458c612c07`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a91485a919c412d218b6441c339f691079ff88e6d28734b1cc3d5938cf58d`  
		Last Modified: Fri, 21 Feb 2020 21:56:08 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b5eadacd92003b0f840ccaa2c2b09ea51d298126dd647d280a6de60720a3d4`  
		Last Modified: Fri, 21 Feb 2020 22:44:36 GMT  
		Size: 12.7 MB (12732441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64db97399f909b605c437d7e2f386a0cb47a6145f0bfb336087cfce892ebe5b8`  
		Last Modified: Fri, 21 Feb 2020 22:45:42 GMT  
		Size: 196.3 MB (196252926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc286385afab138fc4830b80a62b1f81d93fc340238e32639295f3ef5b5a0bf`  
		Last Modified: Sat, 22 Feb 2020 00:38:29 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb976737b9160563de97bc94df037965b15cf0c4621584878ae3523b9bf84ca`  
		Last Modified: Sat, 22 Feb 2020 00:38:54 GMT  
		Size: 11.3 MB (11309055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1336897db7a7bbf8eab4abdbf14c3ffd3835ac76d2f7bdc23320902aaf84af`  
		Last Modified: Sat, 22 Feb 2020 00:38:52 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d2d871b33d03eb8a3f9417d4e5dd3157996815b2ed187f082f6dead9bccc0f`  
		Last Modified: Sat, 22 Feb 2020 00:59:14 GMT  
		Size: 175.9 MB (175862387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eda1534ca6cc45731380d5f44da51975869bcb60b12b30b4deb62d856b9a7`  
		Last Modified: Sat, 22 Feb 2020 01:00:06 GMT  
		Size: 286.4 MB (286435627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a996a313c76499fc79b73550a00066a75027722d0ad19d6bfb7d2f718e47bd9`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 618.9 KB (618854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c1ff703b46b96ad29c9c1b4f569c89204405f11435ad179d23db00c21c469`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca8989f730e7743799d7702767871253bed274f8cf39f0c01827409182225df`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a6c8e6da707a15d03551dac93d989a3bc03452776d430a87e64aa7fd1ae9c8`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 4.3 KB (4310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca00c930e2908b8bc04a76bc3f901733ced827553f8fd5a17475d9446ec776`  
		Last Modified: Sat, 22 Feb 2020 00:59:26 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
