## `tomcat:10-jdk8-adoptopenjdk-hotspot`

```console
$ docker pull tomcat@sha256:aba2791de810d3aaa48eb662b3166baf9e87b1549601d5b9cda47084449f5f2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:10-jdk8-adoptopenjdk-hotspot` - linux; amd64

```console
$ docker pull tomcat@sha256:64e5d2a7d1e456a5794ce6bcc694f1c7e0b35bc247900ce798aacb2662cd609a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160942700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157e5694014460cbdade392100e9608bfe6e9b8b5c79948e6bad88f0c06b6b5c`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:08 GMT
ADD file:a8d2f02fbaddf8cec8e4da320cd03c06435f395e9d454f69954efe422eb6e1ba in / 
# Thu, 25 Mar 2021 22:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:11 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:11 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 09:57:14 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 26 Mar 2021 09:58:10 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:58:10 GMT
ENV JAVA_VERSION=jdk8u282-b08
# Fri, 26 Mar 2021 09:58:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='d69bd545691058b55337d2a5eb1092880a5cab0753ede4d82b181242aac8a8fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u282b08.tar.gz';          ;;        s390x)          ESUM='040cde56788a803a6972af9e5d4985dbb8d698e6691c3aa0edfc765e91aeea33';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_s390x_linux_hotspot_8u282b08.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='e6e6e0356649b9696fa5082cfcb0663d4bef159fc22d406e3a012e71fce83a5c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u282b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 26 Mar 2021 09:58:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 18:27:08 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 26 Mar 2021 18:27:08 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 18:27:09 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 26 Mar 2021 18:27:10 GMT
WORKDIR /usr/local/tomcat
# Fri, 26 Mar 2021 18:27:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 26 Mar 2021 18:27:10 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 26 Mar 2021 18:27:10 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 26 Mar 2021 18:27:11 GMT
ENV TOMCAT_MAJOR=10
# Fri, 26 Mar 2021 18:27:11 GMT
ENV TOMCAT_VERSION=10.0.4
# Fri, 26 Mar 2021 18:27:11 GMT
ENV TOMCAT_SHA512=c88e2068e33ed0e08985770da252440f3341c6e1ef7198aacba84492084ada3cd888f7fe52297898f44668672b80c97a39057b8c46a9dcdc4c981d36c05a9969
# Fri, 26 Mar 2021 18:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Fri, 26 Mar 2021 18:28:17 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 26 Mar 2021 18:28:17 GMT
EXPOSE 8080
# Fri, 26 Mar 2021 18:28:18 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:04a5f4cda3eea2313a61a2f72208342a57ea36a9326dff54f4f26ed47d145c7c`  
		Last Modified: Thu, 25 Mar 2021 22:34:46 GMT  
		Size: 28.6 MB (28569428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff496a88c8ed9b745dab2f00bfbd9013c6d1db198442a6a8683998a29a85458a`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce83f459fe7e0bf459d0c222ef3b2ca4d9911f6b0f9aae02c2120561b54ca18`  
		Last Modified: Thu, 25 Mar 2021 22:34:37 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6315e58a4fe1441064bfd504990b519f51bf9e2c0318a7b2f7f18c6dc8c0812`  
		Last Modified: Fri, 26 Mar 2021 10:09:22 GMT  
		Size: 16.0 MB (16033051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95544a631453a086b2ce2748d5e2baf9e753a84324e868d45be42c91f339308b`  
		Last Modified: Fri, 26 Mar 2021 10:09:30 GMT  
		Size: 103.4 MB (103400554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79355d7d9c0e0ba43ae342dc248b5010f913733b3e707c42b3466a95133085f6`  
		Last Modified: Fri, 26 Mar 2021 18:49:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d384ef65ceb0ab108720562c037b28d386b1f9f7771ee966a6d36f2e9fc93ac8`  
		Last Modified: Fri, 26 Mar 2021 18:49:40 GMT  
		Size: 12.9 MB (12938326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740786b964ae2669de92caf5ca7fe6065c4443b88e76bb929d391fd65898b462`  
		Last Modified: Fri, 26 Mar 2021 18:49:36 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk8-adoptopenjdk-hotspot` - linux; ppc64le

```console
$ docker pull tomcat@sha256:b352ac8dd795fb371265a5c305a562e5a75b2715d842a7a666193ae2a08140c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.4 MB (164397135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a083d78ed8f7ff96ab40d0cf91d2cce24b86fa70d564e9baba8a844038195df`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 04 Mar 2021 02:57:39 GMT
ADD file:b709cd21d0acd910f23e8ad46933746a841aeac2e6e28c7c42fe92616cdbfa0d in / 
# Thu, 04 Mar 2021 02:58:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:58:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:58:41 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:58:46 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:20:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 04 Mar 2021 03:26:27 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:26:35 GMT
ENV JAVA_VERSION=jdk8u282-b08
# Thu, 04 Mar 2021 03:27:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='d69bd545691058b55337d2a5eb1092880a5cab0753ede4d82b181242aac8a8fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u282b08.tar.gz';          ;;        s390x)          ESUM='040cde56788a803a6972af9e5d4985dbb8d698e6691c3aa0edfc765e91aeea33';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_s390x_linux_hotspot_8u282b08.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='e6e6e0356649b9696fa5082cfcb0663d4bef159fc22d406e3a012e71fce83a5c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u282b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 04 Mar 2021 03:27:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 02:13:10 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Mar 2021 02:13:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 02:13:25 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Mar 2021 02:13:29 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Mar 2021 02:13:35 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Mar 2021 02:13:42 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Mar 2021 02:13:47 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Mar 2021 02:13:54 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Mar 2021 02:14:01 GMT
ENV TOMCAT_VERSION=10.0.4
# Thu, 11 Mar 2021 02:14:08 GMT
ENV TOMCAT_SHA512=c88e2068e33ed0e08985770da252440f3341c6e1ef7198aacba84492084ada3cd888f7fe52297898f44668672b80c97a39057b8c46a9dcdc4c981d36c05a9969
# Thu, 11 Mar 2021 02:21:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 11 Mar 2021 02:22:15 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Mar 2021 02:22:26 GMT
EXPOSE 8080
# Thu, 11 Mar 2021 02:22:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6340e19a714d2edb6591a3c7a742db49afda548f15fb462e592a6c2f4783fbb6`  
		Last Modified: Mon, 22 Feb 2021 16:18:13 GMT  
		Size: 33.3 MB (33279996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596b04c7047b52ebc24e2f93ba001030d6500a930738602afcd7d5b793cd0074`  
		Last Modified: Thu, 04 Mar 2021 03:02:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d017db017688e47f4621a1ee72d3f358aed2f118ae88144b9453be0044dd8daf`  
		Last Modified: Thu, 04 Mar 2021 03:02:07 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334b1128d6e933464fd8278724d2de3f5499c61253a2e9beee32fe89b744d6e5`  
		Last Modified: Thu, 04 Mar 2021 03:56:14 GMT  
		Size: 17.2 MB (17207685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f970ccf2d4d91b1bc64bcaa5d1809d7fc2ef0d56df43277cccb2cd5e235fb877`  
		Last Modified: Thu, 04 Mar 2021 03:56:24 GMT  
		Size: 100.9 MB (100903623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410d4c933c4c1e1fb90c7b956f83456aad23268b7979e610432b180cddfbc678`  
		Last Modified: Thu, 11 Mar 2021 04:23:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff4b006c9fa56e1daf83d3a58540e60d72c5bad12d03f42f4640072f47245d4`  
		Last Modified: Thu, 11 Mar 2021 04:23:29 GMT  
		Size: 13.0 MB (13004490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc04d135d56a706177ca1d16dc9915b11b16e1495bcbb4dc4114619dd2e22c17`  
		Last Modified: Thu, 11 Mar 2021 04:23:29 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk8-adoptopenjdk-hotspot` - linux; s390x

```console
$ docker pull tomcat@sha256:a75206af62addafef6d736db334c3667b631e43e50f600da0d4827d61bf95405
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154386035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10b1d1dc86ea3a505ecfa8a8b8444d422fcff6e14b306ffa17a718922d4ba95`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:39 GMT
ADD file:1969d90a813b25d38c41fc98f6c3deaac4bfefd16fcb6d1b2f76f7f7d8368d9c in / 
# Thu, 04 Mar 2021 02:47:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:43 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:43 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:04:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 04 Mar 2021 03:04:42 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:04:43 GMT
ENV JAVA_VERSION=jdk8u282-b08
# Thu, 04 Mar 2021 03:04:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        ppc64el|ppc64le)          ESUM='d69bd545691058b55337d2a5eb1092880a5cab0753ede4d82b181242aac8a8fe';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u282b08.tar.gz';          ;;        s390x)          ESUM='040cde56788a803a6972af9e5d4985dbb8d698e6691c3aa0edfc765e91aeea33';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_s390x_linux_hotspot_8u282b08.tar.gz';          LIBFFI_SUM='05e456a2e8ad9f20db846ccb96c483235c3243e27025c3e8e8e358411fd48be9';          LIBFFI_URL='http://launchpadlibrarian.net/354371408/libffi6_3.2.1-8_s390x.deb';          curl -LfsSo /tmp/libffi6.deb ${LIBFFI_URL};          echo "${LIBFFI_SUM} /tmp/libffi6.deb" | sha256sum -c -;          apt-get install -y --no-install-recommends /tmp/libffi6.deb;          rm -rf /tmp/libffi6.deb;          ;;        amd64|x86_64)          ESUM='e6e6e0356649b9696fa5082cfcb0663d4bef159fc22d406e3a012e71fce83a5c';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk8-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_hotspot_8u282b08.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 04 Mar 2021 03:04:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 00:59:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Mar 2021 00:59:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Mar 2021 00:59:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Mar 2021 00:59:38 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Mar 2021 00:59:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Mar 2021 00:59:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Mar 2021 00:59:39 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Mar 2021 00:59:39 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Mar 2021 00:59:39 GMT
ENV TOMCAT_VERSION=10.0.4
# Thu, 11 Mar 2021 00:59:39 GMT
ENV TOMCAT_SHA512=c88e2068e33ed0e08985770da252440f3341c6e1ef7198aacba84492084ada3cd888f7fe52297898f44668672b80c97a39057b8c46a9dcdc4c981d36c05a9969
# Thu, 11 Mar 2021 01:00:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Thu, 11 Mar 2021 01:00:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Mar 2021 01:00:49 GMT
EXPOSE 8080
# Thu, 11 Mar 2021 01:00:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c50e9afb4f48654833d2e6830472f28dd58c9a469906fdeec89d4866a4c2f2cd`  
		Last Modified: Mon, 22 Feb 2021 17:49:17 GMT  
		Size: 27.2 MB (27184264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d1636aa19d4ea5d1acb9e3d2fc7e8eccdace4d5eeaa6c5f7ef4e3a333bf44c`  
		Last Modified: Thu, 04 Mar 2021 02:48:40 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34ff5c86ca0b0872a71672b70fdf570e0a99a3d6d63842f30efbdb0708feafd`  
		Last Modified: Thu, 04 Mar 2021 02:48:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58a7ba8323d85db0dbae1851b6e1cbdcf0126f4bd444c9f7be48b15f2629ceb`  
		Last Modified: Thu, 04 Mar 2021 03:21:07 GMT  
		Size: 15.7 MB (15741124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1630a909c46755d35008172d56cf07d2b96589928c72489ea04a1ba96d4aa593`  
		Last Modified: Thu, 04 Mar 2021 03:21:12 GMT  
		Size: 98.5 MB (98508697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe09f1131773aa06eca3436627e7d723c1d1fb2a212888fdb970f3e8e5a5150`  
		Last Modified: Thu, 11 Mar 2021 01:11:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cfa5f778e0df75151a3c72d652ee65cc02715a9eba2f46820fdc3d0da2bd3e`  
		Last Modified: Thu, 11 Mar 2021 01:11:28 GMT  
		Size: 13.0 MB (12950609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c7a275402ba1fc81e22067d82eb38723fde60c47152acb2953aa699a98f584`  
		Last Modified: Thu, 11 Mar 2021 01:11:27 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
