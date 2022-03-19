## `tomcat:10-jre8-openjdk-slim-buster`

```console
$ docker pull tomcat@sha256:745224eff40c1caa76faa522839bd9c22084f3e9ae624c49eed51932484c03c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jre8-openjdk-slim-buster` - linux; amd64

```console
$ docker pull tomcat@sha256:677376c8ca378aea5d0a66f48748af674ae0d9f8f2e93e24c564c197558d93db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85020801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6439bb618a744fbb0fd6377c4c131a2c1be7b6d72e9295ca2626dd47cee835d9`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:26 GMT
ADD file:7f5787c324936e09d339f9426eec4a0120431e2a4b6ccb0db28b94d61f074ab2 in / 
# Thu, 17 Mar 2022 04:04:27 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:16:51 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 17 Mar 2022 18:16:52 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 17 Mar 2022 18:16:52 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:16:52 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 18:16:52 GMT
ENV JAVA_VERSION=8u322
# Thu, 17 Mar 2022 18:19:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 18 Mar 2022 22:42:01 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 18 Mar 2022 22:42:01 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 22:42:01 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 18 Mar 2022 22:42:02 GMT
WORKDIR /usr/local/tomcat
# Fri, 18 Mar 2022 22:42:02 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 18 Mar 2022 22:42:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 18 Mar 2022 22:42:02 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Fri, 18 Mar 2022 22:42:02 GMT
ENV TOMCAT_MAJOR=10
# Fri, 18 Mar 2022 22:42:02 GMT
ENV TOMCAT_VERSION=10.0.18
# Fri, 18 Mar 2022 22:42:02 GMT
ENV TOMCAT_SHA512=a9e3c516676369bd9d52e768071898b0e07659a9ff03b9dc491e53f084b9981a929bf2c74a694f06ad26dae0644fb9617cc6e364f0e1dcd953c857978a95a644
# Fri, 18 Mar 2022 22:42:03 GMT
COPY dir:89f3457a8b3d0c84e8e696147e9518559d5e2e874e44b34f8b982be9648e767e in /usr/local/tomcat 
# Fri, 18 Mar 2022 22:42:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 22:42:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 18 Mar 2022 22:42:09 GMT
EXPOSE 8080
# Fri, 18 Mar 2022 22:42:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:a4b007099961706d45bdb3eb0a3aab719916c3e36d6da7577b0c9060260e65f8`  
		Last Modified: Thu, 17 Mar 2022 04:10:54 GMT  
		Size: 27.2 MB (27153828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d899da7a457921f26453d8b8d7627f92345b2d4e0148e596703edd05fff65e`  
		Last Modified: Thu, 17 Mar 2022 18:25:35 GMT  
		Size: 3.3 MB (3269586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433a4a4746210b0477d3fe9848e12cdbefc758bfcd7c6a251048893017aa2f41`  
		Last Modified: Thu, 17 Mar 2022 18:35:11 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db33ba88a3314fa4fdfb8ea50da1e13a7dfd80b55acab5d7a9b86e0966a164a`  
		Last Modified: Thu, 17 Mar 2022 18:36:06 GMT  
		Size: 41.7 MB (41672165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87aa3dfd9b23dafde8d1a2e75ada00c7891ef9fea097f53ec23beeed7f90615f`  
		Last Modified: Fri, 18 Mar 2022 23:12:21 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb78acd9a4a4505d94b0c925c9d587eaf8679a11e7be55f17c0b1684b7e2093`  
		Last Modified: Fri, 18 Mar 2022 23:12:22 GMT  
		Size: 12.5 MB (12536997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d9c73d53c2630e65d5d385f99f041eea40cabf4efecf93884730e1dc7f104f`  
		Last Modified: Fri, 18 Mar 2022 23:12:21 GMT  
		Size: 387.7 KB (387709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a6f9783beaf2bb8f4c3437028358b2490e87e33e7517dbf16f2be52c70d484`  
		Last Modified: Fri, 18 Mar 2022 23:12:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-openjdk-slim-buster` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:470880dfbdb58af13b5eec6117fbcf0bf5494ffadb5a5ebbb6ed46b729b9e427
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.5 MB (82483668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9341f86b401a2bee3f6abc9759b91d8d3433b934e76c731bbf0db94bc767cce`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:22 GMT
ADD file:1c7d8cedf5dc79c676acebde5252ecd3005088a9f29e5e6be547f659f41efb1f in / 
# Thu, 17 Mar 2022 03:22:22 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 23:23:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 23:35:48 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 17 Mar 2022 23:35:49 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 17 Mar 2022 23:35:50 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 23:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 23:35:52 GMT
ENV JAVA_VERSION=8u322
# Thu, 17 Mar 2022 23:38:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Sat, 19 Mar 2022 11:34:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 19 Mar 2022 11:34:08 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 11:34:09 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 19 Mar 2022 11:34:10 GMT
WORKDIR /usr/local/tomcat
# Sat, 19 Mar 2022 11:34:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 19 Mar 2022 11:34:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 19 Mar 2022 11:34:13 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Sat, 19 Mar 2022 11:34:14 GMT
ENV TOMCAT_MAJOR=10
# Sat, 19 Mar 2022 11:34:15 GMT
ENV TOMCAT_VERSION=10.0.18
# Sat, 19 Mar 2022 11:34:16 GMT
ENV TOMCAT_SHA512=a9e3c516676369bd9d52e768071898b0e07659a9ff03b9dc491e53f084b9981a929bf2c74a694f06ad26dae0644fb9617cc6e364f0e1dcd953c857978a95a644
# Sat, 19 Mar 2022 11:34:18 GMT
COPY dir:cbfe3c748b5aa04ab3f895e8e0103ab5141bedec56908a5288cff0b2e51bdb14 in /usr/local/tomcat 
# Sat, 19 Mar 2022 11:34:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 11:34:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 19 Mar 2022 11:34:24 GMT
EXPOSE 8080
# Sat, 19 Mar 2022 11:34:25 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:c9277cac12165646c33f028489f2a5be3f70745382f4385cd9ed12fcc8cec183`  
		Last Modified: Thu, 17 Mar 2022 03:29:27 GMT  
		Size: 25.9 MB (25923233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae7314079173e0b84736e3e2bd8ab0ecb4a61a7e8edf7f35305c0176b6d73a7`  
		Last Modified: Thu, 17 Mar 2022 23:48:51 GMT  
		Size: 3.1 MB (3118894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab252bc0c3a5e2c37e8345f9745d882134b72b71f62dd374cd3be03c1a56efb4`  
		Last Modified: Fri, 18 Mar 2022 00:02:47 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc1ec2675f9ed5c32927637f2b44970a919c438f0ba05f46892d7ef567d120b`  
		Last Modified: Fri, 18 Mar 2022 00:04:14 GMT  
		Size: 40.7 MB (40716733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f273a0f06be3375957ad63dbd4471d3b80cccf17c999f6d047868249b0d337`  
		Last Modified: Sat, 19 Mar 2022 12:40:50 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a45bb9615d2950c0c929d4e03f0b4185b804f6b4d39c8a7c4cad7120f6c2763`  
		Last Modified: Sat, 19 Mar 2022 12:40:51 GMT  
		Size: 12.6 MB (12550837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d164a920045b0ae80ff9e036f4bce1472b37d2b9174268f49c8d5c91a6bd7899`  
		Last Modified: Sat, 19 Mar 2022 12:40:50 GMT  
		Size: 173.6 KB (173620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
