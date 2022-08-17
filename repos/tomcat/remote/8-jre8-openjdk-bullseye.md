## `tomcat:8-jre8-openjdk-bullseye`

```console
$ docker pull tomcat@sha256:bf1e414022830500ccace4d77dcc29017f69756225d0f4ca1477f09e8a5ce131
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `tomcat:8-jre8-openjdk-bullseye` - linux; amd64

```console
$ docker pull tomcat@sha256:90f4ef07cdfbecacc567ba322d529d0b9de725b23b922479cdd3877c5b1bad82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129747838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af465ba245ae99d8baceff0dfddc26db863aaefe67c48adef1f1aa4a9e89782`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 05:53:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 05:55:37 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 02 Aug 2022 05:55:37 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 02 Aug 2022 05:55:37 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 05:55:38 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 05:55:38 GMT
ENV JAVA_VERSION=8u342
# Tue, 02 Aug 2022 05:55:44 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jre_x64_linux_8u342b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jre_aarch64_linux_8u342b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 03 Aug 2022 04:54:45 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 03 Aug 2022 04:54:45 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 04:54:45 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 03 Aug 2022 04:54:46 GMT
WORKDIR /usr/local/tomcat
# Wed, 03 Aug 2022 04:54:46 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 03 Aug 2022 04:54:46 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 03 Aug 2022 05:16:05 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 03 Aug 2022 05:16:05 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 21:36:09 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 21:36:09 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 21:36:10 GMT
COPY dir:3e3d9f260b98eb35415831d8f3de57d46140ed80fe3b53c1a53dfc13c5d3222b in /usr/local/tomcat 
# Wed, 17 Aug 2022 21:36:13 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Aug 2022 21:36:15 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 21:36:15 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 21:36:15 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8510da692cda60e4746c14dd90905695eade5888e2ad640706a2be9dc42a0224`  
		Last Modified: Tue, 02 Aug 2022 06:11:48 GMT  
		Size: 5.7 MB (5657904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34215579d03c1311f4e8cd3525bc03dbbb53d79d8b58e63cce8cdd355356347`  
		Last Modified: Tue, 02 Aug 2022 06:15:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d77b4774a96dfa09076212d5170e977d153ceab60c1ec4312a8f436b91371c`  
		Last Modified: Tue, 02 Aug 2022 06:15:07 GMT  
		Size: 41.4 MB (41423772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25be23b96412121e9e10fbdcadb75f26f550828dc6a1e57c9d731b1408ab18b`  
		Last Modified: Wed, 03 Aug 2022 05:39:11 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67060f7bbd3f2fe5b4791f4c9915ecad62a19f121f44f4a8b76b40cd367b2aa8`  
		Last Modified: Wed, 17 Aug 2022 21:57:42 GMT  
		Size: 11.2 MB (11173865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa62dee7e57d4e2ab1990867e7e11735933f05433cbed55e27ea3aa2c8577d`  
		Last Modified: Wed, 17 Aug 2022 21:57:41 GMT  
		Size: 459.7 KB (459711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d55e5af255c18ecce11733b9a094490c514cec4fdaaeaeea8c4be4ba738b705`  
		Last Modified: Wed, 17 Aug 2022 21:57:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre8-openjdk-bullseye` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:c2329555d41ce30ad201caff72af3b62ae8babce28a794c410a4655a94a57099
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127215901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e967ce9d7afa291020d1f3b92142f78686cbe5f4325ad3084da1fbc64679218`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 04:50:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 04:53:23 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 02 Aug 2022 04:53:24 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 02 Aug 2022 04:53:25 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 04:53:26 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 04:53:27 GMT
ENV JAVA_VERSION=8u342
# Tue, 02 Aug 2022 04:53:34 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jre_x64_linux_8u342b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jre_aarch64_linux_8u342b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Wed, 03 Aug 2022 02:00:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 03 Aug 2022 02:00:41 GMT
ENV PATH=/usr/local/tomcat/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 02:00:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 03 Aug 2022 02:00:43 GMT
WORKDIR /usr/local/tomcat
# Wed, 03 Aug 2022 02:00:44 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 03 Aug 2022 02:00:45 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 03 Aug 2022 02:34:30 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Wed, 03 Aug 2022 02:34:31 GMT
ENV TOMCAT_MAJOR=8
# Wed, 17 Aug 2022 22:11:16 GMT
ENV TOMCAT_VERSION=8.5.82
# Wed, 17 Aug 2022 22:11:17 GMT
ENV TOMCAT_SHA512=ba701002be9729e19b5d2e12e1f4a723a38ad4452ab235127a19397bc81e95adc060187501701ba0160f0017723525b506a42f0dbb4f9f91f1a1a53be1ba1b25
# Wed, 17 Aug 2022 22:11:19 GMT
COPY dir:39efdb2f05ae40d516e3c7e5c8281b88f71e133cff1e40cf875d1c806823546c in /usr/local/tomcat 
# Wed, 17 Aug 2022 22:11:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Aug 2022 22:11:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 17 Aug 2022 22:11:25 GMT
EXPOSE 8080
# Wed, 17 Aug 2022 22:11:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b7f28ea2855580a872ab6a4242d40e22c12ccc0312535acf914ece186b4562`  
		Last Modified: Tue, 02 Aug 2022 05:16:26 GMT  
		Size: 5.6 MB (5648824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae63f090f1cf677ac0a8b14766bdacaa3e3b598faae1e9b82b31f20a8dba394`  
		Last Modified: Tue, 02 Aug 2022 05:20:07 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2302b171bb2da8e12297bf60ac12b223b2f4c89251b0065ab36a194c109e35b`  
		Last Modified: Tue, 02 Aug 2022 05:20:12 GMT  
		Size: 40.7 MB (40673905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386d3e25cae34a0b03590874dc8025cd8a07479a31c69fcae413200e70f7212c`  
		Last Modified: Wed, 03 Aug 2022 03:08:13 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f55229ef25d7636fc629128af5d4fc304ab707bf0bcca6ff036a98856f96217`  
		Last Modified: Wed, 17 Aug 2022 22:53:01 GMT  
		Size: 11.2 MB (11186259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68f60de5eeb5812fe26e0ef2bbc695b8fcb587f7ca074b4deff2396fc5a4a81`  
		Last Modified: Wed, 17 Aug 2022 22:52:46 GMT  
		Size: 217.2 KB (217163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
