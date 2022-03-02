## `tomcat:10-jre8-openjdk-buster`

```console
$ docker pull tomcat@sha256:abc4ca1b6425eb0e392c82dc900bca3168cce2e5fc8c7a7a26f39623ba301c72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:10-jre8-openjdk-buster` - linux; amd64

```console
$ docker pull tomcat@sha256:c70a4077d6603bdfd349fb23aa53768d640d938503895759aed5e9f425b90dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128193522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb9bd3c9d651c5afc9ef7145140c69cbce138a6db3366fa602f98b003919523`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:41 GMT
ADD file:e8b516b464e535b435a6ed8609bac98acc90ee30e2a0667f68932f0d924f6e49 in / 
# Tue, 01 Mar 2022 02:13:42 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:28:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 14:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:34:27 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 01 Mar 2022 14:34:28 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 01 Mar 2022 14:34:28 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 14:34:28 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:34:28 GMT
ENV JAVA_VERSION=8u322
# Tue, 01 Mar 2022 14:34:34 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 02 Mar 2022 11:12:41 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 02 Mar 2022 11:12:41 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 11:12:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 02 Mar 2022 11:12:42 GMT
WORKDIR /usr/local/tomcat
# Wed, 02 Mar 2022 11:12:42 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 02 Mar 2022 11:12:42 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 02 Mar 2022 11:12:42 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 02 Mar 2022 11:12:42 GMT
ENV TOMCAT_MAJOR=10
# Wed, 02 Mar 2022 11:12:43 GMT
ENV TOMCAT_VERSION=10.0.17
# Wed, 02 Mar 2022 11:12:43 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Wed, 02 Mar 2022 11:12:43 GMT
COPY dir:78f38d98312ca3aabd651c6efa483f03a287817b66124dfc5bff9e99655cde35 in /usr/local/tomcat 
# Wed, 02 Mar 2022 11:12:47 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 11:12:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 02 Mar 2022 11:12:49 GMT
EXPOSE 8080
# Wed, 02 Mar 2022 11:12:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1c9a8b42b5780ac49c71f392c9512c0167ecc23de9b30b1b5f38747b73097d1a`  
		Last Modified: Tue, 01 Mar 2022 02:19:43 GMT  
		Size: 50.4 MB (50437046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163066942b43a00ba7f4674c4c1ca90eccc8d99366a3dc47cb64e06ad79c36e5`  
		Last Modified: Tue, 01 Mar 2022 06:37:36 GMT  
		Size: 7.8 MB (7834052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf70e03a8272d87e65c7b1592f97f6e739cf1f5d13cc536670f41c28b086b4cb`  
		Last Modified: Tue, 01 Mar 2022 06:37:37 GMT  
		Size: 10.0 MB (9997298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0aebff17902b5ae62c7128c8a267d2e6000eccb66e0ba4b6ea1033eb5d2a3`  
		Last Modified: Tue, 01 Mar 2022 14:53:28 GMT  
		Size: 5.5 MB (5532021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c64b6508806fe3b66717b7b5aa79a958648317b2967b528f492f335f95e77d2`  
		Last Modified: Tue, 01 Mar 2022 14:56:47 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ea8df420a28fb3612f5cc6098356be9e1476ccf00ca90535c4a22aebd69669`  
		Last Modified: Tue, 01 Mar 2022 14:56:52 GMT  
		Size: 41.4 MB (41395159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96947ecbb735430c663c6412adc2e710176ec965358ab52405e00629259bc0cc`  
		Last Modified: Wed, 02 Mar 2022 12:00:50 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7467003eb0ccd6606f84ccf78b8b6b336ec6a08605d7e10f9b502415956cab74`  
		Last Modified: Wed, 02 Mar 2022 12:00:51 GMT  
		Size: 12.5 MB (12536502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2339f4a961c972a557b27f8ae3c715a36c45a93ba8c0d02a6ebca5ce10a472c4`  
		Last Modified: Wed, 02 Mar 2022 12:00:50 GMT  
		Size: 460.9 KB (460933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85eeda14debd8f993fc925a885fed675d5d6f03023030a06590c65b9c240e705`  
		Last Modified: Wed, 02 Mar 2022 12:00:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-openjdk-buster` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:06f685423fbad4fb031d2d948c40fe25382b9eb0d7818c2e134a10bd41659931
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125619572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05c05359749d7c0ba6503e134e09b129c0f75dd2061b4a69e2dad73c5ee2e8e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:41 GMT
ADD file:ec3d90624857dbfae217c1372a38966f453fcd51282379652f07d2ccf6fcc67e in / 
# Tue, 01 Mar 2022 02:11:42 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:35:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 13:59:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 14:03:33 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 01 Mar 2022 14:03:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 01 Mar 2022 14:03:35 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 14:03:36 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 14:03:37 GMT
ENV JAVA_VERSION=8u322
# Tue, 01 Mar 2022 14:03:52 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 02 Mar 2022 00:40:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 02 Mar 2022 00:40:52 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 00:40:53 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 02 Mar 2022 00:40:54 GMT
WORKDIR /usr/local/tomcat
# Wed, 02 Mar 2022 00:40:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 02 Mar 2022 00:40:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 02 Mar 2022 00:40:57 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 02 Mar 2022 00:40:58 GMT
ENV TOMCAT_MAJOR=10
# Wed, 02 Mar 2022 00:40:59 GMT
ENV TOMCAT_VERSION=10.0.17
# Wed, 02 Mar 2022 00:41:00 GMT
ENV TOMCAT_SHA512=c9a8894ddedb9a4966abb8698a029c00dda2603acb798bbf11a99cf585c2e5db967bee006689ea148b819fa11d1d8fe1e799ceb09243e70b1310ca18ada1f17f
# Wed, 02 Mar 2022 00:41:02 GMT
COPY dir:ed031019a6ebfaf2c2ebbf925a412ae339b32c13892957906fd3b04ec8693dbb in /usr/local/tomcat 
# Wed, 02 Mar 2022 00:41:05 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 00:41:07 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 02 Mar 2022 00:41:08 GMT
EXPOSE 8080
# Wed, 02 Mar 2022 00:41:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:72f0eb753e825356fa0fef854ac259cc8eefdb0f689516f29b13da8b1595c342`  
		Last Modified: Tue, 01 Mar 2022 02:18:46 GMT  
		Size: 49.2 MB (49223022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93053a54416be8288cbcc300d0a929f1279cceff9eb11ad9c080fe5439d62dbd`  
		Last Modified: Tue, 01 Mar 2022 10:45:39 GMT  
		Size: 7.7 MB (7695236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2387f0e2dcc6f4271b34d3158d1768015e4424839f06ae428f4e22de8a5c1542`  
		Last Modified: Tue, 01 Mar 2022 10:45:40 GMT  
		Size: 9.8 MB (9767253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fd7cb2a892d9067394a0609355afafe5337c3293a821ecfc941c3b47dc3507`  
		Last Modified: Tue, 01 Mar 2022 14:26:20 GMT  
		Size: 5.5 MB (5505844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570854edc867997edb34fcd6d6f35138c5944bdf2f411fa7fcc7ebf0e687faaf`  
		Last Modified: Tue, 01 Mar 2022 14:30:04 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7bc8e0c6e5caa8e24d82a71d75976cda605cda6ba715f4e3ff1c662562d563`  
		Last Modified: Tue, 01 Mar 2022 14:30:09 GMT  
		Size: 40.7 MB (40659886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6901fd900f7003c6e580aa1e512d5723573eeb8e71da71fd1b3fc98d904b6d1`  
		Last Modified: Wed, 02 Mar 2022 01:49:58 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969093f06c77814b825c0558f28980f5b3da5e452826e5da61f45492dd3f1576`  
		Last Modified: Wed, 02 Mar 2022 01:50:00 GMT  
		Size: 12.5 MB (12549766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46301eba850966aa7b7f5c9ac82d93944bc69d016ed2b8f5587f984d7956cd8`  
		Last Modified: Wed, 02 Mar 2022 01:49:59 GMT  
		Size: 218.2 KB (218218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
