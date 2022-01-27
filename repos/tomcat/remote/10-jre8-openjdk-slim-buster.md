## `tomcat:10-jre8-openjdk-slim-buster`

```console
$ docker pull tomcat@sha256:6473b5af1a85ee10279600b2b67cb76e868f0cac6ab6145d0f4874559258b820
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jre8-openjdk-slim-buster` - linux; amd64

```console
$ docker pull tomcat@sha256:35756b58c5410b805804c9d782b6f1fceb49e3c337f72c886957db219f611cdb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85006092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20c7d373e104aeaf6ae761a05b54b24eb0179a5892abd451e45ccb531024c69e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 22:58:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:06:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 23:06:59 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 23:06:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:06:59 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 23:07:00 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 23:08:48 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 22 Dec 2021 17:13:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 22 Dec 2021 17:13:27 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 17:13:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 22 Dec 2021 17:13:28 GMT
WORKDIR /usr/local/tomcat
# Wed, 22 Dec 2021 17:13:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:13:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 22 Dec 2021 17:13:28 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 22 Dec 2021 17:13:28 GMT
ENV TOMCAT_MAJOR=10
# Fri, 21 Jan 2022 01:53:48 GMT
ENV TOMCAT_VERSION=10.0.16
# Fri, 21 Jan 2022 01:53:48 GMT
ENV TOMCAT_SHA512=9b70f4db2c7b2efb5453cd581322b1137df7b6443acd6a8e278eaaf97de89c9ad0c7c7996a2d545ef1e4d965aca43c40d2b2c7d5e46b021695f87093143fbba2
# Fri, 21 Jan 2022 01:53:48 GMT
COPY dir:cbe5b093fafa4a0f2af9e5b3993def907d950fae2e619626098080aef0a62e88 in /usr/local/tomcat 
# Fri, 21 Jan 2022 01:53:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 21 Jan 2022 01:53:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 21 Jan 2022 01:53:55 GMT
EXPOSE 8080
# Fri, 21 Jan 2022 01:53:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c983bcc370920d99695dc288c345343be841987206e4ce762a4e7599f28c96`  
		Last Modified: Tue, 21 Dec 2021 23:16:09 GMT  
		Size: 3.3 MB (3269567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffc6ac20cd8533d7d04760fd209378d44e47146260329ef2f2a99b5bd2dc165`  
		Last Modified: Tue, 21 Dec 2021 23:29:09 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877da5312739a7da73a607d597b79307039a80cbe36fcddc2482dffb0d437689`  
		Last Modified: Tue, 21 Dec 2021 23:30:31 GMT  
		Size: 41.6 MB (41647367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff443db5a545714ff5e0d2d8095ed80c86bcfe1a538ebaae942af8c02dc05b8`  
		Last Modified: Wed, 22 Dec 2021 17:55:14 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad45ecda95959c476ce87dd4221d3cb0c4f3eb9d5a700600e48c4df1f6d4410`  
		Last Modified: Fri, 21 Jan 2022 02:56:59 GMT  
		Size: 12.5 MB (12547228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf69f5f2d866f292f15e2c44c6f6d6e681b8c6fea93eaa53ed30038e5c9b232`  
		Last Modified: Fri, 21 Jan 2022 02:56:58 GMT  
		Size: 387.7 KB (387692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52dea873dfdc02ac0129f28c709b46e336c9280a3e0811d82eae5c422ac5af`  
		Last Modified: Fri, 21 Jan 2022 02:56:58 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-openjdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:31ee8095388ce1df4d93935f391527678be03c2ae48e8a527ac5003254ddfc21
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82468734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e94382d18ce168bccbe8630c384f8042b18de27b6db7a965174f947a937bf2f`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:51:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:02:36 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 26 Jan 2022 06:02:37 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 26 Jan 2022 06:02:38 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 06:02:39 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 06:02:40 GMT
ENV JAVA_VERSION=8u312
# Wed, 26 Jan 2022 06:04:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jre_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 27 Jan 2022 00:03:10 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 27 Jan 2022 00:03:11 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Jan 2022 00:03:12 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 27 Jan 2022 00:03:13 GMT
WORKDIR /usr/local/tomcat
# Thu, 27 Jan 2022 00:03:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 27 Jan 2022 00:03:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 27 Jan 2022 00:03:16 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 27 Jan 2022 00:03:17 GMT
ENV TOMCAT_MAJOR=10
# Thu, 27 Jan 2022 00:03:18 GMT
ENV TOMCAT_VERSION=10.0.16
# Thu, 27 Jan 2022 00:03:19 GMT
ENV TOMCAT_SHA512=9b70f4db2c7b2efb5453cd581322b1137df7b6443acd6a8e278eaaf97de89c9ad0c7c7996a2d545ef1e4d965aca43c40d2b2c7d5e46b021695f87093143fbba2
# Thu, 27 Jan 2022 00:03:21 GMT
COPY dir:1b569f88061ecb1decc40f4440c0b42bfa54edfd0d124d4ff4fb78102b4def5f in /usr/local/tomcat 
# Thu, 27 Jan 2022 00:03:24 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 00:03:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 27 Jan 2022 00:03:27 GMT
EXPOSE 8080
# Thu, 27 Jan 2022 00:03:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a5c9716b24a17043a5d8ede1303daffeaaa07ff0393fa14caed54f01154833`  
		Last Modified: Wed, 26 Jan 2022 06:14:50 GMT  
		Size: 3.1 MB (3118858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ebebc6e46bda1524e70a5c09062ee822fc4aa6a41486a93ff9832c99c8fa14`  
		Last Modified: Wed, 26 Jan 2022 06:29:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0ce182e48e767de24a86ca33bbc9f8a7cca68edb46bf324b0363308a332db6`  
		Last Modified: Wed, 26 Jan 2022 06:31:22 GMT  
		Size: 40.7 MB (40692324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d848811b4f44bee513a1bff78dffa0de302ef88aa031fe9a359c2f0dc1814`  
		Last Modified: Thu, 27 Jan 2022 01:02:10 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789c91dd472d6ab65abcfcaef4fb62f0d527bf4b2a46c891341bfa7d91e51088`  
		Last Modified: Thu, 27 Jan 2022 01:02:11 GMT  
		Size: 12.6 MB (12560381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8fa464cb64c78cacfaa6b16b69d34a67cbe7230593e412fc465ca5db305831`  
		Last Modified: Thu, 27 Jan 2022 01:02:10 GMT  
		Size: 173.6 KB (173605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
