<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `xwiki`

-	[`xwiki:10`](#xwiki10)
-	[`xwiki:10.11`](#xwiki1011)
-	[`xwiki:10.11.10`](#xwiki101110)
-	[`xwiki:10.11.10-postgres-tomcat`](#xwiki101110-postgres-tomcat)
-	[`xwiki:10.11-postgres-tomcat`](#xwiki1011-postgres-tomcat)
-	[`xwiki:10-mysql-tomcat`](#xwiki10-mysql-tomcat)
-	[`xwiki:10-postgres-tomcat`](#xwiki10-postgres-tomcat)
-	[`xwiki:11`](#xwiki11)
-	[`xwiki:11.10`](#xwiki1110)
-	[`xwiki:11.10.1`](#xwiki11101)
-	[`xwiki:11.10.1-mysql-tomcat`](#xwiki11101-mysql-tomcat)
-	[`xwiki:11.10.1-postgres-tomcat`](#xwiki11101-postgres-tomcat)
-	[`xwiki:11.10-mysql-tomcat`](#xwiki1110-mysql-tomcat)
-	[`xwiki:11.10-postgres-tomcat`](#xwiki1110-postgres-tomcat)
-	[`xwiki:11-mysql-tomcat`](#xwiki11-mysql-tomcat)
-	[`xwiki:11-postgres-tomcat`](#xwiki11-postgres-tomcat)
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

## `xwiki:10`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:10.11`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10.11` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:10.11.10`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10.11.10` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:10.11.10-postgres-tomcat`

```console
$ docker pull xwiki@sha256:4529279b6e198f3fd5812dbe45719e6901678713c2082fe1d2ba881f7d110399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10.11.10-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:f98aa8c81653fb9666afa7ccf64d774147564d25289d7f46db0036fbcb605cca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.5 MB (582531422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e21d1c403a538177acd77eb3d28c1b702f36fb2c498f9398af6b7796ca5ee5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:34:29 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:34:29 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:34:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:35:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:35:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:35:04 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:35:04 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:35:04 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb902e6c6f49874baa982d195c2fb9a0f35626795c41c35a812e4d57952d60d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:32 GMT  
		Size: 179.6 MB (179561790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bd4c892de3cb5c92b26d75ddfcd0cd4e0bb3227e156288959f6991431285`  
		Last Modified: Thu, 19 Dec 2019 11:39:34 GMT  
		Size: 245.9 MB (245948291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0dfb6ef6e2413e90aeb6a3137b55d20ee0a433ed7d595f42b0942cdf7ae0d6`  
		Last Modified: Thu, 19 Dec 2019 11:39:00 GMT  
		Size: 618.9 KB (618862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb946f4daf4e74b50dc53ecff1f874754d68b8869bd6b5a3475ad42e14ae51e`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62c6c0bc3b6dfd611cad0a1e098e905558aa21aeab161a51bad65622175351`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478816a5266fd1955eee53d0536c997efab1ff47f5a1582fcac9bfd34838dd2d`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f2dade4a3e2c2e4b308b3c511a7de8fca644c6fe973c797b8698abab7dd32`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:10.11-postgres-tomcat`

```console
$ docker pull xwiki@sha256:4529279b6e198f3fd5812dbe45719e6901678713c2082fe1d2ba881f7d110399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10.11-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:f98aa8c81653fb9666afa7ccf64d774147564d25289d7f46db0036fbcb605cca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.5 MB (582531422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e21d1c403a538177acd77eb3d28c1b702f36fb2c498f9398af6b7796ca5ee5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:34:29 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:34:29 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:34:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:35:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:35:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:35:04 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:35:04 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:35:04 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb902e6c6f49874baa982d195c2fb9a0f35626795c41c35a812e4d57952d60d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:32 GMT  
		Size: 179.6 MB (179561790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bd4c892de3cb5c92b26d75ddfcd0cd4e0bb3227e156288959f6991431285`  
		Last Modified: Thu, 19 Dec 2019 11:39:34 GMT  
		Size: 245.9 MB (245948291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0dfb6ef6e2413e90aeb6a3137b55d20ee0a433ed7d595f42b0942cdf7ae0d6`  
		Last Modified: Thu, 19 Dec 2019 11:39:00 GMT  
		Size: 618.9 KB (618862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb946f4daf4e74b50dc53ecff1f874754d68b8869bd6b5a3475ad42e14ae51e`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62c6c0bc3b6dfd611cad0a1e098e905558aa21aeab161a51bad65622175351`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478816a5266fd1955eee53d0536c997efab1ff47f5a1582fcac9bfd34838dd2d`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f2dade4a3e2c2e4b308b3c511a7de8fca644c6fe973c797b8698abab7dd32`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:10-mysql-tomcat`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:10-postgres-tomcat`

```console
$ docker pull xwiki@sha256:4529279b6e198f3fd5812dbe45719e6901678713c2082fe1d2ba881f7d110399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:10-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:f98aa8c81653fb9666afa7ccf64d774147564d25289d7f46db0036fbcb605cca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.5 MB (582531422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e21d1c403a538177acd77eb3d28c1b702f36fb2c498f9398af6b7796ca5ee5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:34:29 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:34:29 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:34:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:35:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:35:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:35:04 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:35:04 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:35:04 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb902e6c6f49874baa982d195c2fb9a0f35626795c41c35a812e4d57952d60d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:32 GMT  
		Size: 179.6 MB (179561790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bd4c892de3cb5c92b26d75ddfcd0cd4e0bb3227e156288959f6991431285`  
		Last Modified: Thu, 19 Dec 2019 11:39:34 GMT  
		Size: 245.9 MB (245948291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0dfb6ef6e2413e90aeb6a3137b55d20ee0a433ed7d595f42b0942cdf7ae0d6`  
		Last Modified: Thu, 19 Dec 2019 11:39:00 GMT  
		Size: 618.9 KB (618862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb946f4daf4e74b50dc53ecff1f874754d68b8869bd6b5a3475ad42e14ae51e`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62c6c0bc3b6dfd611cad0a1e098e905558aa21aeab161a51bad65622175351`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478816a5266fd1955eee53d0536c997efab1ff47f5a1582fcac9bfd34838dd2d`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f2dade4a3e2c2e4b308b3c511a7de8fca644c6fe973c797b8698abab7dd32`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10.1`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10.1` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10.1-mysql-tomcat`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10.1-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10.1-postgres-tomcat`

```console
$ docker pull xwiki@sha256:31d7beb881ca1371578a4a43f4f4e7a1998b1e066860a7ba5e4b318f90d0f12c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:11.10.1-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:3321129b125b13bf9d7bff63c3a0482c22ce2c3b4a5d18e5963cc8a8fff30dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.2 MB (714229245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1adce750c46875582d69665c702b9073cd7fd191b6354379e21f544e452a1d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:37:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:38:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:38:01 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:38:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:38:02 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:38:03 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:38:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:38:03 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69943fde18eac83505490ef3c735f32ebcf733b9fad6f5591e62603830c12381`  
		Last Modified: Thu, 19 Dec 2019 11:41:29 GMT  
		Size: 179.6 MB (179561789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd6f0f6c2a5be960b57e7146bcb4b0f15b8288f29c802120b3e2f712b6cd8`  
		Last Modified: Thu, 19 Dec 2019 11:41:15 GMT  
		Size: 284.9 MB (284875943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b167be9a63b332f805beefc3f813edb5d48723f42c48a5efd2122aa463e32f1`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 618.9 KB (618857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb828d4b1d899c58cd2cf4f3e08ea1a4e8227ac3b72802ad83345229eb77f0c`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e68be997c4840a5afe035ce917748b3a7da4b9e40391a7a0ae994e6121173b4`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ce23f6b8dac4883b072833d527df94b69caef40d50fb108e41bdf822a7ceda`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c77d6e21d24a7a3ffbd7eb37af0457d15e0e978b45f0e47bcfdddb4ef4d12a`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:11.10.1-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:631a67798319a23d13699dec868f0606961ac1d5f2986cafa2a439de9f8496ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.9 MB (704922429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86e792018cddc6225bf1c0413a677fd9ed65a61cdfba58476fc248bbe44777d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 22:58:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 31 Oct 2019 22:59:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:59:31 GMT
ENV JAVA_VERSION=jdk-11.0.4+11
# Thu, 31 Oct 2019 22:59:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='10e33e1862638e11a9158947b3d7b461727d8e396e378b171be1eb4dfe12f1ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.4_11.tar.gz';          ;;        armhf)          ESUM='19f16c4b905055a13457d06ce9a107a54289d3828bf3ae378efc6deb908a5572';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_arm_linux_hotspot_11.0.4_11.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fc6b616f83fea033edd836c934f3e70764b5aa1dac0446df8a8b49297ca40a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.4_11.tar.gz';          ;;        s390x)          ESUM='9487d27ef65b0cc30481cd0d23466aa6b36c90dfaa8a033166fad67bc37891de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.4_11.tar.gz';          ;;        amd64|x86_64)          ESUM='90c33cf3f2ed0bd773f648815de7347e69cfbb3416ef3bf41616ab1c4aa0f5a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_x64_linux_hotspot_11.0.4_11.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 31 Oct 2019 22:59:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Oct 2019 22:59:45 GMT
CMD ["jshell"]
# Fri, 01 Nov 2019 00:54:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Nov 2019 00:54:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Nov 2019 00:54:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Nov 2019 00:54:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Nov 2019 00:54:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:54:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:58:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 01 Nov 2019 00:58:57 GMT
ENV TOMCAT_MAJOR=8
# Fri, 01 Nov 2019 00:58:58 GMT
ENV TOMCAT_VERSION=8.5.47
# Fri, 01 Nov 2019 00:58:59 GMT
ENV TOMCAT_SHA512=079b85f3dfca2b137634859208fae6012860201d720d12ff0add3473f1e267d332cb12803958754e1f922599e0d42b7e97f00bcd62584d9148a6f45fde091716
# Fri, 01 Nov 2019 01:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 01 Nov 2019 01:00:14 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Nov 2019 01:00:15 GMT
EXPOSE 8080
# Fri, 01 Nov 2019 01:00:16 GMT
CMD ["catalina.sh" "run"]
# Fri, 01 Nov 2019 03:06:35 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Fri, 01 Nov 2019 03:08:14 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 12 Dec 2019 23:49:06 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 12 Dec 2019 23:49:43 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 12 Dec 2019 23:49:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 12 Dec 2019 23:49:51 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 12 Dec 2019 23:49:52 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Dec 2019 23:49:53 GMT
VOLUME [/usr/local/xwiki]
# Thu, 12 Dec 2019 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Dec 2019 23:49:54 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb929685f4a20d12d37720cde265d3c645d4ec19fbad4db50c81055be5dc25`  
		Last Modified: Thu, 31 Oct 2019 23:01:25 GMT  
		Size: 10.3 MB (10302431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f97f7ce919af2f9159d99882e078d186fa21bd16fef68532d6d679dbb389a43`  
		Last Modified: Thu, 31 Oct 2019 23:02:34 GMT  
		Size: 195.8 MB (195795958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1369695cb0e6be805a7fb3ebf715b726667d3a44b224c59a81c3acb6ea30c96`  
		Last Modified: Fri, 01 Nov 2019 01:04:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8015e1bb0fce9b00f8c17cd5260da9d7875cd7377207869c7a087484b5dfff98`  
		Last Modified: Fri, 01 Nov 2019 01:05:33 GMT  
		Size: 11.2 MB (11239631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad26d06758724e70fdb865a1f4ad39f82059c1db54a8ecb33f98ac2bacc5c1`  
		Last Modified: Fri, 01 Nov 2019 01:05:31 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a9061f184009145ffdc5b158c43877d7e1ae74e5b55e0af4fd8f311cc32af7`  
		Last Modified: Fri, 01 Nov 2019 03:10:13 GMT  
		Size: 178.3 MB (178324032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bca1c1572be382f59f19d495fb87349aeb0fa24b78e8abc71b028bad892fa8`  
		Last Modified: Thu, 12 Dec 2019 23:50:41 GMT  
		Size: 284.9 MB (284875995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3034216b3b1ae3e56b71ca9b196ef2d49d9c9f3ce275e782937fc3d1ed4c87b`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 618.9 KB (618865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79649a8ce7b7e556409909b70ca92c934aee7cb79682bd8f7c424cff2627e4e`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a5489428b3fd471c6d02936d9a5c16519794cf7f2b19152f93fddb0119006`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869106b4c709279f1123b07f550a94076396db8e8d64282e4ab05f87a6af8e66`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24dc36343a305a6172e49daabcc2a637014cb517f6d9c537fd4e9378de75ce1`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10-mysql-tomcat`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11.10-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11.10-postgres-tomcat`

```console
$ docker pull xwiki@sha256:31d7beb881ca1371578a4a43f4f4e7a1998b1e066860a7ba5e4b318f90d0f12c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:11.10-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:3321129b125b13bf9d7bff63c3a0482c22ce2c3b4a5d18e5963cc8a8fff30dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.2 MB (714229245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1adce750c46875582d69665c702b9073cd7fd191b6354379e21f544e452a1d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:37:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:38:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:38:01 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:38:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:38:02 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:38:03 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:38:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:38:03 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69943fde18eac83505490ef3c735f32ebcf733b9fad6f5591e62603830c12381`  
		Last Modified: Thu, 19 Dec 2019 11:41:29 GMT  
		Size: 179.6 MB (179561789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd6f0f6c2a5be960b57e7146bcb4b0f15b8288f29c802120b3e2f712b6cd8`  
		Last Modified: Thu, 19 Dec 2019 11:41:15 GMT  
		Size: 284.9 MB (284875943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b167be9a63b332f805beefc3f813edb5d48723f42c48a5efd2122aa463e32f1`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 618.9 KB (618857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb828d4b1d899c58cd2cf4f3e08ea1a4e8227ac3b72802ad83345229eb77f0c`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e68be997c4840a5afe035ce917748b3a7da4b9e40391a7a0ae994e6121173b4`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ce23f6b8dac4883b072833d527df94b69caef40d50fb108e41bdf822a7ceda`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c77d6e21d24a7a3ffbd7eb37af0457d15e0e978b45f0e47bcfdddb4ef4d12a`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:11.10-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:631a67798319a23d13699dec868f0606961ac1d5f2986cafa2a439de9f8496ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.9 MB (704922429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86e792018cddc6225bf1c0413a677fd9ed65a61cdfba58476fc248bbe44777d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 22:58:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 31 Oct 2019 22:59:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:59:31 GMT
ENV JAVA_VERSION=jdk-11.0.4+11
# Thu, 31 Oct 2019 22:59:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='10e33e1862638e11a9158947b3d7b461727d8e396e378b171be1eb4dfe12f1ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.4_11.tar.gz';          ;;        armhf)          ESUM='19f16c4b905055a13457d06ce9a107a54289d3828bf3ae378efc6deb908a5572';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_arm_linux_hotspot_11.0.4_11.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fc6b616f83fea033edd836c934f3e70764b5aa1dac0446df8a8b49297ca40a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.4_11.tar.gz';          ;;        s390x)          ESUM='9487d27ef65b0cc30481cd0d23466aa6b36c90dfaa8a033166fad67bc37891de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.4_11.tar.gz';          ;;        amd64|x86_64)          ESUM='90c33cf3f2ed0bd773f648815de7347e69cfbb3416ef3bf41616ab1c4aa0f5a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_x64_linux_hotspot_11.0.4_11.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 31 Oct 2019 22:59:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Oct 2019 22:59:45 GMT
CMD ["jshell"]
# Fri, 01 Nov 2019 00:54:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Nov 2019 00:54:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Nov 2019 00:54:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Nov 2019 00:54:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Nov 2019 00:54:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:54:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:58:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 01 Nov 2019 00:58:57 GMT
ENV TOMCAT_MAJOR=8
# Fri, 01 Nov 2019 00:58:58 GMT
ENV TOMCAT_VERSION=8.5.47
# Fri, 01 Nov 2019 00:58:59 GMT
ENV TOMCAT_SHA512=079b85f3dfca2b137634859208fae6012860201d720d12ff0add3473f1e267d332cb12803958754e1f922599e0d42b7e97f00bcd62584d9148a6f45fde091716
# Fri, 01 Nov 2019 01:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 01 Nov 2019 01:00:14 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Nov 2019 01:00:15 GMT
EXPOSE 8080
# Fri, 01 Nov 2019 01:00:16 GMT
CMD ["catalina.sh" "run"]
# Fri, 01 Nov 2019 03:06:35 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Fri, 01 Nov 2019 03:08:14 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 12 Dec 2019 23:49:06 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 12 Dec 2019 23:49:43 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 12 Dec 2019 23:49:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 12 Dec 2019 23:49:51 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 12 Dec 2019 23:49:52 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Dec 2019 23:49:53 GMT
VOLUME [/usr/local/xwiki]
# Thu, 12 Dec 2019 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Dec 2019 23:49:54 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb929685f4a20d12d37720cde265d3c645d4ec19fbad4db50c81055be5dc25`  
		Last Modified: Thu, 31 Oct 2019 23:01:25 GMT  
		Size: 10.3 MB (10302431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f97f7ce919af2f9159d99882e078d186fa21bd16fef68532d6d679dbb389a43`  
		Last Modified: Thu, 31 Oct 2019 23:02:34 GMT  
		Size: 195.8 MB (195795958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1369695cb0e6be805a7fb3ebf715b726667d3a44b224c59a81c3acb6ea30c96`  
		Last Modified: Fri, 01 Nov 2019 01:04:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8015e1bb0fce9b00f8c17cd5260da9d7875cd7377207869c7a087484b5dfff98`  
		Last Modified: Fri, 01 Nov 2019 01:05:33 GMT  
		Size: 11.2 MB (11239631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad26d06758724e70fdb865a1f4ad39f82059c1db54a8ecb33f98ac2bacc5c1`  
		Last Modified: Fri, 01 Nov 2019 01:05:31 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a9061f184009145ffdc5b158c43877d7e1ae74e5b55e0af4fd8f311cc32af7`  
		Last Modified: Fri, 01 Nov 2019 03:10:13 GMT  
		Size: 178.3 MB (178324032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bca1c1572be382f59f19d495fb87349aeb0fa24b78e8abc71b028bad892fa8`  
		Last Modified: Thu, 12 Dec 2019 23:50:41 GMT  
		Size: 284.9 MB (284875995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3034216b3b1ae3e56b71ca9b196ef2d49d9c9f3ce275e782937fc3d1ed4c87b`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 618.9 KB (618865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79649a8ce7b7e556409909b70ca92c934aee7cb79682bd8f7c424cff2627e4e`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a5489428b3fd471c6d02936d9a5c16519794cf7f2b19152f93fddb0119006`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869106b4c709279f1123b07f550a94076396db8e8d64282e4ab05f87a6af8e66`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24dc36343a305a6172e49daabcc2a637014cb517f6d9c537fd4e9378de75ce1`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11-mysql-tomcat`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:11-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:11-postgres-tomcat`

```console
$ docker pull xwiki@sha256:31d7beb881ca1371578a4a43f4f4e7a1998b1e066860a7ba5e4b318f90d0f12c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:11-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:3321129b125b13bf9d7bff63c3a0482c22ce2c3b4a5d18e5963cc8a8fff30dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.2 MB (714229245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1adce750c46875582d69665c702b9073cd7fd191b6354379e21f544e452a1d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:37:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:38:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:38:01 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:38:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:38:02 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:38:03 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:38:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:38:03 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69943fde18eac83505490ef3c735f32ebcf733b9fad6f5591e62603830c12381`  
		Last Modified: Thu, 19 Dec 2019 11:41:29 GMT  
		Size: 179.6 MB (179561789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd6f0f6c2a5be960b57e7146bcb4b0f15b8288f29c802120b3e2f712b6cd8`  
		Last Modified: Thu, 19 Dec 2019 11:41:15 GMT  
		Size: 284.9 MB (284875943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b167be9a63b332f805beefc3f813edb5d48723f42c48a5efd2122aa463e32f1`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 618.9 KB (618857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb828d4b1d899c58cd2cf4f3e08ea1a4e8227ac3b72802ad83345229eb77f0c`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e68be997c4840a5afe035ce917748b3a7da4b9e40391a7a0ae994e6121173b4`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ce23f6b8dac4883b072833d527df94b69caef40d50fb108e41bdf822a7ceda`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c77d6e21d24a7a3ffbd7eb37af0457d15e0e978b45f0e47bcfdddb4ef4d12a`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:11-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:631a67798319a23d13699dec868f0606961ac1d5f2986cafa2a439de9f8496ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.9 MB (704922429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86e792018cddc6225bf1c0413a677fd9ed65a61cdfba58476fc248bbe44777d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 22:58:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 31 Oct 2019 22:59:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:59:31 GMT
ENV JAVA_VERSION=jdk-11.0.4+11
# Thu, 31 Oct 2019 22:59:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='10e33e1862638e11a9158947b3d7b461727d8e396e378b171be1eb4dfe12f1ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.4_11.tar.gz';          ;;        armhf)          ESUM='19f16c4b905055a13457d06ce9a107a54289d3828bf3ae378efc6deb908a5572';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_arm_linux_hotspot_11.0.4_11.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fc6b616f83fea033edd836c934f3e70764b5aa1dac0446df8a8b49297ca40a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.4_11.tar.gz';          ;;        s390x)          ESUM='9487d27ef65b0cc30481cd0d23466aa6b36c90dfaa8a033166fad67bc37891de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.4_11.tar.gz';          ;;        amd64|x86_64)          ESUM='90c33cf3f2ed0bd773f648815de7347e69cfbb3416ef3bf41616ab1c4aa0f5a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_x64_linux_hotspot_11.0.4_11.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 31 Oct 2019 22:59:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Oct 2019 22:59:45 GMT
CMD ["jshell"]
# Fri, 01 Nov 2019 00:54:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Nov 2019 00:54:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Nov 2019 00:54:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Nov 2019 00:54:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Nov 2019 00:54:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:54:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:58:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 01 Nov 2019 00:58:57 GMT
ENV TOMCAT_MAJOR=8
# Fri, 01 Nov 2019 00:58:58 GMT
ENV TOMCAT_VERSION=8.5.47
# Fri, 01 Nov 2019 00:58:59 GMT
ENV TOMCAT_SHA512=079b85f3dfca2b137634859208fae6012860201d720d12ff0add3473f1e267d332cb12803958754e1f922599e0d42b7e97f00bcd62584d9148a6f45fde091716
# Fri, 01 Nov 2019 01:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 01 Nov 2019 01:00:14 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Nov 2019 01:00:15 GMT
EXPOSE 8080
# Fri, 01 Nov 2019 01:00:16 GMT
CMD ["catalina.sh" "run"]
# Fri, 01 Nov 2019 03:06:35 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Fri, 01 Nov 2019 03:08:14 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 12 Dec 2019 23:49:06 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 12 Dec 2019 23:49:43 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 12 Dec 2019 23:49:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 12 Dec 2019 23:49:51 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 12 Dec 2019 23:49:52 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Dec 2019 23:49:53 GMT
VOLUME [/usr/local/xwiki]
# Thu, 12 Dec 2019 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Dec 2019 23:49:54 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb929685f4a20d12d37720cde265d3c645d4ec19fbad4db50c81055be5dc25`  
		Last Modified: Thu, 31 Oct 2019 23:01:25 GMT  
		Size: 10.3 MB (10302431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f97f7ce919af2f9159d99882e078d186fa21bd16fef68532d6d679dbb389a43`  
		Last Modified: Thu, 31 Oct 2019 23:02:34 GMT  
		Size: 195.8 MB (195795958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1369695cb0e6be805a7fb3ebf715b726667d3a44b224c59a81c3acb6ea30c96`  
		Last Modified: Fri, 01 Nov 2019 01:04:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8015e1bb0fce9b00f8c17cd5260da9d7875cd7377207869c7a087484b5dfff98`  
		Last Modified: Fri, 01 Nov 2019 01:05:33 GMT  
		Size: 11.2 MB (11239631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad26d06758724e70fdb865a1f4ad39f82059c1db54a8ecb33f98ac2bacc5c1`  
		Last Modified: Fri, 01 Nov 2019 01:05:31 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a9061f184009145ffdc5b158c43877d7e1ae74e5b55e0af4fd8f311cc32af7`  
		Last Modified: Fri, 01 Nov 2019 03:10:13 GMT  
		Size: 178.3 MB (178324032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bca1c1572be382f59f19d495fb87349aeb0fa24b78e8abc71b028bad892fa8`  
		Last Modified: Thu, 12 Dec 2019 23:50:41 GMT  
		Size: 284.9 MB (284875995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3034216b3b1ae3e56b71ca9b196ef2d49d9c9f3ce275e782937fc3d1ed4c87b`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 618.9 KB (618865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79649a8ce7b7e556409909b70ca92c934aee7cb79682bd8f7c424cff2627e4e`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a5489428b3fd471c6d02936d9a5c16519794cf7f2b19152f93fddb0119006`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869106b4c709279f1123b07f550a94076396db8e8d64282e4ab05f87a6af8e66`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24dc36343a305a6172e49daabcc2a637014cb517f6d9c537fd4e9378de75ce1`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:latest`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:latest` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mysql`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts-mysql` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-postgres`

```console
$ docker pull xwiki@sha256:4529279b6e198f3fd5812dbe45719e6901678713c2082fe1d2ba881f7d110399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:f98aa8c81653fb9666afa7ccf64d774147564d25289d7f46db0036fbcb605cca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.5 MB (582531422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e21d1c403a538177acd77eb3d28c1b702f36fb2c498f9398af6b7796ca5ee5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:34:29 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:34:29 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:34:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:35:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:35:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:35:04 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:35:04 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:35:04 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb902e6c6f49874baa982d195c2fb9a0f35626795c41c35a812e4d57952d60d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:32 GMT  
		Size: 179.6 MB (179561790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bd4c892de3cb5c92b26d75ddfcd0cd4e0bb3227e156288959f6991431285`  
		Last Modified: Thu, 19 Dec 2019 11:39:34 GMT  
		Size: 245.9 MB (245948291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0dfb6ef6e2413e90aeb6a3137b55d20ee0a433ed7d595f42b0942cdf7ae0d6`  
		Last Modified: Thu, 19 Dec 2019 11:39:00 GMT  
		Size: 618.9 KB (618862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb946f4daf4e74b50dc53ecff1f874754d68b8869bd6b5a3475ad42e14ae51e`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62c6c0bc3b6dfd611cad0a1e098e905558aa21aeab161a51bad65622175351`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478816a5266fd1955eee53d0536c997efab1ff47f5a1582fcac9bfd34838dd2d`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f2dade4a3e2c2e4b308b3c511a7de8fca644c6fe973c797b8698abab7dd32`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-postgres-tomcat`

```console
$ docker pull xwiki@sha256:4529279b6e198f3fd5812dbe45719e6901678713c2082fe1d2ba881f7d110399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:lts-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:f98aa8c81653fb9666afa7ccf64d774147564d25289d7f46db0036fbcb605cca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.5 MB (582531422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e21d1c403a538177acd77eb3d28c1b702f36fb2c498f9398af6b7796ca5ee5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:34:29 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:34:29 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:34:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:35:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:35:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:35:04 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:35:04 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:35:04 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb902e6c6f49874baa982d195c2fb9a0f35626795c41c35a812e4d57952d60d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:32 GMT  
		Size: 179.6 MB (179561790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bd4c892de3cb5c92b26d75ddfcd0cd4e0bb3227e156288959f6991431285`  
		Last Modified: Thu, 19 Dec 2019 11:39:34 GMT  
		Size: 245.9 MB (245948291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0dfb6ef6e2413e90aeb6a3137b55d20ee0a433ed7d595f42b0942cdf7ae0d6`  
		Last Modified: Thu, 19 Dec 2019 11:39:00 GMT  
		Size: 618.9 KB (618862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb946f4daf4e74b50dc53ecff1f874754d68b8869bd6b5a3475ad42e14ae51e`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62c6c0bc3b6dfd611cad0a1e098e905558aa21aeab161a51bad65622175351`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478816a5266fd1955eee53d0536c997efab1ff47f5a1582fcac9bfd34838dd2d`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f2dade4a3e2c2e4b308b3c511a7de8fca644c6fe973c797b8698abab7dd32`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:mysql-tomcat`

```console
$ docker pull xwiki@sha256:c5f193adb873679ef66c3f1dc923605ef35234a999510e6343cd86a877a30c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:673b1a2884c3dfecabdc59e1637edbcce9d7a27823ffdda941fcd4365d4a24d2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **583.2 MB (583203795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1621377d5bc3923a0cc5d64fc2904c259e512e9fa27e847eea7b27002b45967e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:33:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:33:03 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:33:34 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:33:34 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:33:35 GMT
COPY file:c4e95f70490b423a9379f336f8f4d780824e06f56fa73bc69a238e245b53e842 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:33:36 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:33:36 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:33:36 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:33:36 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2ebe2fddc325517743f6cb40c1ec6ab8869520f11bd8148f592d36859e081e`  
		Last Modified: Thu, 19 Dec 2019 11:38:50 GMT  
		Size: 179.9 MB (179897623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c3d51f6f66cfa3c8b6e5c28315daf47f86efaa0c3cc0207bf171450c33397e`  
		Last Modified: Thu, 19 Dec 2019 11:38:37 GMT  
		Size: 245.9 MB (245948226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d9899a35b4ee225e1760874abae7b7987d1d39b32b30a2970e0b45090a60f`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 955.6 KB (955601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec8d54e5a60ec249f0b1efa6a5159b3e4ec929dd27e4b0ee6829d554eaa3820`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d162923d09b2043f12ddabe02e0cbe2dad755b7540ccfcc46e078c2d9575e27`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c879c5136943b62701d27d42a0695992052843538fba397f6fdb7bcde77c7ea`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab197f8b5382f91a5aac7b5159f4358d35357be2c5cfb4c00ae066041ac6fed8`  
		Last Modified: Thu, 19 Dec 2019 11:38:18 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:postgres-tomcat`

```console
$ docker pull xwiki@sha256:4529279b6e198f3fd5812dbe45719e6901678713c2082fe1d2ba881f7d110399
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:f98aa8c81653fb9666afa7ccf64d774147564d25289d7f46db0036fbcb605cca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.5 MB (582531422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e21d1c403a538177acd77eb3d28c1b702f36fb2c498f9398af6b7796ca5ee5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:09 GMT
ENV JAVA_VERSION=jdk8u232-b09
# Thu, 19 Dec 2019 06:44:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='da87bdc04b47477b42afc76066dbd96efa35ad967238be03a0081f8840e893a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u232b09.tar.gz';          ;;        s390x)          ESUM='bd20cb8bf4cfab9d3e2b2ccfb9a6f9eda1e4e67b4103b9975d29de12c05ad1f5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_s390x_linux_hotspot_8u232b09.tar.gz';          ;;        amd64|x86_64)          ESUM='7b7884f2eb2ba2d47f4c0bf3bb1a2a95b73a3a7734bd47ebf9798483a7bcc423';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u232-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u232b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:58:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:58:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:58:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:58:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:58:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:01:59 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:01:59 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:02:00 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:02:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:02:40 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:02:40 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:02:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:31:29 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:34:29 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:34:29 GMT
ENV XWIKI_VERSION=10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/10.11.10
# Thu, 19 Dec 2019 11:34:30 GMT
ENV XWIKI_DOWNLOAD_SHA256=e1feedd24f0a27ba4e36464913a2fcb43a60f9310283a8a6be017a1979618bb7
# Thu, 19 Dec 2019 11:34:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:35:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:35:03 GMT
COPY file:bd68ae28ec068b0f89a2e05a10b1098af3b375c97a69f9255831e8fa6e87f773 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:35:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:35:04 GMT
COPY file:815463388fe7ed027546f64c4118a53d9979192231bb194a93fb02ffcb9bf5c1 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:35:04 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:35:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:35:04 GMT
CMD ["xwiki"]
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
	-	`sha256:596d6c23adc7886652eea636e0c856146cc51d2da380a735645fad034dfe5069`  
		Last Modified: Thu, 19 Dec 2019 06:47:29 GMT  
		Size: 105.1 MB (105052689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e5ff6d891b0060d65b87f7018164a705f0e63aa3236cecbdf59eaa0518f5bf`  
		Last Modified: Thu, 19 Dec 2019 10:05:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f7e2eec54aa3018522efe592252c41d7dc1046d306c64bd0b002886c329499`  
		Last Modified: Thu, 19 Dec 2019 10:06:18 GMT  
		Size: 11.3 MB (11290426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c6e56851d23d673537a79706b89e76324cc2192f277907a086ddea4f15e21c`  
		Last Modified: Thu, 19 Dec 2019 10:06:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb902e6c6f49874baa982d195c2fb9a0f35626795c41c35a812e4d57952d60d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:32 GMT  
		Size: 179.6 MB (179561790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bd4c892de3cb5c92b26d75ddfcd0cd4e0bb3227e156288959f6991431285`  
		Last Modified: Thu, 19 Dec 2019 11:39:34 GMT  
		Size: 245.9 MB (245948291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0dfb6ef6e2413e90aeb6a3137b55d20ee0a433ed7d595f42b0942cdf7ae0d6`  
		Last Modified: Thu, 19 Dec 2019 11:39:00 GMT  
		Size: 618.9 KB (618862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb946f4daf4e74b50dc53ecff1f874754d68b8869bd6b5a3475ad42e14ae51e`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e62c6c0bc3b6dfd611cad0a1e098e905558aa21aeab161a51bad65622175351`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478816a5266fd1955eee53d0536c997efab1ff47f5a1582fcac9bfd34838dd2d`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 3.8 KB (3838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24f2dade4a3e2c2e4b308b3c511a7de8fca644c6fe973c797b8698abab7dd32`  
		Last Modified: Thu, 19 Dec 2019 11:38:59 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:stable` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mysql`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:stable-mysql` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mysql-tomcat`

```console
$ docker pull xwiki@sha256:25999c3eed2ba158b26fb2982ea1d9e09d116836b642214c8c880403003d3ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `xwiki:stable-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:ddd7130c50d39049633fb6477537c5bda70ef532c1faf6903854aba871211f07
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.9 MB (714901452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e8705e691f18214cae6d0bbd858d3b1de0ca3dca0970c6cb762b38d784a5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:35:57 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libmysql-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:35:58 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:36:32 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:36:33 GMT
RUN cp /usr/share/java/mysql-connector-java-*.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:36:33 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:36:34 GMT
COPY file:406eb381f87e0aed57baf469c64efee52199868e8fc75ff865a9661b47910460 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:36:34 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:36:35 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:36:35 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:36:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:36:35 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0258ffffcc748d158d335ddeaa2e79c0fa75a27d916680e09018e6dcf25cbecc`  
		Last Modified: Thu, 19 Dec 2019 11:40:36 GMT  
		Size: 179.9 MB (179897337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c04b52f6b570bec78fb87a9f8afc2a59d14ae1db54430466c7d05d79e17027`  
		Last Modified: Thu, 19 Dec 2019 11:40:26 GMT  
		Size: 284.9 MB (284876009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a549679e7292bdba2a9e942537ff2fe4a9244cdf025b361427de2873e427d033`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 955.6 KB (955595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca4cb7ec0dccf7fa4e778858c04f4b16b90923e3204f26b9bf8828a43834497`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01159027fbcaea960620ed3959eb3cdcfcdd889a850fa94c3793b1ed2175602`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.3 KB (2331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e68e3858b4714d83d7ed519044f3cd0f74b71de607c2221d694df4586fc5d0`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 4.3 KB (4264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f90bb9713d82079075a403b7a418bece9f46e73f4ef81bbe7829ab81e3827b8`  
		Last Modified: Thu, 19 Dec 2019 11:39:59 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-postgres`

```console
$ docker pull xwiki@sha256:31d7beb881ca1371578a4a43f4f4e7a1998b1e066860a7ba5e4b318f90d0f12c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:3321129b125b13bf9d7bff63c3a0482c22ce2c3b4a5d18e5963cc8a8fff30dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.2 MB (714229245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1adce750c46875582d69665c702b9073cd7fd191b6354379e21f544e452a1d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:37:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:38:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:38:01 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:38:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:38:02 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:38:03 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:38:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:38:03 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69943fde18eac83505490ef3c735f32ebcf733b9fad6f5591e62603830c12381`  
		Last Modified: Thu, 19 Dec 2019 11:41:29 GMT  
		Size: 179.6 MB (179561789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd6f0f6c2a5be960b57e7146bcb4b0f15b8288f29c802120b3e2f712b6cd8`  
		Last Modified: Thu, 19 Dec 2019 11:41:15 GMT  
		Size: 284.9 MB (284875943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b167be9a63b332f805beefc3f813edb5d48723f42c48a5efd2122aa463e32f1`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 618.9 KB (618857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb828d4b1d899c58cd2cf4f3e08ea1a4e8227ac3b72802ad83345229eb77f0c`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e68be997c4840a5afe035ce917748b3a7da4b9e40391a7a0ae994e6121173b4`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ce23f6b8dac4883b072833d527df94b69caef40d50fb108e41bdf822a7ceda`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c77d6e21d24a7a3ffbd7eb37af0457d15e0e978b45f0e47bcfdddb4ef4d12a`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:631a67798319a23d13699dec868f0606961ac1d5f2986cafa2a439de9f8496ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.9 MB (704922429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86e792018cddc6225bf1c0413a677fd9ed65a61cdfba58476fc248bbe44777d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 22:58:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 31 Oct 2019 22:59:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:59:31 GMT
ENV JAVA_VERSION=jdk-11.0.4+11
# Thu, 31 Oct 2019 22:59:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='10e33e1862638e11a9158947b3d7b461727d8e396e378b171be1eb4dfe12f1ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.4_11.tar.gz';          ;;        armhf)          ESUM='19f16c4b905055a13457d06ce9a107a54289d3828bf3ae378efc6deb908a5572';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_arm_linux_hotspot_11.0.4_11.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fc6b616f83fea033edd836c934f3e70764b5aa1dac0446df8a8b49297ca40a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.4_11.tar.gz';          ;;        s390x)          ESUM='9487d27ef65b0cc30481cd0d23466aa6b36c90dfaa8a033166fad67bc37891de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.4_11.tar.gz';          ;;        amd64|x86_64)          ESUM='90c33cf3f2ed0bd773f648815de7347e69cfbb3416ef3bf41616ab1c4aa0f5a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_x64_linux_hotspot_11.0.4_11.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 31 Oct 2019 22:59:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Oct 2019 22:59:45 GMT
CMD ["jshell"]
# Fri, 01 Nov 2019 00:54:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Nov 2019 00:54:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Nov 2019 00:54:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Nov 2019 00:54:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Nov 2019 00:54:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:54:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:58:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 01 Nov 2019 00:58:57 GMT
ENV TOMCAT_MAJOR=8
# Fri, 01 Nov 2019 00:58:58 GMT
ENV TOMCAT_VERSION=8.5.47
# Fri, 01 Nov 2019 00:58:59 GMT
ENV TOMCAT_SHA512=079b85f3dfca2b137634859208fae6012860201d720d12ff0add3473f1e267d332cb12803958754e1f922599e0d42b7e97f00bcd62584d9148a6f45fde091716
# Fri, 01 Nov 2019 01:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 01 Nov 2019 01:00:14 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Nov 2019 01:00:15 GMT
EXPOSE 8080
# Fri, 01 Nov 2019 01:00:16 GMT
CMD ["catalina.sh" "run"]
# Fri, 01 Nov 2019 03:06:35 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Fri, 01 Nov 2019 03:08:14 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 12 Dec 2019 23:49:06 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 12 Dec 2019 23:49:43 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 12 Dec 2019 23:49:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 12 Dec 2019 23:49:51 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 12 Dec 2019 23:49:52 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Dec 2019 23:49:53 GMT
VOLUME [/usr/local/xwiki]
# Thu, 12 Dec 2019 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Dec 2019 23:49:54 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb929685f4a20d12d37720cde265d3c645d4ec19fbad4db50c81055be5dc25`  
		Last Modified: Thu, 31 Oct 2019 23:01:25 GMT  
		Size: 10.3 MB (10302431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f97f7ce919af2f9159d99882e078d186fa21bd16fef68532d6d679dbb389a43`  
		Last Modified: Thu, 31 Oct 2019 23:02:34 GMT  
		Size: 195.8 MB (195795958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1369695cb0e6be805a7fb3ebf715b726667d3a44b224c59a81c3acb6ea30c96`  
		Last Modified: Fri, 01 Nov 2019 01:04:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8015e1bb0fce9b00f8c17cd5260da9d7875cd7377207869c7a087484b5dfff98`  
		Last Modified: Fri, 01 Nov 2019 01:05:33 GMT  
		Size: 11.2 MB (11239631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad26d06758724e70fdb865a1f4ad39f82059c1db54a8ecb33f98ac2bacc5c1`  
		Last Modified: Fri, 01 Nov 2019 01:05:31 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a9061f184009145ffdc5b158c43877d7e1ae74e5b55e0af4fd8f311cc32af7`  
		Last Modified: Fri, 01 Nov 2019 03:10:13 GMT  
		Size: 178.3 MB (178324032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bca1c1572be382f59f19d495fb87349aeb0fa24b78e8abc71b028bad892fa8`  
		Last Modified: Thu, 12 Dec 2019 23:50:41 GMT  
		Size: 284.9 MB (284875995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3034216b3b1ae3e56b71ca9b196ef2d49d9c9f3ce275e782937fc3d1ed4c87b`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 618.9 KB (618865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79649a8ce7b7e556409909b70ca92c934aee7cb79682bd8f7c424cff2627e4e`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a5489428b3fd471c6d02936d9a5c16519794cf7f2b19152f93fddb0119006`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869106b4c709279f1123b07f550a94076396db8e8d64282e4ab05f87a6af8e66`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24dc36343a305a6172e49daabcc2a637014cb517f6d9c537fd4e9378de75ce1`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-postgres-tomcat`

```console
$ docker pull xwiki@sha256:31d7beb881ca1371578a4a43f4f4e7a1998b1e066860a7ba5e4b318f90d0f12c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:3321129b125b13bf9d7bff63c3a0482c22ce2c3b4a5d18e5963cc8a8fff30dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.2 MB (714229245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1adce750c46875582d69665c702b9073cd7fd191b6354379e21f544e452a1d00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Thu, 19 Dec 2019 06:44:33 GMT
ENV JAVA_VERSION=jdk-11.0.5+10
# Thu, 19 Dec 2019 06:44:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        armhf)          ESUM='c6b1fda3f8807028cbfcc34a4ded2e8a5a6b6239d2bcc1f06673ea6b1530df94';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.5_10.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d763481ddc29ac0bdefb24216b3a0bf9afbb058552682567a075f9c0f7da5814';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.5_10.tar.gz';          ;;        amd64|x86_64)          ESUM='6dd0c9c8a740e6c19149e98034fba8e368fd9aa16ab417aa636854d40db1a161';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.5%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.5_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 19 Dec 2019 06:44:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 06:44:47 GMT
CMD ["jshell"]
# Thu, 19 Dec 2019 09:56:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 19 Dec 2019 09:56:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Dec 2019 09:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 19 Dec 2019 09:56:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 19 Dec 2019 09:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 09:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 19 Dec 2019 10:00:17 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_MAJOR=8
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_VERSION=8.5.50
# Thu, 19 Dec 2019 10:00:18 GMT
ENV TOMCAT_SHA512=ffca86027d298ba107c7d01c779318c05b61ba48767cc5967ee6ce5a88271bb6ec8eed60708d45453f30eeedddcaedd1a369d6df1b49eea2cd14fa40832cfb90
# Thu, 19 Dec 2019 10:00:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Thu, 19 Dec 2019 10:00:53 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 19 Dec 2019 10:00:53 GMT
EXPOSE 8080
# Thu, 19 Dec 2019 10:00:53 GMT
CMD ["catalina.sh" "run"]
# Thu, 19 Dec 2019 11:35:11 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Thu, 19 Dec 2019 11:37:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 19 Dec 2019 11:37:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 19 Dec 2019 11:38:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 19 Dec 2019 11:38:01 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 19 Dec 2019 11:38:01 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 19 Dec 2019 11:38:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 19 Dec 2019 11:38:02 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 11:38:03 GMT
VOLUME [/usr/local/xwiki]
# Thu, 19 Dec 2019 11:38:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 11:38:03 GMT
CMD ["xwiki"]
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
	-	`sha256:f3a5601342fdc19041e774599a3a5f0e49e747e6ff8a02429de43656a48d5790`  
		Last Modified: Thu, 19 Dec 2019 06:48:02 GMT  
		Size: 197.8 MB (197822308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6e638c3f1e77e75cffcd292e6443a6094610ab5ab1306de15622a68dc26582`  
		Last Modified: Thu, 19 Dec 2019 10:05:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc4533e46bdd27c17a28cabd4317add264d6f59fb638ab1b95671062a2d75c`  
		Last Modified: Thu, 19 Dec 2019 10:06:04 GMT  
		Size: 11.3 MB (11290564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553c751188238a7a12fcada06b7f83a3b5aa27be8d77781f938d246bf262d61a`  
		Last Modified: Thu, 19 Dec 2019 10:06:02 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69943fde18eac83505490ef3c735f32ebcf733b9fad6f5591e62603830c12381`  
		Last Modified: Thu, 19 Dec 2019 11:41:29 GMT  
		Size: 179.6 MB (179561789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fd6f0f6c2a5be960b57e7146bcb4b0f15b8288f29c802120b3e2f712b6cd8`  
		Last Modified: Thu, 19 Dec 2019 11:41:15 GMT  
		Size: 284.9 MB (284875943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b167be9a63b332f805beefc3f813edb5d48723f42c48a5efd2122aa463e32f1`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 618.9 KB (618857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb828d4b1d899c58cd2cf4f3e08ea1a4e8227ac3b72802ad83345229eb77f0c`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e68be997c4840a5afe035ce917748b3a7da4b9e40391a7a0ae994e6121173b4`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ce23f6b8dac4883b072833d527df94b69caef40d50fb108e41bdf822a7ceda`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c77d6e21d24a7a3ffbd7eb37af0457d15e0e978b45f0e47bcfdddb4ef4d12a`  
		Last Modified: Thu, 19 Dec 2019 11:40:52 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:631a67798319a23d13699dec868f0606961ac1d5f2986cafa2a439de9f8496ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.9 MB (704922429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f86e792018cddc6225bf1c0413a677fd9ed65a61cdfba58476fc248bbe44777d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 31 Oct 2019 22:40:37 GMT
ADD file:4c6cab77271e86386e8f3d4ecf06c17a3e9339481bea878a706d2c5dc4a0addd in / 
# Thu, 31 Oct 2019 22:40:40 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:40:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:40:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:40:44 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 22:58:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 31 Oct 2019 22:59:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends curl ca-certificates locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 22:59:31 GMT
ENV JAVA_VERSION=jdk-11.0.4+11
# Thu, 31 Oct 2019 22:59:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='10e33e1862638e11a9158947b3d7b461727d8e396e378b171be1eb4dfe12f1ed';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.4_11.tar.gz';          ;;        armhf)          ESUM='19f16c4b905055a13457d06ce9a107a54289d3828bf3ae378efc6deb908a5572';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_arm_linux_hotspot_11.0.4_11.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='fc6b616f83fea033edd836c934f3e70764b5aa1dac0446df8a8b49297ca40a5e';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.4_11.tar.gz';          ;;        s390x)          ESUM='9487d27ef65b0cc30481cd0d23466aa6b36c90dfaa8a033166fad67bc37891de';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.4_11.tar.gz';          ;;        amd64|x86_64)          ESUM='90c33cf3f2ed0bd773f648815de7347e69cfbb3416ef3bf41616ab1c4aa0f5a8';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.4%2B11/OpenJDK11U-jdk_x64_linux_hotspot_11.0.4_11.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 31 Oct 2019 22:59:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Oct 2019 22:59:45 GMT
CMD ["jshell"]
# Fri, 01 Nov 2019 00:54:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 01 Nov 2019 00:54:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Nov 2019 00:54:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 01 Nov 2019 00:54:51 GMT
WORKDIR /usr/local/tomcat
# Fri, 01 Nov 2019 00:54:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:54:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 01 Nov 2019 00:58:57 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Fri, 01 Nov 2019 00:58:57 GMT
ENV TOMCAT_MAJOR=8
# Fri, 01 Nov 2019 00:58:58 GMT
ENV TOMCAT_VERSION=8.5.47
# Fri, 01 Nov 2019 00:58:59 GMT
ENV TOMCAT_SHA512=079b85f3dfca2b137634859208fae6012860201d720d12ff0add3473f1e267d332cb12803958754e1f922599e0d42b7e97f00bcd62584d9148a6f45fde091716
# Fri, 01 Nov 2019 01:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work
# Fri, 01 Nov 2019 01:00:14 GMT
RUN set -e 	&& nativeLines="$(catalina.sh configtest 2>&1)" 	&& nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')" 	&& nativeLines="$(echo "$nativeLines" | sort -u)" 	&& if ! echo "$nativeLines" | grep 'INFO: Loaded APR based Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 01 Nov 2019 01:00:15 GMT
EXPOSE 8080
# Fri, 01 Nov 2019 01:00:16 GMT
CMD ["catalina.sh" "run"]
# Fri, 01 Nov 2019 03:06:35 GMT
MAINTAINER Vincent Massol <vincent@massol.net>
# Fri, 01 Nov 2019 03:08:14 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 12 Dec 2019 23:49:06 GMT
ENV XWIKI_VERSION=11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.1
# Thu, 12 Dec 2019 23:49:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=531c105af1848274185f3472a2d0f1c6de9c046ea64d0efba4f657545fc247be
# Thu, 12 Dec 2019 23:49:43 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 12 Dec 2019 23:49:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 12 Dec 2019 23:49:49 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 12 Dec 2019 23:49:51 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 12 Dec 2019 23:49:52 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 12 Dec 2019 23:49:53 GMT
VOLUME [/usr/local/xwiki]
# Thu, 12 Dec 2019 23:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Dec 2019 23:49:54 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6531af3558948c8839fd7cc7eb7062aa86bfae891870ccaafd554ac65c97971b`  
		Last Modified: Thu, 31 Oct 2019 22:42:23 GMT  
		Size: 23.7 MB (23718403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7942d2fb7381ee1735a4c972ef45c89b6521902e6eba024d4791dfd069def`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 35.2 KB (35198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce94e690d563311eb8b102b49e94a01b2a4c965daa9e33d5e59168dc4327e0`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96a89ada1c32e30a1998945a8785c18bcdce55dcfe2b666bb587d432255cb11`  
		Last Modified: Thu, 31 Oct 2019 22:42:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb929685f4a20d12d37720cde265d3c645d4ec19fbad4db50c81055be5dc25`  
		Last Modified: Thu, 31 Oct 2019 23:01:25 GMT  
		Size: 10.3 MB (10302431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f97f7ce919af2f9159d99882e078d186fa21bd16fef68532d6d679dbb389a43`  
		Last Modified: Thu, 31 Oct 2019 23:02:34 GMT  
		Size: 195.8 MB (195795958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1369695cb0e6be805a7fb3ebf715b726667d3a44b224c59a81c3acb6ea30c96`  
		Last Modified: Fri, 01 Nov 2019 01:04:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8015e1bb0fce9b00f8c17cd5260da9d7875cd7377207869c7a087484b5dfff98`  
		Last Modified: Fri, 01 Nov 2019 01:05:33 GMT  
		Size: 11.2 MB (11239631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad26d06758724e70fdb865a1f4ad39f82059c1db54a8ecb33f98ac2bacc5c1`  
		Last Modified: Fri, 01 Nov 2019 01:05:31 GMT  
		Size: 164.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a9061f184009145ffdc5b158c43877d7e1ae74e5b55e0af4fd8f311cc32af7`  
		Last Modified: Fri, 01 Nov 2019 03:10:13 GMT  
		Size: 178.3 MB (178324032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bca1c1572be382f59f19d495fb87349aeb0fa24b78e8abc71b028bad892fa8`  
		Last Modified: Thu, 12 Dec 2019 23:50:41 GMT  
		Size: 284.9 MB (284875995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3034216b3b1ae3e56b71ca9b196ef2d49d9c9f3ce275e782937fc3d1ed4c87b`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 618.9 KB (618865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79649a8ce7b7e556409909b70ca92c934aee7cb79682bd8f7c424cff2627e4e`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6a5489428b3fd471c6d02936d9a5c16519794cf7f2b19152f93fddb0119006`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869106b4c709279f1123b07f550a94076396db8e8d64282e4ab05f87a6af8e66`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 4.3 KB (4269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24dc36343a305a6172e49daabcc2a637014cb517f6d9c537fd4e9378de75ce1`  
		Last Modified: Thu, 12 Dec 2019 23:50:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
