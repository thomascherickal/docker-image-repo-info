## `tomcat:10-jdk15-adoptopenjdk-openj9`

```console
$ docker pull tomcat@sha256:cb13aa14a3e7337839e765eeeb7055c25bc4a326e8562fe18cd04121b8f30fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:10-jdk15-adoptopenjdk-openj9` - linux; amd64

```console
$ docker pull tomcat@sha256:e535278b49cb7c8c8cffa06e57811381f5b90ef03eafc00f1515462f052cf946
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.9 MB (259882280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a271c3d9c35db3f98db18edbf1ed77ec0a555891910a72ce2170ce1e99388e6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:06 GMT
ADD file:27277aee655dd263ee698d1f2fe17f0b1dbba740615bcac8642723a6ac0d62be in / 
# Sat, 03 Apr 2021 00:53:07 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:08 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:09 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:09 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:29:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:29:33 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:34:34 GMT
ENV JAVA_VERSION=jdk-15.0.2+7_openj9-0.24.0
# Sat, 03 Apr 2021 01:34:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b69a4bc87ed2e985d252cff02d53f1a11b8d83d39e0800cd4a1cab4521375314';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_aarch64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b2158268de0be247801b7823ee3e7f739254d77718a1879848627181feee2f4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_ppc64le_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='0f34a9dd2b800f669e004e543529e454c047a19919ec3b423552d171cb4f2626';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_s390x_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5515ccd79b1b5e8d8a615b80d5fe1272f7bb41100e46d94fb78ee611ea014816';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_x64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 01:34:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 01:34:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 03 Apr 2021 01:35:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 03 Apr 2021 01:35:21 GMT
CMD ["jshell"]
# Tue, 06 Apr 2021 22:30:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 06 Apr 2021 22:30:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Apr 2021 22:30:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 06 Apr 2021 22:30:18 GMT
WORKDIR /usr/local/tomcat
# Tue, 06 Apr 2021 22:30:18 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 22:30:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 22:30:18 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 06 Apr 2021 22:30:18 GMT
ENV TOMCAT_MAJOR=10
# Tue, 06 Apr 2021 22:30:19 GMT
ENV TOMCAT_VERSION=10.0.5
# Tue, 06 Apr 2021 22:30:19 GMT
ENV TOMCAT_SHA512=27271e17c8daf52503490c6657c992cc150cf2942e1b0179b738f34e9aa5e1aac3c7b947c67441d17294a8f1e772a00e38e30b2135372d6ee9d71207ac7261c3
# Tue, 06 Apr 2021 22:31:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Tue, 06 Apr 2021 22:31:04 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 06 Apr 2021 22:31:04 GMT
EXPOSE 8080
# Tue, 06 Apr 2021 22:31:04 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a70d879fa5984474288d52009479054b8bb2993de2a1859f43b5480600cecb24`  
		Last Modified: Thu, 01 Apr 2021 15:20:06 GMT  
		Size: 28.6 MB (28569016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4394a92d1f8760cf7d17fee0bcee732c94c5b858dd8d19c7ff02beecf3b4e83`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6159c56c084c858f5de2416454ac0a49ddda47b764e4379c5d5a147c9bf5f`  
		Last Modified: Sat, 03 Apr 2021 00:54:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04b772c31f76720583412a2507c5c53889985db45169a85f0d3cd7f842e041a`  
		Last Modified: Sat, 03 Apr 2021 01:39:30 GMT  
		Size: 16.0 MB (16032891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7be38023a782c14359e3a29bd25b0feb487064591efa67c31fe26d3ee9a2307`  
		Last Modified: Sat, 03 Apr 2021 01:44:33 GMT  
		Size: 197.1 MB (197096694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a4c2c58f595a940946f8ffaea325b9bfc076ef15abbeda9c61b85fcd83b712`  
		Last Modified: Sat, 03 Apr 2021 01:44:18 GMT  
		Size: 5.2 MB (5239706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c802fd31767f736a90e281a08da472e8ef48e84a68f8e8c5e3f4a418cca6017`  
		Last Modified: Tue, 06 Apr 2021 23:16:17 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a588948cb45dc4b08dabeb933a8ccf502292e6343fb4fb5efdd3dc8841ad987`  
		Last Modified: Tue, 06 Apr 2021 23:16:19 GMT  
		Size: 12.9 MB (12942583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7edfb3f40ffbe224b81efb79f32818ffb83f8e87003945585973dfd86b19206`  
		Last Modified: Tue, 06 Apr 2021 23:16:17 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk15-adoptopenjdk-openj9` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:f416cdffc6f09634f185db72c9d0848e74b33a1760738b8ac6d168557650d62e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.2 MB (254193072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2ae1e7adbe872bc5a5cd502d29a8b561725e9e5586ac56cf3dbe60385bea79`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 03 Apr 2021 04:10:04 GMT
ADD file:5a9b188c70f1f07ae9d68f3eb7aa18a1683faf50d5ff20eda1b04db3255877b9 in / 
# Sat, 03 Apr 2021 04:10:08 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 04:10:11 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 04:10:13 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 04:10:14 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:27 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:41:56 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:48:03 GMT
ENV JAVA_VERSION=jdk-15.0.2+7_openj9-0.24.0
# Sat, 03 Apr 2021 05:48:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b69a4bc87ed2e985d252cff02d53f1a11b8d83d39e0800cd4a1cab4521375314';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_aarch64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b2158268de0be247801b7823ee3e7f739254d77718a1879848627181feee2f4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_ppc64le_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='0f34a9dd2b800f669e004e543529e454c047a19919ec3b423552d171cb4f2626';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_s390x_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5515ccd79b1b5e8d8a615b80d5fe1272f7bb41100e46d94fb78ee611ea014816';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_x64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 05:48:19 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 05:48:20 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 03 Apr 2021 05:48:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 03 Apr 2021 05:48:57 GMT
CMD ["jshell"]
# Tue, 06 Apr 2021 21:37:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 06 Apr 2021 21:37:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Apr 2021 21:37:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 06 Apr 2021 21:37:22 GMT
WORKDIR /usr/local/tomcat
# Tue, 06 Apr 2021 21:37:22 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 21:37:23 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 21:37:24 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 06 Apr 2021 21:37:25 GMT
ENV TOMCAT_MAJOR=10
# Tue, 06 Apr 2021 21:37:26 GMT
ENV TOMCAT_VERSION=10.0.5
# Tue, 06 Apr 2021 21:37:27 GMT
ENV TOMCAT_SHA512=27271e17c8daf52503490c6657c992cc150cf2942e1b0179b738f34e9aa5e1aac3c7b947c67441d17294a8f1e772a00e38e30b2135372d6ee9d71207ac7261c3
# Tue, 06 Apr 2021 21:38:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Tue, 06 Apr 2021 21:38:36 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 06 Apr 2021 21:38:37 GMT
EXPOSE 8080
# Tue, 06 Apr 2021 21:38:38 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2b20d1a80822f7dbd2175f235caa068029e82a265d0924d4f4d39c1bf9dc7f9b`  
		Last Modified: Thu, 01 Apr 2021 08:25:41 GMT  
		Size: 27.2 MB (27176807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e993c4ee9ad2dd0f069e7c34bbf137c835c5a2c2cc3f111e37fba05c79c1d7`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2befefc5146bc156f83e891873a69526513f1e942e3d2bf68129f1e2fa17613`  
		Last Modified: Sat, 03 Apr 2021 04:11:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f1b84b0f5e74897b899c79e269e294408197cec9b0f1770ff44d654874d22c`  
		Last Modified: Sat, 03 Apr 2021 05:53:32 GMT  
		Size: 15.9 MB (15894829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8d1cbc6b79246cfecae2fc7d17e0b48eb22761fc5bbbf51821ed127bf8b3c8`  
		Last Modified: Sat, 03 Apr 2021 05:58:32 GMT  
		Size: 193.1 MB (193102229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f66ccf7548989d5b3ffaa4a8beef889932fe2f37f1ddd8e266f20004125d216`  
		Last Modified: Sat, 03 Apr 2021 05:58:07 GMT  
		Size: 5.1 MB (5059333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7756716cd812aacc2fb723e7046e4d27ee74f860124bdf9e8188547bfe4eb132`  
		Last Modified: Tue, 06 Apr 2021 22:47:00 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9df241679415ba3057d5c740b8850577a7df6c815b2687d90a081d427b4ab2`  
		Last Modified: Tue, 06 Apr 2021 22:47:02 GMT  
		Size: 13.0 MB (12958473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e18aedb7cd4f9db21a6734476ad63696b18e1a0b8d99e7bccc9838bb630ea`  
		Last Modified: Tue, 06 Apr 2021 22:47:00 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk15-adoptopenjdk-openj9` - linux; ppc64le

```console
$ docker pull tomcat@sha256:7405907c754a9247a4683bad479b101348bce263cd526dcc0bae033968bae651
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.0 MB (266009947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d6c96985311545aac1053dfa6756495ed10f1fee9aed1d2126336886b82593`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 03 Apr 2021 02:11:32 GMT
ADD file:52b5c16e73309b9cdf3ac6dd8ce6b519d2ed0d2fa13f1dd0bc16f143241a1369 in / 
# Sat, 03 Apr 2021 02:11:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 02:12:07 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 02:12:27 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 02:12:35 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 05:41:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 05:43:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 05:54:16 GMT
ENV JAVA_VERSION=jdk-15.0.2+7_openj9-0.24.0
# Sat, 03 Apr 2021 05:54:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b69a4bc87ed2e985d252cff02d53f1a11b8d83d39e0800cd4a1cab4521375314';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_aarch64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b2158268de0be247801b7823ee3e7f739254d77718a1879848627181feee2f4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_ppc64le_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='0f34a9dd2b800f669e004e543529e454c047a19919ec3b423552d171cb4f2626';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_s390x_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5515ccd79b1b5e8d8a615b80d5fe1272f7bb41100e46d94fb78ee611ea014816';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_x64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 05:54:43 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 05:54:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 03 Apr 2021 05:55:27 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 03 Apr 2021 05:55:31 GMT
CMD ["jshell"]
# Tue, 06 Apr 2021 22:42:33 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 06 Apr 2021 22:42:39 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Apr 2021 22:42:58 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 06 Apr 2021 22:43:04 GMT
WORKDIR /usr/local/tomcat
# Tue, 06 Apr 2021 22:43:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 22:43:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 22:43:20 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 06 Apr 2021 22:43:24 GMT
ENV TOMCAT_MAJOR=10
# Tue, 06 Apr 2021 22:43:27 GMT
ENV TOMCAT_VERSION=10.0.5
# Tue, 06 Apr 2021 22:43:31 GMT
ENV TOMCAT_SHA512=27271e17c8daf52503490c6657c992cc150cf2942e1b0179b738f34e9aa5e1aac3c7b947c67441d17294a8f1e772a00e38e30b2135372d6ee9d71207ac7261c3
# Tue, 06 Apr 2021 22:52:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Tue, 06 Apr 2021 22:52:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 06 Apr 2021 22:52:46 GMT
EXPOSE 8080
# Tue, 06 Apr 2021 22:52:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:aec64c5886d73bce6909d3e499c002da0a348e48c54730f8dd94fbb6811002db`  
		Last Modified: Fri, 02 Apr 2021 12:47:56 GMT  
		Size: 33.3 MB (33280041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a277bf183c930722f7e28d4f861e58debfeb1c7f985890be32cee394785d4d0`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7f599b30432860ae303a223c7b2b802cf41e3411db44b165b5db701e1d7aaa`  
		Last Modified: Sat, 03 Apr 2021 02:17:52 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3147f9d7021e4b4f874d531cd0d820bd489543f00c894d4d9df8f2c1b0777d2b`  
		Last Modified: Sat, 03 Apr 2021 06:01:07 GMT  
		Size: 17.2 MB (17208203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bb2d1bb51ebc4b823eeffa89def388ac717bab3451654c91b1cff1d5c9d02f`  
		Last Modified: Sat, 03 Apr 2021 06:07:08 GMT  
		Size: 198.1 MB (198071591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99548ce103dfd87f1e0c92d9421ec713cbf3d888d69a218e2f06b205dff2a04c`  
		Last Modified: Sat, 03 Apr 2021 06:06:46 GMT  
		Size: 4.4 MB (4439013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0676358f4953ea6c952c3daf3b5d4f0e0dd490e65a132c474161316b0d21613`  
		Last Modified: Wed, 07 Apr 2021 01:05:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed41ac2d61e8fdddf27fafed280d03dfbc07f399d87a9b62631b1a1f7d441792`  
		Last Modified: Wed, 07 Apr 2021 01:05:51 GMT  
		Size: 13.0 MB (13009703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520380346cba38b71522f96c348872879caa0ef14d1f86d3d52e51647cd2a5be`  
		Last Modified: Wed, 07 Apr 2021 01:05:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jdk15-adoptopenjdk-openj9` - linux; s390x

```console
$ docker pull tomcat@sha256:fbeed9fcb4a4677e205b0a289b3168bd1aacba755fade38228b90d5490e4cef8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.3 MB (256332021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e00b84b6c14d6c3b37cfc9ff795ce7d717b278446847f11dc1a29a11d5921e9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Sat, 03 Apr 2021 00:53:12 GMT
ADD file:f0f77d23ef3ed00b88007dfb57647c2043738698d025cf825203923097fc31e5 in / 
# Sat, 03 Apr 2021 00:53:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Sat, 03 Apr 2021 00:53:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Sat, 03 Apr 2021 00:53:15 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Sat, 03 Apr 2021 00:53:15 GMT
CMD ["/bin/bash"]
# Sat, 03 Apr 2021 01:17:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 03 Apr 2021 01:18:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 03 Apr 2021 01:23:19 GMT
ENV JAVA_VERSION=jdk-15.0.2+7_openj9-0.24.0
# Sat, 03 Apr 2021 01:23:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b69a4bc87ed2e985d252cff02d53f1a11b8d83d39e0800cd4a1cab4521375314';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_aarch64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='5b2158268de0be247801b7823ee3e7f739254d77718a1879848627181feee2f4';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_ppc64le_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        s390x)          ESUM='0f34a9dd2b800f669e004e543529e454c047a19919ec3b423552d171cb4f2626';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_s390x_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        amd64|x86_64)          ESUM='5515ccd79b1b5e8d8a615b80d5fe1272f7bb41100e46d94fb78ee611ea014816';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.2%2B7_openj9-0.24.0/OpenJDK15U-jdk_x64_linux_openj9_15.0.2_7_openj9-0.24.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 03 Apr 2021 01:23:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 03 Apr 2021 01:23:32 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 03 Apr 2021 01:24:05 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 03 Apr 2021 01:24:06 GMT
CMD ["jshell"]
# Tue, 06 Apr 2021 21:42:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 06 Apr 2021 21:42:53 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Apr 2021 21:42:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 06 Apr 2021 21:42:55 GMT
WORKDIR /usr/local/tomcat
# Tue, 06 Apr 2021 21:42:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 21:42:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 06 Apr 2021 21:42:57 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 06 Apr 2021 21:42:58 GMT
ENV TOMCAT_MAJOR=10
# Tue, 06 Apr 2021 21:42:59 GMT
ENV TOMCAT_VERSION=10.0.5
# Tue, 06 Apr 2021 21:42:59 GMT
ENV TOMCAT_SHA512=27271e17c8daf52503490c6657c992cc150cf2942e1b0179b738f34e9aa5e1aac3c7b947c67441d17294a8f1e772a00e38e30b2135372d6ee9d71207ac7261c3
# Tue, 06 Apr 2021 21:43:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg dirmngr 		wget ca-certificates 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local mvnFile="${1:-}"; 		local success=; 		local distUrl=; 		for distUrl in 			"https://www.apache.org/dyn/closer.cgi?action=download&filename=$distFile" 			"https://www-us.apache.org/dist/$distFile" 			"https://www.apache.org/dist/$distFile" 			"https://archive.apache.org/dist/$distFile" 			${mvnFile:+"https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/$mvnFile"} 		; do 			if wget -O "$f" "$distUrl" --progress=dot:giga && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'tomcat.tar.gz' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz"; 	echo "$TOMCAT_SHA512 *tomcat.tar.gz" | sha512sum --strict --check -; 	ddist 'tomcat.tar.gz.asc' "tomcat/tomcat-$TOMCAT_MAJOR/v$TOMCAT_VERSION/bin/apache-tomcat-$TOMCAT_VERSION.tar.gz.asc" "$TOMCAT_VERSION/tomcat-$TOMCAT_VERSION.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify tomcat.tar.gz.asc tomcat.tar.gz; 	tar -xf tomcat.tar.gz --strip-components=1; 	rm bin/*.bat; 	rm tomcat.tar.gz*; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME"; 		mv webapps webapps.dist; 	mkdir webapps; 		nativeBuildDir="$(mktemp -d)"; 	tar -xf bin/tomcat-native.tar.gz -C "$nativeBuildDir" --strip-components=1; 	apt-get install -y --no-install-recommends 		dpkg-dev 		gcc 		libapr1-dev 		libssl-dev 		make 	; 	( 		export CATALINA_HOME="$PWD"; 		cd "$nativeBuildDir/native"; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 		aprConfig="$(command -v apr-1-config)"; 		./configure 			--build="$gnuArch" 			--libdir="$TOMCAT_NATIVE_LIBDIR" 			--prefix="$CATALINA_HOME" 			--with-apr="$aprConfig" 			--with-java-home="$JAVA_HOME" 			--with-ssl=yes; 		make -j "$(nproc)"; 		make install; 	); 	rm -rf "$nativeBuildDir"; 	rm bin/tomcat-native.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find "$TOMCAT_NATIVE_LIBDIR" -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| xargs -rt readlink -e 		| sort -u 		| xargs -rt dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		find ./bin/ -name '*.sh' -exec sed -ri 's|^#!/bin/sh$|#!/usr/bin/env bash|' '{}' +; 		chmod -R +rX .; 	chmod 777 logs temp work; 		catalina.sh version
# Tue, 06 Apr 2021 21:44:03 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 06 Apr 2021 21:44:04 GMT
EXPOSE 8080
# Tue, 06 Apr 2021 21:44:05 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c667d3511750ec1ba4a5a25116565ac6f0c1e009e2af25deed3fd628b2d58447`  
		Last Modified: Fri, 02 Apr 2021 12:48:01 GMT  
		Size: 27.2 MB (27185749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b0e7f885536f559da072e429c3f0c0b4c52982c7b9ed4d76926cef7ec74c59`  
		Last Modified: Sat, 03 Apr 2021 00:54:01 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4c1ba7f00973d05cf601630fb8c201b1e42b2fc5df060a6810b6bd9ef309f9`  
		Last Modified: Sat, 03 Apr 2021 00:54:01 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acf01335898508ae34af2fef3754ef7741a902ffdf2faf6a2ca25a3f9cce476`  
		Last Modified: Sat, 03 Apr 2021 01:28:01 GMT  
		Size: 15.7 MB (15741335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f976cf78b4cfeee2eb20d6b7b32df3431e2d30c4a0c74ca21f498abcc06cc1a2`  
		Last Modified: Sat, 03 Apr 2021 01:31:45 GMT  
		Size: 195.1 MB (195121484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6a47cf4db3481e2066c4afbc735a9c81029d6fbcb048b4793fbeb903d785b`  
		Last Modified: Sat, 03 Apr 2021 01:31:31 GMT  
		Size: 5.3 MB (5328457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cfff31af71f4f48b0526c147a1e478661ff7a673e5d76ddc95c206e8379bee`  
		Last Modified: Tue, 06 Apr 2021 22:09:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e15ddb25b4629e59d4942bda8641a4ad880e9411a645be3da47cd0f050275f`  
		Last Modified: Tue, 06 Apr 2021 22:09:28 GMT  
		Size: 13.0 MB (12953606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee6cf726ddd17fc6d99ad34c6ed605d900235f646c609d359095e2514eb1f8f`  
		Last Modified: Tue, 06 Apr 2021 22:09:28 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
