<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `jetty`

-	[`jetty:10.0.6`](#jetty1006)
-	[`jetty:10.0.6-jdk11`](#jetty1006-jdk11)
-	[`jetty:10.0.6-jdk11-slim`](#jetty1006-jdk11-slim)
-	[`jetty:10.0.6-jdk16`](#jetty1006-jdk16)
-	[`jetty:10.0.6-jdk16-slim`](#jetty1006-jdk16-slim)
-	[`jetty:10.0.6-jre11`](#jetty1006-jre11)
-	[`jetty:10.0.6-jre11-slim`](#jetty1006-jre11-slim)
-	[`jetty:11.0.6`](#jetty1106)
-	[`jetty:11.0.6-jdk11`](#jetty1106-jdk11)
-	[`jetty:11.0.6-jdk11-slim`](#jetty1106-jdk11-slim)
-	[`jetty:11.0.6-jdk16`](#jetty1106-jdk16)
-	[`jetty:11.0.6-jdk16-slim`](#jetty1106-jdk16-slim)
-	[`jetty:11.0.6-jre11`](#jetty1106-jre11)
-	[`jetty:11.0.6-jre11-slim`](#jetty1106-jre11-slim)
-	[`jetty:9`](#jetty9)
-	[`jetty:9-jdk11`](#jetty9-jdk11)
-	[`jetty:9-jdk11-slim`](#jetty9-jdk11-slim)
-	[`jetty:9-jdk16`](#jetty9-jdk16)
-	[`jetty:9-jdk16-slim`](#jetty9-jdk16-slim)
-	[`jetty:9-jdk8`](#jetty9-jdk8)
-	[`jetty:9-jdk8-slim`](#jetty9-jdk8-slim)
-	[`jetty:9-jre11`](#jetty9-jre11)
-	[`jetty:9-jre11-slim`](#jetty9-jre11-slim)
-	[`jetty:9-jre8`](#jetty9-jre8)
-	[`jetty:9-jre8-slim`](#jetty9-jre8-slim)
-	[`jetty:9.2-jre8`](#jetty92-jre8)
-	[`jetty:9.2.30-jre8`](#jetty9230-jre8)
-	[`jetty:9.3-jre8`](#jetty93-jre8)
-	[`jetty:9.3.29-jre8`](#jetty9329-jre8)
-	[`jetty:9.4`](#jetty94)
-	[`jetty:9.4-jdk11`](#jetty94-jdk11)
-	[`jetty:9.4-jdk11-slim`](#jetty94-jdk11-slim)
-	[`jetty:9.4-jdk16`](#jetty94-jdk16)
-	[`jetty:9.4-jdk16-slim`](#jetty94-jdk16-slim)
-	[`jetty:9.4-jdk8`](#jetty94-jdk8)
-	[`jetty:9.4-jdk8-slim`](#jetty94-jdk8-slim)
-	[`jetty:9.4-jre11`](#jetty94-jre11)
-	[`jetty:9.4-jre11-slim`](#jetty94-jre11-slim)
-	[`jetty:9.4-jre8`](#jetty94-jre8)
-	[`jetty:9.4-jre8-slim`](#jetty94-jre8-slim)
-	[`jetty:9.4.43`](#jetty9443)
-	[`jetty:9.4.43-jdk11`](#jetty9443-jdk11)
-	[`jetty:9.4.43-jdk11-slim`](#jetty9443-jdk11-slim)
-	[`jetty:9.4.43-jdk16`](#jetty9443-jdk16)
-	[`jetty:9.4.43-jdk16-slim`](#jetty9443-jdk16-slim)
-	[`jetty:9.4.43-jdk8`](#jetty9443-jdk8)
-	[`jetty:9.4.43-jdk8-slim`](#jetty9443-jdk8-slim)
-	[`jetty:9.4.43-jre11`](#jetty9443-jre11)
-	[`jetty:9.4.43-jre11-slim`](#jetty9443-jre11-slim)
-	[`jetty:9.4.43-jre8`](#jetty9443-jre8)
-	[`jetty:9.4.43-jre8-slim`](#jetty9443-jre8-slim)
-	[`jetty:jdk16`](#jettyjdk16)
-	[`jetty:latest`](#jettylatest)

## `jetty:10.0.6`

```console
$ docker pull jetty@sha256:eed0a49c93041f28e41c16c52fcd62aaf29d7d2d4aae7dbec10f3828491e984c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6` - linux; amd64

```console
$ docker pull jetty@sha256:0645b5c849fd4f376d1cfeca23719a6c0be0e5c83b23bf782b3dd10f0a18a472
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.1 MB (250054500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50f96a8ca6e03a183abeafbe8e2eb1f9cff6339448d251f2c44322cd34df0b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:04:36 GMT
ENV JETTY_VERSION=10.0.6
# Thu, 12 Aug 2021 20:04:37 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:04:37 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:04:37 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:04:37 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:04:37 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Thu, 12 Aug 2021 20:04:38 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:04:45 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:04:46 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:04:46 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:04:46 GMT
USER jetty
# Thu, 12 Aug 2021 20:04:46 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:04:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:04:47 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b7a60f7927167e79325e4630818163a0e3bcc9ccbff5a5e7d450b08554122`  
		Last Modified: Thu, 12 Aug 2021 20:06:48 GMT  
		Size: 9.7 MB (9714605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b06da9a7a4a17ec89a8428727d33ffe373ed09996a091810996e3deb77c513`  
		Last Modified: Thu, 12 Aug 2021 20:06:47 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:10.0.6-jdk11`

```console
$ docker pull jetty@sha256:47a7ae491d5f2f36da548ef07156ecce7618d2818e56b35a114b74950bbae427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6-jdk11` - linux; amd64

```console
$ docker pull jetty@sha256:64ad06c6d71bc9854017f639477b4921bed0b18fe249aeb6e03721bf8f624ce6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.2 MB (338237731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ba9e55870770545d2dc4772a863b79b5ee19ace51ad8f5829b3c756e4dcb7d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:35:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:35:51 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:35:52 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Jul 2021 13:36:06 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 06:58:40 GMT
ENV JETTY_VERSION=10.0.6
# Fri, 23 Jul 2021 06:58:40 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:58:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:58:41 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:58:41 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:58:41 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Fri, 23 Jul 2021 06:58:41 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:58:48 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:58:48 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:58:49 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:58:49 GMT
USER jetty
# Fri, 23 Jul 2021 06:58:49 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:58:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:58:49 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f970878fad14882553683f35f608f8e510c8886959085d5c5b43947104abe`  
		Last Modified: Thu, 22 Jul 2021 13:48:14 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed434bfebf18b6bcb8ae2c5552ff4319f726cbfa5006cd890d8c044403fee7fb`  
		Last Modified: Thu, 22 Jul 2021 13:48:30 GMT  
		Size: 203.1 MB (203126840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d233451203fc40d5f35855844bac8705176fa1ff74229eed8c7fc14ea904c1b`  
		Last Modified: Fri, 23 Jul 2021 07:04:43 GMT  
		Size: 9.7 MB (9715719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918a214e40e711b762e9bf8c9690dd4da4606027c68f60f0a686e2bfe9a0953`  
		Last Modified: Fri, 23 Jul 2021 07:04:41 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:10.0.6-jdk11-slim`

```console
$ docker pull jetty@sha256:9ca3acb4a7f6b408889bb20ab0e4933eef093c4d4b4f32dd779b552b1f2f0cb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6-jdk11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:3f410d6a6b7468d8a5e5706bbf25eccd1c33648991e25ff39cb3082e682b3f6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243806683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e57057f0565a0a767a066cde52d957f9d531c06bb1937acbbc29c3ed9289220`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:55:08 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:51:58 GMT
ENV JETTY_VERSION=10.0.6
# Tue, 17 Aug 2021 18:51:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:51:58 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:51:58 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:51:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:51:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Tue, 17 Aug 2021 18:51:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:52:16 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:52:17 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:52:18 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:52:18 GMT
USER jetty
# Tue, 17 Aug 2021 18:52:18 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:52:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:52:19 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0a59079bf8f55f7ca770b4e060d8f49a02723cde1616cdc7ea122832e46095`  
		Last Modified: Tue, 17 Aug 2021 07:03:02 GMT  
		Size: 203.4 MB (203396055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6a6d1b775f4d78d5e121110c43941c7bf31e55a01c664160bbd5dad1999fe`  
		Last Modified: Tue, 17 Aug 2021 18:57:21 GMT  
		Size: 10.0 MB (9994215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061345718f44622ec14f2f88cd7bcef1533f4a4b4a58777dc86bc25775b91383`  
		Last Modified: Tue, 17 Aug 2021 18:57:20 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:10.0.6-jdk16`

```console
$ docker pull jetty@sha256:eed0a49c93041f28e41c16c52fcd62aaf29d7d2d4aae7dbec10f3828491e984c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6-jdk16` - linux; amd64

```console
$ docker pull jetty@sha256:0645b5c849fd4f376d1cfeca23719a6c0be0e5c83b23bf782b3dd10f0a18a472
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.1 MB (250054500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50f96a8ca6e03a183abeafbe8e2eb1f9cff6339448d251f2c44322cd34df0b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:04:36 GMT
ENV JETTY_VERSION=10.0.6
# Thu, 12 Aug 2021 20:04:37 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:04:37 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:04:37 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:04:37 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:04:37 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Thu, 12 Aug 2021 20:04:38 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:04:45 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:04:46 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:04:46 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:04:46 GMT
USER jetty
# Thu, 12 Aug 2021 20:04:46 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:04:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:04:47 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774b7a60f7927167e79325e4630818163a0e3bcc9ccbff5a5e7d450b08554122`  
		Last Modified: Thu, 12 Aug 2021 20:06:48 GMT  
		Size: 9.7 MB (9714605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b06da9a7a4a17ec89a8428727d33ffe373ed09996a091810996e3deb77c513`  
		Last Modified: Thu, 12 Aug 2021 20:06:47 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:10.0.6-jdk16-slim`

```console
$ docker pull jetty@sha256:654828d4287ea770e7b4d38c78799913aeeab32ed4a38d170f5f108b76113e8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6-jdk16-slim` - linux; amd64

```console
$ docker pull jetty@sha256:a05c9103a16d1d1b23bf9c460b1863f257dd32524b774b9e2b8bd08f84d71ae3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.6 MB (225598584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701efb35a985685f9c4692fc9036fffaf5395079e9e6653a1d30eb2808fa52db`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 17 Aug 2021 06:54:11 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 17 Aug 2021 06:54:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:54:26 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:51:33 GMT
ENV JETTY_VERSION=10.0.6
# Tue, 17 Aug 2021 18:51:34 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:51:34 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:51:34 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:51:34 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:51:34 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Tue, 17 Aug 2021 18:51:35 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:51:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:51:51 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:51:51 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:51:51 GMT
USER jetty
# Tue, 17 Aug 2021 18:51:52 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:51:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:51:52 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ad83747fb7044c2d6fcded5230f47d13e824250a8f11b72b2b24989f2f1bf5`  
		Last Modified: Tue, 17 Aug 2021 07:01:53 GMT  
		Size: 185.2 MB (185189599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f17663364da457448c85ae8916d840ad09aa317004a6eb7b9e53219225b278f0`  
		Last Modified: Tue, 17 Aug 2021 18:57:11 GMT  
		Size: 10.0 MB (9992784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e29058c96abaa056699ba35d28894f33c5f7acd2e4d79a8096d485cceaa9951`  
		Last Modified: Tue, 17 Aug 2021 18:57:10 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:10.0.6-jre11`

```console
$ docker pull jetty@sha256:931de5ea42a897ffca69d6f8c23474414df1460d5efede1d68e8bcf035343c56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:7ebee5170032c0166777f0274e0da6ce62e471580434cb03a556133ba1d7af5a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130378299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a72ff6092117e94a990e82be017aaebd50f277524b33a2b9d69b2e1116e18590`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:36:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:36:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:36:47 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:36:48 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:36:48 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Fri, 23 Jul 2021 06:57:31 GMT
ENV JETTY_VERSION=10.0.6
# Fri, 23 Jul 2021 06:57:31 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:57:31 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:57:31 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:57:31 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:57:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Fri, 23 Jul 2021 06:57:32 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:57:39 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:57:39 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:57:39 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:57:39 GMT
USER jetty
# Fri, 23 Jul 2021 06:57:40 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:57:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:57:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4a4d63704982a336f8cf6aae3cb36289ab6cbb2928c25a41a5d5adcbc5368`  
		Last Modified: Thu, 22 Jul 2021 13:49:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6172f170f291e20ff4db4b3892e4444242091b4b12f5fe9e785b4fd2870d6`  
		Last Modified: Thu, 22 Jul 2021 13:50:02 GMT  
		Size: 46.9 MB (46864013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c760f909d06f93f9e27b5e4350bdc33db3ebb1e8b7e62624a2fa4ee437c18c01`  
		Last Modified: Fri, 23 Jul 2021 07:04:07 GMT  
		Size: 9.7 MB (9715728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac692d2ec3107b853f2c72aca5ad98353fa83289eb159832617b5f97cd65c72`  
		Last Modified: Fri, 23 Jul 2021 07:04:06 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:10.0.6-jre11-slim`

```console
$ docker pull jetty@sha256:e10b1774e24b69e1fae8c1f16698dcc498d238d0fc4d4ea36d35572440eecffb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:10.0.6-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:8c804b20f750a78841fa363d4ed0d137c087cc002693a83d7bdcf4ca4535eb49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87547799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3fa4ce526e9cd8066770fa8ae528d627ee6e35caf306ff9853ffef2aee4960`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 18:51:09 GMT
ENV JETTY_VERSION=10.0.6
# Tue, 17 Aug 2021 18:51:10 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:51:10 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:51:10 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:51:10 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:51:10 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.6/jetty-home-10.0.6.tar.gz
# Tue, 17 Aug 2021 18:51:11 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:51:27 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:51:27 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:51:28 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:51:28 GMT
USER jetty
# Tue, 17 Aug 2021 18:51:28 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:51:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:51:28 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663bffc94428db61042052aaa00b98a379ea871642fce53bdc8ac9e06754493b`  
		Last Modified: Tue, 17 Aug 2021 07:03:45 GMT  
		Size: 47.1 MB (47137229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f6b981c0cd78e476d4929235152613f74943107998fee863b336fb1860d80c`  
		Last Modified: Tue, 17 Aug 2021 18:57:02 GMT  
		Size: 10.0 MB (9994159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b24fb6230fa4735653c87158752f5ef6b1e39d8b9044c920cb238def6e85c2a`  
		Last Modified: Tue, 17 Aug 2021 18:57:01 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6`

```console
$ docker pull jetty@sha256:23beaaed95abcaf7d265aca538e56a9d47218ac69ce0e3b3ccfdea5e7f49dcd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6` - linux; amd64

```console
$ docker pull jetty@sha256:1bfa037fe6b7073cf09b6f417ad6eb19325b47e4a66a891f3e64eb3ca66cf623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.8 MB (253768704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a06913749b69dd7ccf1fb3cb941694f562912efe8a5c1d7d41cc01c35b278ae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:04:07 GMT
ENV JETTY_VERSION=11.0.6
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:04:08 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:04:08 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:04:21 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:04:21 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:04:22 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:04:22 GMT
USER jetty
# Thu, 12 Aug 2021 20:04:22 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:04:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:04:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccdd03ef97a1644fd8b2b9d35ba1607ff2b89386518ae774d9d98d1f43ed7`  
		Last Modified: Thu, 12 Aug 2021 20:06:35 GMT  
		Size: 13.4 MB (13428808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42908cc54f4fe9d6202c05b04aa37aa4102b2595711cc534360f6df208424421`  
		Last Modified: Thu, 12 Aug 2021 20:06:34 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6-jdk11`

```console
$ docker pull jetty@sha256:e072acd3160abf9eaee4f2c7dd87f83b0f0537110fcbb88c353c467c6ed1ae3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6-jdk11` - linux; amd64

```console
$ docker pull jetty@sha256:6bc024b61a61fc751768f09f94603d5efa6b4a95e115b3508a50807ddbe21eb4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.0 MB (341952209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2619f727c6ca29de938f370f675dc6a9d9a0fdc9390fdaf5f77d8a3093a6a7aa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:35:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:35:51 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:35:52 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Jul 2021 13:36:06 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 06:56:56 GMT
ENV JETTY_VERSION=11.0.6
# Fri, 23 Jul 2021 06:56:56 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:56:56 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:56:56 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:56:57 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:56:57 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Fri, 23 Jul 2021 06:56:57 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:57:04 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:57:04 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:57:04 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:57:04 GMT
USER jetty
# Fri, 23 Jul 2021 06:57:05 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:57:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:57:05 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f970878fad14882553683f35f608f8e510c8886959085d5c5b43947104abe`  
		Last Modified: Thu, 22 Jul 2021 13:48:14 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed434bfebf18b6bcb8ae2c5552ff4319f726cbfa5006cd890d8c044403fee7fb`  
		Last Modified: Thu, 22 Jul 2021 13:48:30 GMT  
		Size: 203.1 MB (203126840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0746360b66f355c48b2f4f60fe4686e4f981cd1d854796469ed950c91b62ca10`  
		Last Modified: Fri, 23 Jul 2021 07:03:50 GMT  
		Size: 13.4 MB (13430197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a1aa54b76e8131329fae73973044030549af41dc880973d1a7784bc23247eb`  
		Last Modified: Fri, 23 Jul 2021 07:03:49 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6-jdk11-slim`

```console
$ docker pull jetty@sha256:5d1ac5ff9799f8c86dab279ec4365dfd235f9a0bacb4cd0270d5dc79f10b4c94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6-jdk11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:c10a6d4a0c6c6818b5a15c9323d151530dbf1f488e44b700fea718c4dd5a797b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.5 MB (247522295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37090152ea6f741bb811ddd959569a4cf546ba7618e1e9932b64904e35ee1c76`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:55:08 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:50:46 GMT
ENV JETTY_VERSION=11.0.6
# Tue, 17 Aug 2021 18:50:46 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:50:46 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:50:46 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:50:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:50:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Tue, 17 Aug 2021 18:50:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:51:03 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:51:03 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:51:03 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:51:04 GMT
USER jetty
# Tue, 17 Aug 2021 18:51:04 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:51:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:51:04 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0a59079bf8f55f7ca770b4e060d8f49a02723cde1616cdc7ea122832e46095`  
		Last Modified: Tue, 17 Aug 2021 07:03:02 GMT  
		Size: 203.4 MB (203396055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede1e603dd14a6a42f5a54ca1607fea111a1c9afedf83b6305b455297326912c`  
		Last Modified: Tue, 17 Aug 2021 18:56:52 GMT  
		Size: 13.7 MB (13709828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac981359de62d43c14ce0bc55a736f5434b29b7e43ea3e0f5537190f322386cc`  
		Last Modified: Tue, 17 Aug 2021 18:56:51 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6-jdk16`

```console
$ docker pull jetty@sha256:23beaaed95abcaf7d265aca538e56a9d47218ac69ce0e3b3ccfdea5e7f49dcd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6-jdk16` - linux; amd64

```console
$ docker pull jetty@sha256:1bfa037fe6b7073cf09b6f417ad6eb19325b47e4a66a891f3e64eb3ca66cf623
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.8 MB (253768704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a06913749b69dd7ccf1fb3cb941694f562912efe8a5c1d7d41cc01c35b278ae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:04:07 GMT
ENV JETTY_VERSION=11.0.6
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:04:08 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:04:08 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Thu, 12 Aug 2021 20:04:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:04:21 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:04:21 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:04:22 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:04:22 GMT
USER jetty
# Thu, 12 Aug 2021 20:04:22 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:04:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:04:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adccdd03ef97a1644fd8b2b9d35ba1607ff2b89386518ae774d9d98d1f43ed7`  
		Last Modified: Thu, 12 Aug 2021 20:06:35 GMT  
		Size: 13.4 MB (13428808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42908cc54f4fe9d6202c05b04aa37aa4102b2595711cc534360f6df208424421`  
		Last Modified: Thu, 12 Aug 2021 20:06:34 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6-jdk16-slim`

```console
$ docker pull jetty@sha256:70624fbb6e38b4917f9515564d206b865b77a92eae8b88423643069d1f96d1fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6-jdk16-slim` - linux; amd64

```console
$ docker pull jetty@sha256:bd43c157b806dee66a51e67cab82ae39a8525e8dbd2d2c1f0e9bd6e06c520a84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.3 MB (229313849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4e03f80186cb7ab67bfacd92fd25aa3474ac2453e224c822f484995ed2fced`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 17 Aug 2021 06:54:11 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 17 Aug 2021 06:54:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:54:26 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:50:21 GMT
ENV JETTY_VERSION=11.0.6
# Tue, 17 Aug 2021 18:50:21 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:50:21 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:50:21 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:50:22 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:50:22 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Tue, 17 Aug 2021 18:50:22 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:50:38 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:50:39 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:50:39 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:50:39 GMT
USER jetty
# Tue, 17 Aug 2021 18:50:39 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:50:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:50:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ad83747fb7044c2d6fcded5230f47d13e824250a8f11b72b2b24989f2f1bf5`  
		Last Modified: Tue, 17 Aug 2021 07:01:53 GMT  
		Size: 185.2 MB (185189599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0499093440043203404da0ee59d290f46d2a82d05b019e9a27572aaf1af0b3fb`  
		Last Modified: Tue, 17 Aug 2021 18:56:42 GMT  
		Size: 13.7 MB (13708051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ed6dcb5d15de549138180419e3eb1f5f0f59ecab11639e7dbeb5886a8107d1`  
		Last Modified: Tue, 17 Aug 2021 18:56:41 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6-jre11`

```console
$ docker pull jetty@sha256:12dde3a2828dd086c935fe071fe1f4c709abbea0bcfd6d5f15d2da4d90281696
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:3d6d19712ce2a5775e11f255c555a0a419aa6ad630dc4d29e0101298f39cc74f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134092765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c7a859300dfdf1cd497f54f4f4cb9b65b69448c25453bc7163221eba8f19fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:36:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:36:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:36:47 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:36:48 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:36:48 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Fri, 23 Jul 2021 06:55:46 GMT
ENV JETTY_VERSION=11.0.6
# Fri, 23 Jul 2021 06:55:47 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:55:47 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:55:47 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:55:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:55:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Fri, 23 Jul 2021 06:55:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:55:55 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:55:55 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:55:55 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:55:55 GMT
USER jetty
# Fri, 23 Jul 2021 06:55:56 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:55:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:55:56 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4a4d63704982a336f8cf6aae3cb36289ab6cbb2928c25a41a5d5adcbc5368`  
		Last Modified: Thu, 22 Jul 2021 13:49:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6172f170f291e20ff4db4b3892e4444242091b4b12f5fe9e785b4fd2870d6`  
		Last Modified: Thu, 22 Jul 2021 13:50:02 GMT  
		Size: 46.9 MB (46864013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032909605d387f5eac7610ee4195981536f823d249bba93f0a0ff9712f13dde0`  
		Last Modified: Fri, 23 Jul 2021 07:03:11 GMT  
		Size: 13.4 MB (13430194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355be47330c28458a0ff9207642735fa8839f25fec1cef2f7ad8983ca22339e4`  
		Last Modified: Fri, 23 Jul 2021 07:03:10 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:11.0.6-jre11-slim`

```console
$ docker pull jetty@sha256:1fc6bc6fe776827474c95f78b02d73ecf0a75d8c9772ff3168f9374b5331fd87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:11.0.6-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:945461a11a651f079a569e284a5ebd7ca39b0a89477460d0fa991e2276a1e1e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.3 MB (91263354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e6f0932b2ebdd5974fdc33ee973d20ca9f395e4275d45ac5bad67d658f7051`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 18:49:42 GMT
ENV JETTY_VERSION=11.0.6
# Tue, 17 Aug 2021 18:49:43 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:49:43 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:49:43 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:49:44 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:49:44 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/11.0.6/jetty-home-11.0.6.tar.gz
# Tue, 17 Aug 2021 18:49:44 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:50:12 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:50:12 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:50:13 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:50:13 GMT
USER jetty
# Tue, 17 Aug 2021 18:50:14 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:50:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:50:14 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663bffc94428db61042052aaa00b98a379ea871642fce53bdc8ac9e06754493b`  
		Last Modified: Tue, 17 Aug 2021 07:03:45 GMT  
		Size: 47.1 MB (47137229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616ae3cff287e76531a537ce5a7010de9d1c5f30efed8d7068d67a59e17715fa`  
		Last Modified: Tue, 17 Aug 2021 18:56:33 GMT  
		Size: 13.7 MB (13709711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6db2e903c4bb0d2f83dc60f091369e5a0add1d77dce05f81d8a61530fea450`  
		Last Modified: Tue, 17 Aug 2021 18:56:32 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk11`

```console
$ docker pull jetty@sha256:981c7b25e90efb473dc1dd454271090b743313e00c8ba48cbb2a94f94bfe52b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk11` - linux; amd64

```console
$ docker pull jetty@sha256:e0196c15b8eca94aac36b960e45de121e49a80ccda4331329710c65132c3d3a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338375071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871e5fd87fe4cba18e330165c700c69d9faed8b4f359c99d6383faf3a80ba9a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:35:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:35:51 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:35:52 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Jul 2021 13:36:06 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:00:59 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:00:59 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:00:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 07:00:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 07:01:07 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 07:01:07 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:07 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:07 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:08 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:08 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f970878fad14882553683f35f608f8e510c8886959085d5c5b43947104abe`  
		Last Modified: Thu, 22 Jul 2021 13:48:14 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed434bfebf18b6bcb8ae2c5552ff4319f726cbfa5006cd890d8c044403fee7fb`  
		Last Modified: Thu, 22 Jul 2021 13:48:30 GMT  
		Size: 203.1 MB (203126840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2890585e7d2cba10effebc57a553c69b822289cc1e40614bc508cfc676cbae`  
		Last Modified: Fri, 23 Jul 2021 07:06:40 GMT  
		Size: 9.9 MB (9853059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f9a6cae06da8b65d9c9614da3ef83d05c3256a6e97260cb7cc2e0286fa4671`  
		Last Modified: Fri, 23 Jul 2021 07:06:39 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk11-slim`

```console
$ docker pull jetty@sha256:f5cfeef23f62557e3ab8b9fd906a97c93a20325376198b8e3de9cfbc1c53205e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:b6129ffb23b560f243522bcdecd65b31a1590b2f53076846d082f7993c1908f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243945688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50cca3404afd93b2c54e7548cc192330fc8c03ee88a63793560075bb026c7d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:55:08 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:54:18 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:54:18 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:54:18 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:54:19 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:54:41 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:54:41 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:54:42 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:54:42 GMT
USER jetty
# Tue, 17 Aug 2021 18:54:42 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:54:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:54:43 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0a59079bf8f55f7ca770b4e060d8f49a02723cde1616cdc7ea122832e46095`  
		Last Modified: Tue, 17 Aug 2021 07:03:02 GMT  
		Size: 203.4 MB (203396055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152791ae647028cbdf5ecfbc86652e86d9cb560ad058b0d3b32afeea118ef435`  
		Last Modified: Tue, 17 Aug 2021 18:58:20 GMT  
		Size: 10.1 MB (10133220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a03c5d8ea655f24b04cafad6c7ba3f5733640a89ba35beb84159257e4eaaa9`  
		Last Modified: Tue, 17 Aug 2021 18:58:18 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk16`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk16` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk16-slim`

```console
$ docker pull jetty@sha256:bb28f2175f04ac0afe7056c7c337e2711a67d2bff830e12b73be378fee6fddb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk16-slim` - linux; amd64

```console
$ docker pull jetty@sha256:26ddb87de319b43efae5673451cc0af505fe7dda20daa49f31ad2e1e3181acc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225737261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d4d4fc61e8a4edd42da04322c321542715b98015d53f988575cfebaf76e139`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 17 Aug 2021 06:54:11 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 17 Aug 2021 06:54:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:54:26 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:53:42 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:53:42 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:53:42 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:53:42 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:54:03 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:54:03 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:54:04 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:54:04 GMT
USER jetty
# Tue, 17 Aug 2021 18:54:04 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:54:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:54:05 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ad83747fb7044c2d6fcded5230f47d13e824250a8f11b72b2b24989f2f1bf5`  
		Last Modified: Tue, 17 Aug 2021 07:01:53 GMT  
		Size: 185.2 MB (185189599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504137de46a6e7e98355f577ff70dec53da19dc464250c33c9b2d92260097fef`  
		Last Modified: Tue, 17 Aug 2021 18:58:01 GMT  
		Size: 10.1 MB (10131461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69186bdfcd05fc5f6ca509e60f8fa2852f211cc5978168bf0e969251169ba22d`  
		Last Modified: Tue, 17 Aug 2021 18:58:01 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk8`

```console
$ docker pull jetty@sha256:f36a93a458fc5137d38fccf1a78ddeda15e46822943dd6bf6ee82ff943261522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk8` - linux; amd64

```console
$ docker pull jetty@sha256:093f16c4311d71ded5ae426f4b0f2eaaf160cae2edaf3e86605119dd04d7af1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241241239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac6185f2f3eb714fa07e8b0cd5f7c6560eb87a3bd677683373e62f0c30bf62b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:37:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:37:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:37:23 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:37:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:37:23 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:37:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:33 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:34 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:34 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 07:01:34 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 07:01:41 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 07:01:41 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:42 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:42 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:42 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:42 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5dee180760796a18d9e387c8d18020519dd17415ccefe9d33eaddde5e73d62`  
		Last Modified: Thu, 22 Jul 2021 13:50:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26c02f721c269f3df6c3d2cbc36042d2e89cd7bc7aeaf24d0603e30e014ae45`  
		Last Modified: Thu, 22 Jul 2021 13:50:59 GMT  
		Size: 106.0 MB (105993014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dfea9c9510e26f432f61251ef4872e527e3450cf8e49bc66cb7da496499fa4`  
		Last Modified: Fri, 23 Jul 2021 07:07:10 GMT  
		Size: 9.9 MB (9853053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f61b2f740f3e62734316433b0978c05b6178eacfa68b4636461d4efc4d14910`  
		Last Modified: Fri, 23 Jul 2021 07:07:09 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk8-slim`

```console
$ docker pull jetty@sha256:2cb536296ea48b728db5720b0623e1ecf2f4c196fbe23f9e96468b4f32a0e3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jdk8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:df8f4fc4f7748c996679464d0d7d92d84224990879b7857dbe8dfcdd29f27235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146818720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d8050c4111360f3cdd51162ab7ab8871467d266acfa9adc541ef00892fa6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:54:51 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:54:52 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:54:52 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:54:52 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:55:15 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:55:15 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:55:16 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:55:16 GMT
USER jetty
# Tue, 17 Aug 2021 18:55:16 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:55:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:55:17 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fdd77aee065a3593352d4910487a661d9f1cc12555573e767f55ba3e1c10e0`  
		Last Modified: Tue, 17 Aug 2021 07:04:19 GMT  
		Size: 106.3 MB (106270512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240559f39de32db44c9ad352f1c532ac6bd8e8651e0f6ca3bd9272728d456d13`  
		Last Modified: Tue, 17 Aug 2021 18:58:36 GMT  
		Size: 10.1 MB (10131795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3262ebab7c98d109ec1bd6950016290289c265df653aaa167af1e363254f99`  
		Last Modified: Tue, 17 Aug 2021 18:58:36 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre11`

```console
$ docker pull jetty@sha256:cf6fab1e124bd172a99cc5f444998004c39009b9a7a85e07b2071ed4da282f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:6827ba260cce1694cc8966a4227b91cf8e85c8e8a1f5e596b6c381fe05937c26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130515617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:122bf720dd9c7858c8c32903c6bae77f6abc6f6303ee936b2acc24873c45b7d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:36:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:36:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:36:47 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:36:48 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:36:48 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:59:16 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:59:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:59:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 06:59:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:59:23 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:59:23 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:59:23 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:59:23 GMT
USER jetty
# Fri, 23 Jul 2021 06:59:23 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:59:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:59:24 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4a4d63704982a336f8cf6aae3cb36289ab6cbb2928c25a41a5d5adcbc5368`  
		Last Modified: Thu, 22 Jul 2021 13:49:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6172f170f291e20ff4db4b3892e4444242091b4b12f5fe9e785b4fd2870d6`  
		Last Modified: Thu, 22 Jul 2021 13:50:02 GMT  
		Size: 46.9 MB (46864013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2267fb349bf26ba4686e70a5917aab61dd091d637a4b86527b3d70c702f65e52`  
		Last Modified: Fri, 23 Jul 2021 07:05:05 GMT  
		Size: 9.9 MB (9853046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04c9a88beab783b8a9b0eb8738064e51779c80c738a9c0cc7cad8b164ecd665`  
		Last Modified: Fri, 23 Jul 2021 07:05:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9-jre11` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:1a07c17ad9c475e8c3ab89b9f648c08f76ef5578620e1d7bc51810a447586706
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128192433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37af330e0ffc0944c8ea84b25cd17b5efc19878eff9f20254251d0e52511eee8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 05:19:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:19:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 05:19:58 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 05:19:58 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 05:19:58 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 05:19:59 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 05:20:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 22 Jul 2021 21:18:31 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 22 Jul 2021 21:18:32 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 21:18:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 22 Jul 2021 21:18:32 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 22 Jul 2021 21:18:39 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 22 Jul 2021 21:18:39 GMT
WORKDIR /var/lib/jetty
# Thu, 22 Jul 2021 21:18:39 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 22 Jul 2021 21:18:39 GMT
USER jetty
# Thu, 22 Jul 2021 21:18:40 GMT
EXPOSE 8080
# Thu, 22 Jul 2021 21:18:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 22 Jul 2021 21:18:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b2c9f5cef9708e735967f5de94f32003e308811f5df8fa33e09517ebeb7ae5`  
		Last Modified: Thu, 22 Jul 2021 05:37:44 GMT  
		Size: 5.5 MB (5505472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e2e88ae1dedf4258ab2fab5534ce7eb7bca1bcb94c42355ea79adb5dad107`  
		Last Modified: Thu, 22 Jul 2021 05:37:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b704173261f5be427cc946401c131da901ac5a7638e1521c1a4f7b539713e0`  
		Last Modified: Thu, 22 Jul 2021 05:37:50 GMT  
		Size: 45.9 MB (45930931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2822e39998d3f07ebd834f24d834323207c8557ae0e77f81d3e741fecf067fc`  
		Last Modified: Thu, 22 Jul 2021 21:19:21 GMT  
		Size: 9.9 MB (9853022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef13c62a343e3f2198fb56261650aa26eced41edd55a0362203e4e3419ab207`  
		Last Modified: Thu, 22 Jul 2021 21:19:20 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre11-slim`

```console
$ docker pull jetty@sha256:f971551cf97a446fca1d91206a7fabf7a1a3a715dd0e2a0c172a82e7c9609401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:4a695365926694c5c74786f856b308b82f0b1ab7c4662d601e34ce02f051977f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87686770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17065f0194a09cd5ab90dbda54124cc7708649ae8bf37894d26b3e5f01a49a31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:52:28 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:52:28 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:52:28 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:52:29 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:52:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:52:51 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:52:52 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:52:52 GMT
USER jetty
# Tue, 17 Aug 2021 18:52:53 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:52:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:52:53 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663bffc94428db61042052aaa00b98a379ea871642fce53bdc8ac9e06754493b`  
		Last Modified: Tue, 17 Aug 2021 07:03:45 GMT  
		Size: 47.1 MB (47137229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210a578564c3c97979e60d07ed2430cf8a7c2de433a65067122f9353769bb92`  
		Last Modified: Tue, 17 Aug 2021 18:57:30 GMT  
		Size: 10.1 MB (10133127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05254c4841fdd3f3309b9f28e1c7e5b268e7a428854ac19f533e8eeda906abf0`  
		Last Modified: Tue, 17 Aug 2021 18:57:29 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9-jre11-slim` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:5cef81d40cbe6163a12ebeb795a685f82c4bf764631393beff62304ea7d679d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85372141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0c6ecf89566c6b645cf35217655eb66ea2960196c5cba22ed89b1a681a0a23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:04:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:06:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:06:39 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:06:39 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:06:40 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:06:40 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:07:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 15:06:33 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 15:06:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 15:06:52 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 15:06:52 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 15:06:52 GMT
USER jetty
# Tue, 17 Aug 2021 15:06:52 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 15:06:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:53 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a27af984eefbe6b82ccb775aead56e92f82cf16d079218087ebe132125cf5`  
		Last Modified: Tue, 17 Aug 2021 06:15:41 GMT  
		Size: 3.1 MB (3118861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1ea50abf433035bb7f308b855f144aefbbe47ce996fb9e38d8db45df6f75a`  
		Last Modified: Tue, 17 Aug 2021 06:19:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c588b82388c8608ec757f28fdb2010018e105b0185377e9760686d75bd84720`  
		Last Modified: Tue, 17 Aug 2021 06:20:31 GMT  
		Size: 46.2 MB (46203534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056e07629bcce0ced329e35409d5406df7623ca76bf56dfef1e3f71952df97d`  
		Last Modified: Tue, 17 Aug 2021 15:07:22 GMT  
		Size: 10.1 MB (10133016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044aff060f3fb8a334183198c9f35c91ea523124b8d90babecc28c292694f0f8`  
		Last Modified: Tue, 17 Aug 2021 15:07:21 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre8`

```console
$ docker pull jetty@sha256:56d4d91f1f9daeff0dacd6eed8a0d0a450613023ec6816ffe8dbe681c8db4ec0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:bf04496737ae44e7da2ecad5693c72be892efe8c80366247e28f02c6131c70b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125018714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d7967e0f56907792b8367c25e9ca8b53d1dcafccfce130d28a1e86f65cdd19`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 06:59:50 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:59:56 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:59:57 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:59:57 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:59:57 GMT
USER jetty
# Fri, 23 Jul 2021 06:59:57 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:59:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:59:58 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f4546f4bef5b9e49314eddaec771f078092e15b64d89d8a1d85f8ecf43cee`  
		Last Modified: Fri, 23 Jul 2021 07:05:34 GMT  
		Size: 9.9 MB (9853043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db6cd19bd4107bf79cf93a9151642f3a7810705b86e34aa1410e22f87ef19c1`  
		Last Modified: Fri, 23 Jul 2021 07:05:33 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre8-slim`

```console
$ docker pull jetty@sha256:bbb98db45282ee782f609c963da7c16804442930f1a84adc7ccfb142e5382627
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jre8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:72df872a30764ac5438812cbe874e6ada4a249476071679544780a57d1b60404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82190701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d955a50d999b225c136eb7b8f0e2d26530bfae3f59461b8a446d6b72d377bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 17 Aug 2021 18:53:01 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:53:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:53:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:53:02 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:53:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:53:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:53:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:53:28 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:53:28 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:53:29 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:53:29 GMT
USER jetty
# Tue, 17 Aug 2021 18:53:29 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:53:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:53:30 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684a63cea6ad88087bcbba64a242772c2e579702d67656a067619cf4691f0a09`  
		Last Modified: Tue, 17 Aug 2021 07:04:50 GMT  
		Size: 41.6 MB (41641133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbd0b203fe0500696e5f56d54442302307654fb62a304b6d663157d33c00744`  
		Last Modified: Tue, 17 Aug 2021 18:57:46 GMT  
		Size: 10.1 MB (10133156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a934241f4124a75ff57a59dc52f576e4ad66e947be5e190d844c6f4a0c1de683`  
		Last Modified: Tue, 17 Aug 2021 18:57:45 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.2-jre8`

```console
$ docker pull jetty@sha256:d7a4232360f7f27f6a96f0b25fcaad8690e48b95c8e19fe284131ba5695958b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.2-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:34d7f5fa787c54987198c82e7cb0904744e4c188fcb9d4b04d82bc1c0445a078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129013237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7afd9076a97c99450368ca11daf530fc9fb8ba32f31d00f2988b879c3bd3db2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 07:01:57 GMT
ENV JETTY_VERSION=9.2.30.v20200428
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:58 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.2.30.v20200428/jetty-distribution-9.2.30.v20200428.tar.gz
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 23 Jul 2021 07:02:05 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 23 Jul 2021 07:02:05 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:02:05 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 23 Jul 2021 07:02:05 GMT
USER jetty
# Fri, 23 Jul 2021 07:02:06 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:02:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:02:06 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6500aa013621589d04ba73c28a582bcf0847837a69a93741c2a82c2789aa92`  
		Last Modified: Fri, 23 Jul 2021 07:07:35 GMT  
		Size: 13.8 MB (13847597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edfabb16c3561adc4a0ebc7ceda56b3cb6160415f5067801c63886f52e21d40`  
		Last Modified: Fri, 23 Jul 2021 07:07:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.2.30-jre8`

```console
$ docker pull jetty@sha256:d7a4232360f7f27f6a96f0b25fcaad8690e48b95c8e19fe284131ba5695958b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.2.30-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:34d7f5fa787c54987198c82e7cb0904744e4c188fcb9d4b04d82bc1c0445a078
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (129013237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7afd9076a97c99450368ca11daf530fc9fb8ba32f31d00f2988b879c3bd3db2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 07:01:57 GMT
ENV JETTY_VERSION=9.2.30.v20200428
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:58 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.2.30.v20200428/jetty-distribution-9.2.30.v20200428.tar.gz
# Fri, 23 Jul 2021 07:01:58 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 23 Jul 2021 07:02:05 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 23 Jul 2021 07:02:05 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:02:05 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 23 Jul 2021 07:02:05 GMT
USER jetty
# Fri, 23 Jul 2021 07:02:06 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:02:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:02:06 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6500aa013621589d04ba73c28a582bcf0847837a69a93741c2a82c2789aa92`  
		Last Modified: Fri, 23 Jul 2021 07:07:35 GMT  
		Size: 13.8 MB (13847597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edfabb16c3561adc4a0ebc7ceda56b3cb6160415f5067801c63886f52e21d40`  
		Last Modified: Fri, 23 Jul 2021 07:07:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.3-jre8`

```console
$ docker pull jetty@sha256:260a25ec8f3db66af49ed31f1ff013d0bed37a46d36142fc25062fc56c719603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.3-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:c5802dd00538b803a63a2faa63644f495169f427dd8fe423dadcc456462f3638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132905054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158cc2b5aa3d00c1540bb5cc65302e9d6ee0ca609e8b42f1dbd386e748a9747a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 07:01:46 GMT
ENV JETTY_VERSION=9.3.29.v20201019
# Fri, 23 Jul 2021 07:01:46 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:47 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:47 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.3.29.v20201019/jetty-distribution-9.3.29.v20201019.tar.gz
# Fri, 23 Jul 2021 07:01:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 23 Jul 2021 07:01:53 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 23 Jul 2021 07:01:54 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:54 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:54 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:54 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:55 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e821885cc9326c662ee1f6cda16ac0c39100891b323dbea54f57a791fb4db`  
		Last Modified: Fri, 23 Jul 2021 07:07:25 GMT  
		Size: 17.7 MB (17739382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4be6e7af1b9725623550831f900c9a559c658f74a0c635d1d1794cdf79db9c`  
		Last Modified: Fri, 23 Jul 2021 07:07:23 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.3.29-jre8`

```console
$ docker pull jetty@sha256:260a25ec8f3db66af49ed31f1ff013d0bed37a46d36142fc25062fc56c719603
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.3.29-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:c5802dd00538b803a63a2faa63644f495169f427dd8fe423dadcc456462f3638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132905054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:158cc2b5aa3d00c1540bb5cc65302e9d6ee0ca609e8b42f1dbd386e748a9747a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 07:01:46 GMT
ENV JETTY_VERSION=9.3.29.v20201019
# Fri, 23 Jul 2021 07:01:46 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:47 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:47 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:47 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:47 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.3.29.v20201019/jetty-distribution-9.3.29.v20201019.tar.gz
# Fri, 23 Jul 2021 07:01:47 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 23 Jul 2021 07:01:53 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 23 Jul 2021 07:01:54 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:54 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:54 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:54 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:55 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e821885cc9326c662ee1f6cda16ac0c39100891b323dbea54f57a791fb4db`  
		Last Modified: Fri, 23 Jul 2021 07:07:25 GMT  
		Size: 17.7 MB (17739382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4be6e7af1b9725623550831f900c9a559c658f74a0c635d1d1794cdf79db9c`  
		Last Modified: Fri, 23 Jul 2021 07:07:23 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk11`

```console
$ docker pull jetty@sha256:981c7b25e90efb473dc1dd454271090b743313e00c8ba48cbb2a94f94bfe52b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jdk11` - linux; amd64

```console
$ docker pull jetty@sha256:e0196c15b8eca94aac36b960e45de121e49a80ccda4331329710c65132c3d3a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338375071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871e5fd87fe4cba18e330165c700c69d9faed8b4f359c99d6383faf3a80ba9a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:35:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:35:51 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:35:52 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Jul 2021 13:36:06 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:00:59 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:00:59 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:00:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 07:00:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 07:01:07 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 07:01:07 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:07 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:07 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:08 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:08 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f970878fad14882553683f35f608f8e510c8886959085d5c5b43947104abe`  
		Last Modified: Thu, 22 Jul 2021 13:48:14 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed434bfebf18b6bcb8ae2c5552ff4319f726cbfa5006cd890d8c044403fee7fb`  
		Last Modified: Thu, 22 Jul 2021 13:48:30 GMT  
		Size: 203.1 MB (203126840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2890585e7d2cba10effebc57a553c69b822289cc1e40614bc508cfc676cbae`  
		Last Modified: Fri, 23 Jul 2021 07:06:40 GMT  
		Size: 9.9 MB (9853059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f9a6cae06da8b65d9c9614da3ef83d05c3256a6e97260cb7cc2e0286fa4671`  
		Last Modified: Fri, 23 Jul 2021 07:06:39 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk11-slim`

```console
$ docker pull jetty@sha256:f5cfeef23f62557e3ab8b9fd906a97c93a20325376198b8e3de9cfbc1c53205e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jdk11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:b6129ffb23b560f243522bcdecd65b31a1590b2f53076846d082f7993c1908f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243945688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50cca3404afd93b2c54e7548cc192330fc8c03ee88a63793560075bb026c7d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:55:08 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:54:18 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:54:18 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:54:18 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:54:19 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:54:41 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:54:41 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:54:42 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:54:42 GMT
USER jetty
# Tue, 17 Aug 2021 18:54:42 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:54:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:54:43 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0a59079bf8f55f7ca770b4e060d8f49a02723cde1616cdc7ea122832e46095`  
		Last Modified: Tue, 17 Aug 2021 07:03:02 GMT  
		Size: 203.4 MB (203396055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152791ae647028cbdf5ecfbc86652e86d9cb560ad058b0d3b32afeea118ef435`  
		Last Modified: Tue, 17 Aug 2021 18:58:20 GMT  
		Size: 10.1 MB (10133220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a03c5d8ea655f24b04cafad6c7ba3f5733640a89ba35beb84159257e4eaaa9`  
		Last Modified: Tue, 17 Aug 2021 18:58:18 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk16`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jdk16` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk16-slim`

```console
$ docker pull jetty@sha256:bb28f2175f04ac0afe7056c7c337e2711a67d2bff830e12b73be378fee6fddb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jdk16-slim` - linux; amd64

```console
$ docker pull jetty@sha256:26ddb87de319b43efae5673451cc0af505fe7dda20daa49f31ad2e1e3181acc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225737261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d4d4fc61e8a4edd42da04322c321542715b98015d53f988575cfebaf76e139`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 17 Aug 2021 06:54:11 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 17 Aug 2021 06:54:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:54:26 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:53:42 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:53:42 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:53:42 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:53:42 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:54:03 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:54:03 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:54:04 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:54:04 GMT
USER jetty
# Tue, 17 Aug 2021 18:54:04 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:54:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:54:05 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ad83747fb7044c2d6fcded5230f47d13e824250a8f11b72b2b24989f2f1bf5`  
		Last Modified: Tue, 17 Aug 2021 07:01:53 GMT  
		Size: 185.2 MB (185189599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504137de46a6e7e98355f577ff70dec53da19dc464250c33c9b2d92260097fef`  
		Last Modified: Tue, 17 Aug 2021 18:58:01 GMT  
		Size: 10.1 MB (10131461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69186bdfcd05fc5f6ca509e60f8fa2852f211cc5978168bf0e969251169ba22d`  
		Last Modified: Tue, 17 Aug 2021 18:58:01 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk8`

```console
$ docker pull jetty@sha256:f36a93a458fc5137d38fccf1a78ddeda15e46822943dd6bf6ee82ff943261522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jdk8` - linux; amd64

```console
$ docker pull jetty@sha256:093f16c4311d71ded5ae426f4b0f2eaaf160cae2edaf3e86605119dd04d7af1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241241239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac6185f2f3eb714fa07e8b0cd5f7c6560eb87a3bd677683373e62f0c30bf62b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:37:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:37:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:37:23 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:37:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:37:23 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:37:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:33 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:34 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:34 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 07:01:34 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 07:01:41 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 07:01:41 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:42 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:42 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:42 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:42 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5dee180760796a18d9e387c8d18020519dd17415ccefe9d33eaddde5e73d62`  
		Last Modified: Thu, 22 Jul 2021 13:50:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26c02f721c269f3df6c3d2cbc36042d2e89cd7bc7aeaf24d0603e30e014ae45`  
		Last Modified: Thu, 22 Jul 2021 13:50:59 GMT  
		Size: 106.0 MB (105993014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dfea9c9510e26f432f61251ef4872e527e3450cf8e49bc66cb7da496499fa4`  
		Last Modified: Fri, 23 Jul 2021 07:07:10 GMT  
		Size: 9.9 MB (9853053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f61b2f740f3e62734316433b0978c05b6178eacfa68b4636461d4efc4d14910`  
		Last Modified: Fri, 23 Jul 2021 07:07:09 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk8-slim`

```console
$ docker pull jetty@sha256:2cb536296ea48b728db5720b0623e1ecf2f4c196fbe23f9e96468b4f32a0e3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jdk8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:df8f4fc4f7748c996679464d0d7d92d84224990879b7857dbe8dfcdd29f27235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146818720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d8050c4111360f3cdd51162ab7ab8871467d266acfa9adc541ef00892fa6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:54:51 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:54:52 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:54:52 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:54:52 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:55:15 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:55:15 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:55:16 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:55:16 GMT
USER jetty
# Tue, 17 Aug 2021 18:55:16 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:55:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:55:17 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fdd77aee065a3593352d4910487a661d9f1cc12555573e767f55ba3e1c10e0`  
		Last Modified: Tue, 17 Aug 2021 07:04:19 GMT  
		Size: 106.3 MB (106270512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240559f39de32db44c9ad352f1c532ac6bd8e8651e0f6ca3bd9272728d456d13`  
		Last Modified: Tue, 17 Aug 2021 18:58:36 GMT  
		Size: 10.1 MB (10131795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3262ebab7c98d109ec1bd6950016290289c265df653aaa167af1e363254f99`  
		Last Modified: Tue, 17 Aug 2021 18:58:36 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre11`

```console
$ docker pull jetty@sha256:cf6fab1e124bd172a99cc5f444998004c39009b9a7a85e07b2071ed4da282f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:6827ba260cce1694cc8966a4227b91cf8e85c8e8a1f5e596b6c381fe05937c26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130515617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:122bf720dd9c7858c8c32903c6bae77f6abc6f6303ee936b2acc24873c45b7d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:36:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:36:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:36:47 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:36:48 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:36:48 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:59:16 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:59:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:59:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 06:59:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:59:23 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:59:23 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:59:23 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:59:23 GMT
USER jetty
# Fri, 23 Jul 2021 06:59:23 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:59:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:59:24 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4a4d63704982a336f8cf6aae3cb36289ab6cbb2928c25a41a5d5adcbc5368`  
		Last Modified: Thu, 22 Jul 2021 13:49:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6172f170f291e20ff4db4b3892e4444242091b4b12f5fe9e785b4fd2870d6`  
		Last Modified: Thu, 22 Jul 2021 13:50:02 GMT  
		Size: 46.9 MB (46864013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2267fb349bf26ba4686e70a5917aab61dd091d637a4b86527b3d70c702f65e52`  
		Last Modified: Fri, 23 Jul 2021 07:05:05 GMT  
		Size: 9.9 MB (9853046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04c9a88beab783b8a9b0eb8738064e51779c80c738a9c0cc7cad8b164ecd665`  
		Last Modified: Fri, 23 Jul 2021 07:05:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4-jre11` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:1a07c17ad9c475e8c3ab89b9f648c08f76ef5578620e1d7bc51810a447586706
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128192433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37af330e0ffc0944c8ea84b25cd17b5efc19878eff9f20254251d0e52511eee8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 05:19:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:19:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 05:19:58 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 05:19:58 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 05:19:58 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 05:19:59 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 05:20:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 22 Jul 2021 21:18:31 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 22 Jul 2021 21:18:32 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 21:18:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 22 Jul 2021 21:18:32 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 22 Jul 2021 21:18:39 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 22 Jul 2021 21:18:39 GMT
WORKDIR /var/lib/jetty
# Thu, 22 Jul 2021 21:18:39 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 22 Jul 2021 21:18:39 GMT
USER jetty
# Thu, 22 Jul 2021 21:18:40 GMT
EXPOSE 8080
# Thu, 22 Jul 2021 21:18:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 22 Jul 2021 21:18:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b2c9f5cef9708e735967f5de94f32003e308811f5df8fa33e09517ebeb7ae5`  
		Last Modified: Thu, 22 Jul 2021 05:37:44 GMT  
		Size: 5.5 MB (5505472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e2e88ae1dedf4258ab2fab5534ce7eb7bca1bcb94c42355ea79adb5dad107`  
		Last Modified: Thu, 22 Jul 2021 05:37:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b704173261f5be427cc946401c131da901ac5a7638e1521c1a4f7b539713e0`  
		Last Modified: Thu, 22 Jul 2021 05:37:50 GMT  
		Size: 45.9 MB (45930931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2822e39998d3f07ebd834f24d834323207c8557ae0e77f81d3e741fecf067fc`  
		Last Modified: Thu, 22 Jul 2021 21:19:21 GMT  
		Size: 9.9 MB (9853022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef13c62a343e3f2198fb56261650aa26eced41edd55a0362203e4e3419ab207`  
		Last Modified: Thu, 22 Jul 2021 21:19:20 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre11-slim`

```console
$ docker pull jetty@sha256:f971551cf97a446fca1d91206a7fabf7a1a3a715dd0e2a0c172a82e7c9609401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:4a695365926694c5c74786f856b308b82f0b1ab7c4662d601e34ce02f051977f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87686770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17065f0194a09cd5ab90dbda54124cc7708649ae8bf37894d26b3e5f01a49a31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:52:28 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:52:28 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:52:28 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:52:29 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:52:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:52:51 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:52:52 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:52:52 GMT
USER jetty
# Tue, 17 Aug 2021 18:52:53 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:52:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:52:53 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663bffc94428db61042052aaa00b98a379ea871642fce53bdc8ac9e06754493b`  
		Last Modified: Tue, 17 Aug 2021 07:03:45 GMT  
		Size: 47.1 MB (47137229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210a578564c3c97979e60d07ed2430cf8a7c2de433a65067122f9353769bb92`  
		Last Modified: Tue, 17 Aug 2021 18:57:30 GMT  
		Size: 10.1 MB (10133127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05254c4841fdd3f3309b9f28e1c7e5b268e7a428854ac19f533e8eeda906abf0`  
		Last Modified: Tue, 17 Aug 2021 18:57:29 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4-jre11-slim` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:5cef81d40cbe6163a12ebeb795a685f82c4bf764631393beff62304ea7d679d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85372141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0c6ecf89566c6b645cf35217655eb66ea2960196c5cba22ed89b1a681a0a23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:04:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:06:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:06:39 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:06:39 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:06:40 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:06:40 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:07:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 15:06:33 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 15:06:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 15:06:52 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 15:06:52 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 15:06:52 GMT
USER jetty
# Tue, 17 Aug 2021 15:06:52 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 15:06:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:53 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a27af984eefbe6b82ccb775aead56e92f82cf16d079218087ebe132125cf5`  
		Last Modified: Tue, 17 Aug 2021 06:15:41 GMT  
		Size: 3.1 MB (3118861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1ea50abf433035bb7f308b855f144aefbbe47ce996fb9e38d8db45df6f75a`  
		Last Modified: Tue, 17 Aug 2021 06:19:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c588b82388c8608ec757f28fdb2010018e105b0185377e9760686d75bd84720`  
		Last Modified: Tue, 17 Aug 2021 06:20:31 GMT  
		Size: 46.2 MB (46203534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056e07629bcce0ced329e35409d5406df7623ca76bf56dfef1e3f71952df97d`  
		Last Modified: Tue, 17 Aug 2021 15:07:22 GMT  
		Size: 10.1 MB (10133016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044aff060f3fb8a334183198c9f35c91ea523124b8d90babecc28c292694f0f8`  
		Last Modified: Tue, 17 Aug 2021 15:07:21 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre8`

```console
$ docker pull jetty@sha256:56d4d91f1f9daeff0dacd6eed8a0d0a450613023ec6816ffe8dbe681c8db4ec0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:bf04496737ae44e7da2ecad5693c72be892efe8c80366247e28f02c6131c70b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125018714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d7967e0f56907792b8367c25e9ca8b53d1dcafccfce130d28a1e86f65cdd19`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 06:59:50 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:59:56 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:59:57 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:59:57 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:59:57 GMT
USER jetty
# Fri, 23 Jul 2021 06:59:57 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:59:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:59:58 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f4546f4bef5b9e49314eddaec771f078092e15b64d89d8a1d85f8ecf43cee`  
		Last Modified: Fri, 23 Jul 2021 07:05:34 GMT  
		Size: 9.9 MB (9853043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db6cd19bd4107bf79cf93a9151642f3a7810705b86e34aa1410e22f87ef19c1`  
		Last Modified: Fri, 23 Jul 2021 07:05:33 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre8-slim`

```console
$ docker pull jetty@sha256:bbb98db45282ee782f609c963da7c16804442930f1a84adc7ccfb142e5382627
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4-jre8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:72df872a30764ac5438812cbe874e6ada4a249476071679544780a57d1b60404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82190701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d955a50d999b225c136eb7b8f0e2d26530bfae3f59461b8a446d6b72d377bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 17 Aug 2021 18:53:01 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:53:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:53:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:53:02 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:53:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:53:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:53:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:53:28 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:53:28 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:53:29 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:53:29 GMT
USER jetty
# Tue, 17 Aug 2021 18:53:29 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:53:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:53:30 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684a63cea6ad88087bcbba64a242772c2e579702d67656a067619cf4691f0a09`  
		Last Modified: Tue, 17 Aug 2021 07:04:50 GMT  
		Size: 41.6 MB (41641133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbd0b203fe0500696e5f56d54442302307654fb62a304b6d663157d33c00744`  
		Last Modified: Tue, 17 Aug 2021 18:57:46 GMT  
		Size: 10.1 MB (10133156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a934241f4124a75ff57a59dc52f576e4ad66e947be5e190d844c6f4a0c1de683`  
		Last Modified: Tue, 17 Aug 2021 18:57:45 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jdk11`

```console
$ docker pull jetty@sha256:981c7b25e90efb473dc1dd454271090b743313e00c8ba48cbb2a94f94bfe52b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jdk11` - linux; amd64

```console
$ docker pull jetty@sha256:e0196c15b8eca94aac36b960e45de121e49a80ccda4331329710c65132c3d3a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.4 MB (338375071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871e5fd87fe4cba18e330165c700c69d9faed8b4f359c99d6383faf3a80ba9a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:35:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:35:51 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:35:51 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:35:52 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Jul 2021 13:36:06 GMT
CMD ["jshell"]
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:00:58 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:00:59 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:00:59 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:00:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 07:00:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 07:01:07 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 07:01:07 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:07 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:07 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:08 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:08 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f970878fad14882553683f35f608f8e510c8886959085d5c5b43947104abe`  
		Last Modified: Thu, 22 Jul 2021 13:48:14 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed434bfebf18b6bcb8ae2c5552ff4319f726cbfa5006cd890d8c044403fee7fb`  
		Last Modified: Thu, 22 Jul 2021 13:48:30 GMT  
		Size: 203.1 MB (203126840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2890585e7d2cba10effebc57a553c69b822289cc1e40614bc508cfc676cbae`  
		Last Modified: Fri, 23 Jul 2021 07:06:40 GMT  
		Size: 9.9 MB (9853059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f9a6cae06da8b65d9c9614da3ef83d05c3256a6e97260cb7cc2e0286fa4671`  
		Last Modified: Fri, 23 Jul 2021 07:06:39 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jdk11-slim`

```console
$ docker pull jetty@sha256:f5cfeef23f62557e3ab8b9fd906a97c93a20325376198b8e3de9cfbc1c53205e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jdk11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:b6129ffb23b560f243522bcdecd65b31a1590b2f53076846d082f7993c1908f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243945688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a50cca3404afd93b2c54e7548cc192330fc8c03ee88a63793560075bb026c7d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:07 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jdk_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:55:08 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:54:17 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:54:18 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:54:18 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:54:18 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:54:19 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:54:41 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:54:41 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:54:42 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:54:42 GMT
USER jetty
# Tue, 17 Aug 2021 18:54:42 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:54:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:54:43 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0a59079bf8f55f7ca770b4e060d8f49a02723cde1616cdc7ea122832e46095`  
		Last Modified: Tue, 17 Aug 2021 07:03:02 GMT  
		Size: 203.4 MB (203396055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152791ae647028cbdf5ecfbc86652e86d9cb560ad058b0d3b32afeea118ef435`  
		Last Modified: Tue, 17 Aug 2021 18:58:20 GMT  
		Size: 10.1 MB (10133220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a03c5d8ea655f24b04cafad6c7ba3f5733640a89ba35beb84159257e4eaaa9`  
		Last Modified: Tue, 17 Aug 2021 18:58:18 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jdk16`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jdk16` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jdk16-slim`

```console
$ docker pull jetty@sha256:bb28f2175f04ac0afe7056c7c337e2711a67d2bff830e12b73be378fee6fddb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jdk16-slim` - linux; amd64

```console
$ docker pull jetty@sha256:26ddb87de319b43efae5673451cc0af505fe7dda20daa49f31ad2e1e3181acc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225737261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d4d4fc61e8a4edd42da04322c321542715b98015d53f988575cfebaf76e139`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 17 Aug 2021 06:54:11 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:11 GMT
ENV JAVA_VERSION=16.0.2
# Tue, 17 Aug 2021 06:54:25 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 17 Aug 2021 06:54:26 GMT
CMD ["jshell"]
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:53:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:53:42 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:53:42 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:53:42 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:53:42 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:54:03 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:54:03 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:54:04 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:54:04 GMT
USER jetty
# Tue, 17 Aug 2021 18:54:04 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:54:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:54:05 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ad83747fb7044c2d6fcded5230f47d13e824250a8f11b72b2b24989f2f1bf5`  
		Last Modified: Tue, 17 Aug 2021 07:01:53 GMT  
		Size: 185.2 MB (185189599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504137de46a6e7e98355f577ff70dec53da19dc464250c33c9b2d92260097fef`  
		Last Modified: Tue, 17 Aug 2021 18:58:01 GMT  
		Size: 10.1 MB (10131461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69186bdfcd05fc5f6ca509e60f8fa2852f211cc5978168bf0e969251169ba22d`  
		Last Modified: Tue, 17 Aug 2021 18:58:01 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jdk8`

```console
$ docker pull jetty@sha256:f36a93a458fc5137d38fccf1a78ddeda15e46822943dd6bf6ee82ff943261522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jdk8` - linux; amd64

```console
$ docker pull jetty@sha256:093f16c4311d71ded5ae426f4b0f2eaaf160cae2edaf3e86605119dd04d7af1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241241239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac6185f2f3eb714fa07e8b0cd5f7c6560eb87a3bd677683373e62f0c30bf62b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 01:12:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:37:22 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:37:23 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:37:23 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:37:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:37:23 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:37:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 07:01:33 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 07:01:33 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 07:01:34 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 07:01:34 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 07:01:34 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 07:01:41 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 07:01:41 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 07:01:42 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 07:01:42 GMT
USER jetty
# Fri, 23 Jul 2021 07:01:42 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 07:01:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 07:01:42 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76209566d0c8d78df205b09e6e5b52ff7f10cb4e1c03d9336ed7dd2decd919`  
		Last Modified: Thu, 22 Jul 2021 01:20:16 GMT  
		Size: 51.8 MB (51841203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10db7ba7580dd43abbf34313aab51dae288a6ef8dcd1b60860a97679c47942d`  
		Last Modified: Thu, 22 Jul 2021 13:48:15 GMT  
		Size: 5.3 MB (5286518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5dee180760796a18d9e387c8d18020519dd17415ccefe9d33eaddde5e73d62`  
		Last Modified: Thu, 22 Jul 2021 13:50:48 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26c02f721c269f3df6c3d2cbc36042d2e89cd7bc7aeaf24d0603e30e014ae45`  
		Last Modified: Thu, 22 Jul 2021 13:50:59 GMT  
		Size: 106.0 MB (105993014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dfea9c9510e26f432f61251ef4872e527e3450cf8e49bc66cb7da496499fa4`  
		Last Modified: Fri, 23 Jul 2021 07:07:10 GMT  
		Size: 9.9 MB (9853053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f61b2f740f3e62734316433b0978c05b6178eacfa68b4636461d4efc4d14910`  
		Last Modified: Fri, 23 Jul 2021 07:07:09 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jdk8-slim`

```console
$ docker pull jetty@sha256:2cb536296ea48b728db5720b0623e1ecf2f4c196fbe23f9e96468b4f32a0e3c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jdk8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:df8f4fc4f7748c996679464d0d7d92d84224990879b7857dbe8dfcdd29f27235
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146818720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27d8050c4111360f3cdd51162ab7ab8871467d266acfa9adc541ef00892fa6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:01 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:54:51 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:54:51 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:54:52 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:54:52 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:54:52 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:55:15 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:55:15 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:55:16 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:55:16 GMT
USER jetty
# Tue, 17 Aug 2021 18:55:16 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:55:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:55:17 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fdd77aee065a3593352d4910487a661d9f1cc12555573e767f55ba3e1c10e0`  
		Last Modified: Tue, 17 Aug 2021 07:04:19 GMT  
		Size: 106.3 MB (106270512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240559f39de32db44c9ad352f1c532ac6bd8e8651e0f6ca3bd9272728d456d13`  
		Last Modified: Tue, 17 Aug 2021 18:58:36 GMT  
		Size: 10.1 MB (10131795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3262ebab7c98d109ec1bd6950016290289c265df653aaa167af1e363254f99`  
		Last Modified: Tue, 17 Aug 2021 18:58:36 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jre11`

```console
$ docker pull jetty@sha256:cf6fab1e124bd172a99cc5f444998004c39009b9a7a85e07b2071ed4da282f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4.43-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:6827ba260cce1694cc8966a4227b91cf8e85c8e8a1f5e596b6c381fe05937c26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130515617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:122bf720dd9c7858c8c32903c6bae77f6abc6f6303ee936b2acc24873c45b7d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:36:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 13:36:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:36:47 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:36:48 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:36:48 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 13:36:54 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:59:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:59:16 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:59:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:59:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 06:59:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:59:23 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:59:23 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:59:23 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:59:23 GMT
USER jetty
# Fri, 23 Jul 2021 06:59:23 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:59:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:59:24 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4a4d63704982a336f8cf6aae3cb36289ab6cbb2928c25a41a5d5adcbc5368`  
		Last Modified: Thu, 22 Jul 2021 13:49:56 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6172f170f291e20ff4db4b3892e4444242091b4b12f5fe9e785b4fd2870d6`  
		Last Modified: Thu, 22 Jul 2021 13:50:02 GMT  
		Size: 46.9 MB (46864013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2267fb349bf26ba4686e70a5917aab61dd091d637a4b86527b3d70c702f65e52`  
		Last Modified: Fri, 23 Jul 2021 07:05:05 GMT  
		Size: 9.9 MB (9853046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04c9a88beab783b8a9b0eb8738064e51779c80c738a9c0cc7cad8b164ecd665`  
		Last Modified: Fri, 23 Jul 2021 07:05:04 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4.43-jre11` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:1a07c17ad9c475e8c3ab89b9f648c08f76ef5578620e1d7bc51810a447586706
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128192433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37af330e0ffc0944c8ea84b25cd17b5efc19878eff9f20254251d0e52511eee8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 05:19:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 05:19:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Thu, 22 Jul 2021 05:19:58 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 05:19:58 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 05:19:58 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 05:19:59 GMT
ENV JAVA_VERSION=11.0.12
# Thu, 22 Jul 2021 05:20:09 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 22 Jul 2021 21:18:31 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 22 Jul 2021 21:18:31 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 22 Jul 2021 21:18:32 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 21:18:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 22 Jul 2021 21:18:32 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 22 Jul 2021 21:18:39 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 22 Jul 2021 21:18:39 GMT
WORKDIR /var/lib/jetty
# Thu, 22 Jul 2021 21:18:39 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 22 Jul 2021 21:18:39 GMT
USER jetty
# Thu, 22 Jul 2021 21:18:40 GMT
EXPOSE 8080
# Thu, 22 Jul 2021 21:18:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 22 Jul 2021 21:18:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b2c9f5cef9708e735967f5de94f32003e308811f5df8fa33e09517ebeb7ae5`  
		Last Modified: Thu, 22 Jul 2021 05:37:44 GMT  
		Size: 5.5 MB (5505472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98e2e88ae1dedf4258ab2fab5534ce7eb7bca1bcb94c42355ea79adb5dad107`  
		Last Modified: Thu, 22 Jul 2021 05:37:43 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b704173261f5be427cc946401c131da901ac5a7638e1521c1a4f7b539713e0`  
		Last Modified: Thu, 22 Jul 2021 05:37:50 GMT  
		Size: 45.9 MB (45930931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2822e39998d3f07ebd834f24d834323207c8557ae0e77f81d3e741fecf067fc`  
		Last Modified: Thu, 22 Jul 2021 21:19:21 GMT  
		Size: 9.9 MB (9853022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef13c62a343e3f2198fb56261650aa26eced41edd55a0362203e4e3419ab207`  
		Last Modified: Thu, 22 Jul 2021 21:19:20 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jre11-slim`

```console
$ docker pull jetty@sha256:f971551cf97a446fca1d91206a7fabf7a1a3a715dd0e2a0c172a82e7c9609401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4.43-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:4a695365926694c5c74786f856b308b82f0b1ab7c4662d601e34ce02f051977f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87686770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17065f0194a09cd5ab90dbda54124cc7708649ae8bf37894d26b3e5f01a49a31`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:54:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:54:45 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:54:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:54:45 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:54:45 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:55:30 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:52:27 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:52:28 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:52:28 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:52:28 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:52:29 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:52:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:52:51 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:52:52 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:52:52 GMT
USER jetty
# Tue, 17 Aug 2021 18:52:53 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:52:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:52:53 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea848f5155d0f648fc7fd258de1ce56d16d1ab42c2745a55e8adf26f997b45b`  
		Last Modified: Tue, 17 Aug 2021 07:02:46 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663bffc94428db61042052aaa00b98a379ea871642fce53bdc8ac9e06754493b`  
		Last Modified: Tue, 17 Aug 2021 07:03:45 GMT  
		Size: 47.1 MB (47137229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8210a578564c3c97979e60d07ed2430cf8a7c2de433a65067122f9353769bb92`  
		Last Modified: Tue, 17 Aug 2021 18:57:30 GMT  
		Size: 10.1 MB (10133127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05254c4841fdd3f3309b9f28e1c7e5b268e7a428854ac19f533e8eeda906abf0`  
		Last Modified: Tue, 17 Aug 2021 18:57:29 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4.43-jre11-slim` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:5cef81d40cbe6163a12ebeb795a685f82c4bf764631393beff62304ea7d679d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85372141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a0c6ecf89566c6b645cf35217655eb66ea2960196c5cba22ed89b1a681a0a23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:04:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:06:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Tue, 17 Aug 2021 06:06:39 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:06:39 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:06:40 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:06:40 GMT
ENV JAVA_VERSION=11.0.12
# Tue, 17 Aug 2021 06:07:40 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_x64_linux_11.0.12_7.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.12%2B7/OpenJDK11U-jre_aarch64_linux_11.0.12_7.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		java --version
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 15:06:32 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 15:06:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 15:06:33 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 15:06:51 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 15:06:52 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 15:06:52 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 15:06:52 GMT
USER jetty
# Tue, 17 Aug 2021 15:06:52 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 15:06:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 15:06:53 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a27af984eefbe6b82ccb775aead56e92f82cf16d079218087ebe132125cf5`  
		Last Modified: Tue, 17 Aug 2021 06:15:41 GMT  
		Size: 3.1 MB (3118861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d1ea50abf433035bb7f308b855f144aefbbe47ce996fb9e38d8db45df6f75a`  
		Last Modified: Tue, 17 Aug 2021 06:19:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c588b82388c8608ec757f28fdb2010018e105b0185377e9760686d75bd84720`  
		Last Modified: Tue, 17 Aug 2021 06:20:31 GMT  
		Size: 46.2 MB (46203534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056e07629bcce0ced329e35409d5406df7623ca76bf56dfef1e3f71952df97d`  
		Last Modified: Tue, 17 Aug 2021 15:07:22 GMT  
		Size: 10.1 MB (10133016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044aff060f3fb8a334183198c9f35c91ea523124b8d90babecc28c292694f0f8`  
		Last Modified: Tue, 17 Aug 2021 15:07:21 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jre8`

```console
$ docker pull jetty@sha256:56d4d91f1f9daeff0dacd6eed8a0d0a450613023ec6816ffe8dbe681c8db4ec0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:bf04496737ae44e7da2ecad5693c72be892efe8c80366247e28f02c6131c70b8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125018714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d7967e0f56907792b8367c25e9ca8b53d1dcafccfce130d28a1e86f65cdd19`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 13:36:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 13:38:02 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 22 Jul 2021 13:38:04 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 22 Jul 2021 13:38:04 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 13:38:05 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 13:38:05 GMT
ENV JAVA_VERSION=8u302
# Thu, 22 Jul 2021 13:38:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 23 Jul 2021 06:59:49 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:59:49 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Fri, 23 Jul 2021 06:59:50 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 23 Jul 2021 06:59:56 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 23 Jul 2021 06:59:57 GMT
WORKDIR /var/lib/jetty
# Fri, 23 Jul 2021 06:59:57 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Fri, 23 Jul 2021 06:59:57 GMT
USER jetty
# Fri, 23 Jul 2021 06:59:57 GMT
EXPOSE 8080
# Fri, 23 Jul 2021 06:59:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 06:59:58 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1bd03ef7cfc65ee7ed4ffabaaf72554688a2b5f72e917bcef6370793266e3d`  
		Last Modified: Thu, 22 Jul 2021 13:49:54 GMT  
		Size: 5.5 MB (5531107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c592a76c30927333261ac9d904569c09f8e7b70da35a852e24987a04e88087ae`  
		Last Modified: Thu, 22 Jul 2021 13:52:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c3d312a2dffe0c8bd467709d890ffe0d40c4ec2bc6f92950429f5dcc6b795`  
		Last Modified: Thu, 22 Jul 2021 13:52:07 GMT  
		Size: 41.4 MB (41367112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01f4546f4bef5b9e49314eddaec771f078092e15b64d89d8a1d85f8ecf43cee`  
		Last Modified: Fri, 23 Jul 2021 07:05:34 GMT  
		Size: 9.9 MB (9853043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db6cd19bd4107bf79cf93a9151642f3a7810705b86e34aa1410e22f87ef19c1`  
		Last Modified: Fri, 23 Jul 2021 07:05:33 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.43-jre8-slim`

```console
$ docker pull jetty@sha256:bbb98db45282ee782f609c963da7c16804442930f1a84adc7ccfb142e5382627
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9.4.43-jre8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:72df872a30764ac5438812cbe874e6ada4a249476071679544780a57d1b60404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82190701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46d955a50d999b225c136eb7b8f0e2d26530bfae3f59461b8a446d6b72d377bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 06:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 06:55:46 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 17 Aug 2021 06:55:46 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 17 Aug 2021 06:55:47 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 06:55:47 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 06:55:47 GMT
ENV JAVA_VERSION=8u302
# Tue, 17 Aug 2021 06:56:21 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 17 Aug 2021 18:53:01 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Tue, 17 Aug 2021 18:53:02 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 17 Aug 2021 18:53:02 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 17 Aug 2021 18:53:02 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 17 Aug 2021 18:53:03 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 18:53:03 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Tue, 17 Aug 2021 18:53:03 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 17 Aug 2021 18:53:28 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 17 Aug 2021 18:53:28 GMT
WORKDIR /var/lib/jetty
# Tue, 17 Aug 2021 18:53:29 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Tue, 17 Aug 2021 18:53:29 GMT
USER jetty
# Tue, 17 Aug 2021 18:53:29 GMT
EXPOSE 8080
# Tue, 17 Aug 2021 18:53:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:53:30 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427b7134c0c7b2e1d9cc703e20a84b850cbbf34ef654cfa0db710678a99da78b`  
		Last Modified: Tue, 17 Aug 2021 07:00:00 GMT  
		Size: 3.3 MB (3268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3ca35fb9a4f8f161dc8b1007db271091ce462aa5a6c8aada7e7096f9857b5`  
		Last Modified: Tue, 17 Aug 2021 07:04:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:684a63cea6ad88087bcbba64a242772c2e579702d67656a067619cf4691f0a09`  
		Last Modified: Tue, 17 Aug 2021 07:04:50 GMT  
		Size: 41.6 MB (41641133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbd0b203fe0500696e5f56d54442302307654fb62a304b6d663157d33c00744`  
		Last Modified: Tue, 17 Aug 2021 18:57:46 GMT  
		Size: 10.1 MB (10133156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a934241f4124a75ff57a59dc52f576e4ad66e947be5e190d844c6f4a0c1de683`  
		Last Modified: Tue, 17 Aug 2021 18:57:45 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:jdk16`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:jdk16` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:latest`

```console
$ docker pull jetty@sha256:e8b0525c9e2ca4cf96b5d8ff6fc9b4be0d60fe85b3a46484340c05e86ebccb6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:latest` - linux; amd64

```console
$ docker pull jetty@sha256:359f06940cd0a5fbbcf8c3ef5ed3eaf220c609b1da672988dd5585853b6be16c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250191857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0133201d9d213a20c744ae24c8d4c8c3867cc747e5e394b16da1b84f3f8aa3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 12 Aug 2021 19:20:55 GMT
ADD file:ab982d6f37710c434f7ef9650c722d3c6333906cbb9344bf91e79068088bcc69 in / 
# Thu, 12 Aug 2021 19:20:56 GMT
CMD ["/bin/bash"]
# Thu, 12 Aug 2021 19:37:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 12 Aug 2021 19:38:51 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 19:38:51 GMT
ENV LANG=C.UTF-8
# Thu, 12 Aug 2021 19:38:51 GMT
ENV JAVA_VERSION=16.0.2
# Thu, 12 Aug 2021 19:39:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Aug 2021 19:39:02 GMT
CMD ["jshell"]
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 12 Aug 2021 20:05:07 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 12 Aug 2021 20:05:08 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 12 Aug 2021 20:05:15 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 12 Aug 2021 20:05:15 GMT
WORKDIR /var/lib/jetty
# Thu, 12 Aug 2021 20:05:15 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 12 Aug 2021 20:05:15 GMT
USER jetty
# Thu, 12 Aug 2021 20:05:15 GMT
EXPOSE 8080
# Thu, 12 Aug 2021 20:05:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Aug 2021 20:05:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:c67289558ae5eb060942db5bf46d182448587a87e21c680a0486b147d4b9a0b4`  
		Last Modified: Thu, 12 Aug 2021 19:22:09 GMT  
		Size: 42.2 MB (42158041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12787f1f3888c64bfc9e779a9705ecc45ae1a60b3757074b6f16cf1d8553cac8`  
		Last Modified: Thu, 12 Aug 2021 19:43:29 GMT  
		Size: 13.4 MB (13373335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bd18e93178b3f1f6de8509b634da7edc7b3c3f556919bc74ebf9cf26011d43`  
		Last Modified: Thu, 12 Aug 2021 19:45:13 GMT  
		Size: 184.8 MB (184807071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4b89617f55aa177023a4af89615f954efbd45d84af54005e682b07a650daf`  
		Last Modified: Thu, 12 Aug 2021 20:07:06 GMT  
		Size: 9.9 MB (9851961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2936885a60136564c1831f496c5e66d274b41c98e9f706d79cfbfea181ff6531`  
		Last Modified: Thu, 12 Aug 2021 20:07:05 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
