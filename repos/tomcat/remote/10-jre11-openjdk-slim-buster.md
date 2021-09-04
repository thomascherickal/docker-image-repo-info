## `tomcat:10-jre11-openjdk-slim-buster`

```console
$ docker pull tomcat@sha256:1623eeca24f0647b0dc07ce2da75b1fc8129ef96d991c32875c3e33677e60094
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jre11-openjdk-slim-buster` - linux; amd64

```console
$ docker pull tomcat@sha256:4648380ce425ec99f0d0f8a11c17d15b1b527a47418d17d94d2ef1709e637a92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.4 MB (90446265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d10d09834a825242665874bfd2c1108573263179371bf67fa0dbcccbf467e1c7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:32:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:38:42 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 03 Sep 2021 08:38:43 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 08:38:43 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:38:44 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:38:44 GMT
ENV JAVA_VERSION=11.0.12
# Fri, 03 Sep 2021 08:41:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Sat, 04 Sep 2021 13:16:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 04 Sep 2021 13:16:56 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Sep 2021 13:16:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 04 Sep 2021 13:16:57 GMT
WORKDIR /usr/local/tomcat
# Sat, 04 Sep 2021 13:16:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 04 Sep 2021 13:16:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 04 Sep 2021 13:16:58 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Sat, 04 Sep 2021 13:16:58 GMT
ENV TOMCAT_MAJOR=10
# Sat, 04 Sep 2021 13:22:40 GMT
ENV TOMCAT_VERSION=10.0.10
# Sat, 04 Sep 2021 13:22:40 GMT
ENV TOMCAT_SHA512=3f6d5d292ab67348b3134c1013044c948caf5a4bf142b4e856b5ee63693a6e80994b0b4dbb3404d0fd3542fd6f7f52b4cbe404fc5a0f716ac98d68db879b7112
# Sat, 04 Sep 2021 13:22:41 GMT
COPY dir:bbcaa09fa6b9829c667dc9930a557e5b7b843ec256a81c6ca33808ae036b1848 in /usr/local/tomcat 
# Sat, 04 Sep 2021 13:22:45 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 13:22:46 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 04 Sep 2021 13:22:46 GMT
EXPOSE 8080
# Sat, 04 Sep 2021 13:22:47 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb538b78785f115f86e312f41ac522a9b30e0cb77d061dd273f331e57ae2e471`  
		Last Modified: Fri, 03 Sep 2021 08:50:36 GMT  
		Size: 3.3 MB (3269611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02563c39821201d7d9a1958c1e1b5cc2bdbc768a7cee6122187f5298bc5a05`  
		Last Modified: Fri, 03 Sep 2021 09:03:00 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3b22ab301ebe7f2976a31dd7b841826a54610438efa12f777125a3ae428f10`  
		Last Modified: Fri, 03 Sep 2021 09:05:07 GMT  
		Size: 47.1 MB (47137179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4fa09b64329180340636ce465e91cd4ed60c0cd584b5af72c599f77bf72514`  
		Last Modified: Sat, 04 Sep 2021 13:58:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fd4a995218077702a758ef9d4f61e6fe3e3f36256d5576d3a4a399565456d3`  
		Last Modified: Sat, 04 Sep 2021 14:03:47 GMT  
		Size: 12.5 MB (12505385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a479c5418903e74e156e6053a28c3a19eeb2ddc37daf866094ba7296cac2d807`  
		Last Modified: Sat, 04 Sep 2021 14:03:46 GMT  
		Size: 387.7 KB (387737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ab96382d9d947ef1e53f955717359406723143e2d39825df379de39889bac0`  
		Last Modified: Sat, 04 Sep 2021 14:03:46 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre11-openjdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:d5ec764b4f69c952076afd3544486674612e6be932cf9424effa150a76fadfa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88143948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048ed4de26dc0b95df7c8756be95d195ff4610b094aa41f54393310f6fae96d4`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 10:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:51:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 03 Sep 2021 10:51:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 10:51:07 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 10:51:07 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 10:51:07 GMT
ENV JAVA_VERSION=11.0.12
# Fri, 03 Sep 2021 10:52:55 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Sat, 04 Sep 2021 03:28:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 04 Sep 2021 03:28:24 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Sep 2021 03:28:25 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 04 Sep 2021 03:28:25 GMT
WORKDIR /usr/local/tomcat
# Sat, 04 Sep 2021 03:28:25 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 04 Sep 2021 03:28:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 04 Sep 2021 03:28:26 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Sat, 04 Sep 2021 03:28:26 GMT
ENV TOMCAT_MAJOR=10
# Sat, 04 Sep 2021 03:34:55 GMT
ENV TOMCAT_VERSION=10.0.10
# Sat, 04 Sep 2021 03:34:55 GMT
ENV TOMCAT_SHA512=3f6d5d292ab67348b3134c1013044c948caf5a4bf142b4e856b5ee63693a6e80994b0b4dbb3404d0fd3542fd6f7f52b4cbe404fc5a0f716ac98d68db879b7112
# Sat, 04 Sep 2021 03:34:55 GMT
COPY dir:7b5f10df291c3372a133e7ac03a3d9f75faa31ce64b1fe822d2ab46a9519c550 in /usr/local/tomcat 
# Sat, 04 Sep 2021 03:34:59 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 03:35:01 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 04 Sep 2021 03:35:01 GMT
EXPOSE 8080
# Sat, 04 Sep 2021 03:35:01 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4152925219b6247cb64144905f215af10ba4621b4f699e896b93191fc575742`  
		Last Modified: Fri, 03 Sep 2021 11:06:36 GMT  
		Size: 3.1 MB (3119119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae4172c359f34fa7cfb5057007160bb64e7fb759428f2ec689c0f1b778186c`  
		Last Modified: Fri, 03 Sep 2021 11:16:10 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce379fd28d96fc884d8aedd847223177a12874244ac215bc1464d0ef08b602a`  
		Last Modified: Fri, 03 Sep 2021 11:18:17 GMT  
		Size: 46.2 MB (46203489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6747f60ed0aec166092eba459fcf8215d70619bfaf3159046bfc6c9dd95a75`  
		Last Modified: Sat, 04 Sep 2021 04:25:44 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab02791d75e2d98d0604b18ee763f2331aafb4d388e1fd17b94845c572e80a4`  
		Last Modified: Sat, 04 Sep 2021 04:32:15 GMT  
		Size: 12.5 MB (12519775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cee9412ee4b1436bb02ef745e44ebcc67dc77a5e5a3293a2e3d6f1100615850`  
		Last Modified: Sat, 04 Sep 2021 04:32:14 GMT  
		Size: 386.2 KB (386195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16204874ab9a4db02f71b31535d9dfcd6686cdb9925854b82902d143bca4b000`  
		Last Modified: Sat, 04 Sep 2021 04:32:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
