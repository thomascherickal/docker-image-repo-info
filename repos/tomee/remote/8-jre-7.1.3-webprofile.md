## `tomee:8-jre-7.1.3-webprofile`

```console
$ docker pull tomee@sha256:31686b0ba0d4d36c7582669441a25f40bc541f472711128e0f0f0b59c3cbeaeb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `tomee:8-jre-7.1.3-webprofile` - linux; amd64

```console
$ docker pull tomee@sha256:626fcf681f453346157c848ead8b6eaff8e0cbe206e69693b9010cb596c18420
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154586504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaba142984d32ee7d27dbe9262aca03ad3d7edb3a80dd27a091b2e9cb79321ba`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:16 GMT
ADD file:89dfd7d3ed77fd5e05f20a0ab631142207ae462f5bbd877f8745d3930c751d87 in / 
# Wed, 22 Jul 2020 02:03:16 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:00:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 03:00:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 22 Jul 2020 22:41:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 22:41:09 GMT
ENV LANG=C.UTF-8
# Wed, 22 Jul 2020 22:42:21 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 22 Jul 2020 22:42:22 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 22:42:22 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Thu, 30 Jul 2020 22:26:51 GMT
ENV JAVA_VERSION=8u265
# Thu, 30 Jul 2020 22:26:56 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) downloadUrl=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u265-b01/OpenJDK8U-jre_x64_linux_8u265b01.tar.gz ;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz.asc "$downloadUrl.sign"; 	wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 31 Jul 2020 00:21:48 GMT
ENV PATH=/usr/local/tomee/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Jul 2020 00:21:49 GMT
RUN mkdir -p /usr/local/tomee
# Fri, 31 Jul 2020 00:21:50 GMT
WORKDIR /usr/local/tomee
# Fri, 31 Jul 2020 00:21:50 GMT
ENV GPG_KEYS=223D3A74B068ECA354DC385CE126833F9CF64915     7A2744A8A9AAF063C23EB7868EBE7DBE8D050EEF     82D8419BA697F0E7FB85916EE91287822FDB81B1     9056B710F1E332780DE7AF34CBAEBE39A46C4CA1     A57DAF81C1B69921F4BA8723A8DE0A4DB863A7C1     B7574789F5018690043E6DD9C212662E12F3E1DD     B8B301E6105DF628076BD92C5483E55897ABD9B9     DBCCD103B8B24F86FFAAB025C8BB472CD297D428     F067B8140F5DD80E1D3B5D92318242FE9A0B1183     FAA603D58B1BA4EDF65896D0ED340E0E6D545F97     C92604B0DEC5C62CFF5801E73D4683C24EDC64D1     294A395FFDC9FCF25A7E2BFDCF6FC99C2CC77782
# Fri, 31 Jul 2020 00:21:51 GMT
RUN set -xe     && for key in $GPG_KEYS; do         gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||         gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done
# Fri, 31 Jul 2020 00:22:18 GMT
ENV TOMEE_VER=7.1.3
# Fri, 31 Jul 2020 00:22:46 GMT
ENV TOMEE_BUILD=webprofile
# Fri, 31 Jul 2020 00:22:49 GMT
RUN set -x 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz.asc -o tomee.tar.gz.asc 	&& curl -fSL https://dist.apache.org/repos/dist/release/tomee/tomee-${TOMEE_VER}/apache-tomee-${TOMEE_VER}-${TOMEE_BUILD}.tar.gz -o tomee.tar.gz 	&& gpg --batch --verify tomee.tar.gz.asc tomee.tar.gz 	&& tar -zxf tomee.tar.gz 	&& mv apache-tomee-${TOMEE_BUILD}-${TOMEE_VER}/* /usr/local/tomee 	&& rm -Rf apache-tomee-${TOMEE_BUILD}-${TOMEE_VER} 	&& rm bin/*.bat 	&& rm tomee.tar.gz*
# Fri, 31 Jul 2020 00:22:49 GMT
EXPOSE 8080
# Fri, 31 Jul 2020 00:22:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:31dd5ebca5efc5e96a425402fa85e492b02c8fe757dfd3edfdea2a7c67322909`  
		Last Modified: Wed, 22 Jul 2020 02:09:37 GMT  
		Size: 50.4 MB (50390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed641c4ae9821ca3c399071ea82ae667237acbcaad1e367c3e1e87fc967834c`  
		Last Modified: Wed, 22 Jul 2020 03:16:28 GMT  
		Size: 7.8 MB (7811702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd57146431eae70720cf24877e818256ae1a30b9c1c9e7d0ad093c945ca0af2`  
		Last Modified: Wed, 22 Jul 2020 03:16:28 GMT  
		Size: 10.0 MB (9996319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49dd46492913ebc75f7ee834a77d90bb0ebf30d78f3aff2a2f2018ad7299f81`  
		Last Modified: Wed, 22 Jul 2020 22:47:55 GMT  
		Size: 5.5 MB (5529328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6034d6cdb9bd996e89db23fa6b5e5b3f7a1369a34619c509cd721a7e7d1b66f`  
		Last Modified: Wed, 22 Jul 2020 22:48:58 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc372dc79b70611a5cb2f84ba32b5470e7b8f7b9bb1d4eb56b9ac961e2ebd0ec`  
		Last Modified: Thu, 30 Jul 2020 22:29:49 GMT  
		Size: 40.3 MB (40334763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b231acc980d85b6a8de11df80d4f11925403631f30bc7f6d45c43b73c6d29c21`  
		Last Modified: Fri, 31 Jul 2020 00:24:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce6f1380b9ad4653c902b73f56e2aef4e2c380ce9ec006d4f75ed9c1ebbb556`  
		Last Modified: Fri, 31 Jul 2020 00:24:17 GMT  
		Size: 20.9 KB (20935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4c22c52aaf42c86b3567b1506f01026a2d6c51f2d27a71978f309c9cba0b43`  
		Last Modified: Fri, 31 Jul 2020 00:25:21 GMT  
		Size: 40.5 MB (40502782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
