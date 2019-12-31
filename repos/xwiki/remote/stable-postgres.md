## `xwiki:stable-postgres`

```console
$ docker pull xwiki@sha256:e53f3094a83033b5bc56e6e55799e48361624c52c8885eb63b01da98362425c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:0128a583b7288b0865b500947d80b2efa708f5b181909aae19fe515939437e22
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **714.2 MB (714230125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31e96d56097033237ac87a78c63dd6e86d816d5329b12fae8f560d310aa491fb`
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
# Mon, 30 Dec 2019 23:41:44 GMT
ENV XWIKI_VERSION=11.10.2
# Mon, 30 Dec 2019 23:41:44 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.2
# Mon, 30 Dec 2019 23:41:44 GMT
ENV XWIKI_DOWNLOAD_SHA256=a904633ccebb9570c50349479818f67fcb3482c7baa1666616f19f389dacb727
# Mon, 30 Dec 2019 23:42:16 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Mon, 30 Dec 2019 23:42:17 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Mon, 30 Dec 2019 23:42:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Mon, 30 Dec 2019 23:42:18 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Mon, 30 Dec 2019 23:42:18 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Mon, 30 Dec 2019 23:42:19 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 30 Dec 2019 23:42:19 GMT
VOLUME [/usr/local/xwiki]
# Mon, 30 Dec 2019 23:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 30 Dec 2019 23:42:19 GMT
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
	-	`sha256:527da95d62edba631cf27dd01987742e71deb8b34a162a572570c80b67aec82c`  
		Last Modified: Mon, 30 Dec 2019 23:43:25 GMT  
		Size: 284.9 MB (284876821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fe190d48e30ec9bfe1e3c23695aae75211cfecc7b1a18a1389923d410ae37d`  
		Last Modified: Mon, 30 Dec 2019 23:43:07 GMT  
		Size: 618.9 KB (618856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f321d198dad7ace7cc1e5dbbdd00d59070fa88395f65aaf10a3140a03fb609c`  
		Last Modified: Mon, 30 Dec 2019 23:43:07 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530973a5d0cdd654b5d9247dc18b12060e959acfb21b42db8261a8b98d3a7f67`  
		Last Modified: Mon, 30 Dec 2019 23:43:07 GMT  
		Size: 2.5 KB (2473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3535df20ec083fb948720caa4e4d91668686e74712471d47bdce1bc4ca5eb5`  
		Last Modified: Mon, 30 Dec 2019 23:43:08 GMT  
		Size: 4.3 KB (4265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff17f10dc72be95766c1dd811b547f5ef0b2720bc7f71756fa6253514e1a8ba6`  
		Last Modified: Mon, 30 Dec 2019 23:43:07 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ffdfa413ce5824f1e06caba1f159b28c4bd13f3b81ae7de63dc224c95fe6e34e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **704.9 MB (704923247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7699822e2a7018ba077a517904362af215642f00fd416f4d8ca2ecfb50980927`
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
# Mon, 30 Dec 2019 22:58:13 GMT
ENV XWIKI_VERSION=11.10.2
# Mon, 30 Dec 2019 22:58:13 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/11.10.2
# Mon, 30 Dec 2019 22:58:14 GMT
ENV XWIKI_DOWNLOAD_SHA256=a904633ccebb9570c50349479818f67fcb3482c7baa1666616f19f389dacb727
# Mon, 30 Dec 2019 22:59:01 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Mon, 30 Dec 2019 22:59:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Mon, 30 Dec 2019 22:59:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Mon, 30 Dec 2019 22:59:06 GMT
COPY file:bb513b07693b0f03295b679c3da15a7fa3d7769583b3db4897a41cfec3529978 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Mon, 30 Dec 2019 22:59:08 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Mon, 30 Dec 2019 22:59:09 GMT
COPY file:1aeb90632849dc8f47315bba1c63b571b0f210b5f223333b3a494c471e4b9743 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 30 Dec 2019 22:59:10 GMT
VOLUME [/usr/local/xwiki]
# Mon, 30 Dec 2019 22:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 30 Dec 2019 22:59:11 GMT
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
	-	`sha256:4a71565a9f0e4cb6c8f7be4a921d31d7d8acb7d81fff89b65189e5947b669554`  
		Last Modified: Mon, 30 Dec 2019 22:59:52 GMT  
		Size: 284.9 MB (284876820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce054b788b254452621817530ec6b4025a26980d70861f614e60e2e9b49824e`  
		Last Modified: Mon, 30 Dec 2019 22:59:20 GMT  
		Size: 618.9 KB (618864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401e89a4eccbcfe7f37bf2491f3e76c5ed64f81130d0c57f7ad33520700fb7aa`  
		Last Modified: Mon, 30 Dec 2019 22:59:20 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003c960e49a4556cdf5e075dd0b9428796263f9a8b0569f818232d0d28f1f95f`  
		Last Modified: Mon, 30 Dec 2019 22:59:20 GMT  
		Size: 2.5 KB (2475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f665d942578aed0c5c82fada4b87118d1433177019792d3333af4e5878c9cbb4`  
		Last Modified: Mon, 30 Dec 2019 22:59:20 GMT  
		Size: 4.3 KB (4267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1f4db8765a345899a038af174a2a225270d09ff0e49a1c9de95ac25d0e7adf`  
		Last Modified: Mon, 30 Dec 2019 22:59:21 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
