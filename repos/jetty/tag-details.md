<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `jetty`

-	[`jetty:9`](#jetty9)
-	[`jetty:9.2.29-jre8`](#jetty9229-jre8)
-	[`jetty:9.2-jre8`](#jetty92-jre8)
-	[`jetty:9.3.28-jre8`](#jetty9328-jre8)
-	[`jetty:9.3-jre8`](#jetty93-jre8)
-	[`jetty:9.4`](#jetty94)
-	[`jetty:9.4.26`](#jetty9426)
-	[`jetty:9.4.26-jdk13`](#jetty9426-jdk13)
-	[`jetty:9.4.26-jdk13-slim`](#jetty9426-jdk13-slim)
-	[`jetty:9.4.26-jre11`](#jetty9426-jre11)
-	[`jetty:9.4.26-jre11-slim`](#jetty9426-jre11-slim)
-	[`jetty:9.4.26-jre8`](#jetty9426-jre8)
-	[`jetty:9.4-jdk13`](#jetty94-jdk13)
-	[`jetty:9.4-jdk13-slim`](#jetty94-jdk13-slim)
-	[`jetty:9.4-jre11`](#jetty94-jre11)
-	[`jetty:9.4-jre11-slim`](#jetty94-jre11-slim)
-	[`jetty:9.4-jre8`](#jetty94-jre8)
-	[`jetty:9-jdk13`](#jetty9-jdk13)
-	[`jetty:9-jdk13-slim`](#jetty9-jdk13-slim)
-	[`jetty:9-jre11`](#jetty9-jre11)
-	[`jetty:9-jre11-slim`](#jetty9-jre11-slim)
-	[`jetty:9-jre8`](#jetty9-jre8)
-	[`jetty:jdk13`](#jettyjdk13)
-	[`jetty:latest`](#jettylatest)

## `jetty:9`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.2.29-jre8`

```console
$ docker pull jetty@sha256:f194ae4e217f73bed520b98e4d3657aebbb855a580690dfb109f8a7eb5525430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.2.29-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:0d0984ac7c37ccecc194dab77719b50c84550ba0de6e7fba0a9d7be88f177870
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127753154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e65bc50d0e7c5952db2fe398c156aa4418f3875e1343744ffd1cb2cec20e02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:57 GMT
ENV JETTY_VERSION=9.2.29.v20191105
# Fri, 07 Feb 2020 03:31:57 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:58 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:58 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.2.29.v20191105/jetty-distribution-9.2.29.v20191105.tar.gz
# Fri, 07 Feb 2020 03:31:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:32:04 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 07 Feb 2020 03:32:04 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:32:05 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:32:05 GMT
USER jetty
# Fri, 07 Feb 2020 03:32:05 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:32:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:32:06 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e419f66ae5174c3c0f5bc3609ea19b43b72cb93293c2a071df2d0ad7d81c7bcc`  
		Last Modified: Fri, 07 Feb 2020 03:33:53 GMT  
		Size: 13.8 MB (13846890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab49d6520674a2d9c23070f08c21d99a27ed37c57c32e24c78c68acab5fb804`  
		Last Modified: Fri, 07 Feb 2020 03:33:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.2-jre8`

```console
$ docker pull jetty@sha256:f194ae4e217f73bed520b98e4d3657aebbb855a580690dfb109f8a7eb5525430
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.2-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:0d0984ac7c37ccecc194dab77719b50c84550ba0de6e7fba0a9d7be88f177870
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127753154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e65bc50d0e7c5952db2fe398c156aa4418f3875e1343744ffd1cb2cec20e02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:57 GMT
ENV JETTY_VERSION=9.2.29.v20191105
# Fri, 07 Feb 2020 03:31:57 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:58 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:58 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.2.29.v20191105/jetty-distribution-9.2.29.v20191105.tar.gz
# Fri, 07 Feb 2020 03:31:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:32:04 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 07 Feb 2020 03:32:04 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:32:05 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:32:05 GMT
USER jetty
# Fri, 07 Feb 2020 03:32:05 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:32:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:32:06 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e419f66ae5174c3c0f5bc3609ea19b43b72cb93293c2a071df2d0ad7d81c7bcc`  
		Last Modified: Fri, 07 Feb 2020 03:33:53 GMT  
		Size: 13.8 MB (13846890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab49d6520674a2d9c23070f08c21d99a27ed37c57c32e24c78c68acab5fb804`  
		Last Modified: Fri, 07 Feb 2020 03:33:48 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.3.28-jre8`

```console
$ docker pull jetty@sha256:5764ee83e5d1883791525985bbdf21743bfbb6144a531b6c479690f8510e67f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.3.28-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:d9b1d4baacb1179cfe364d5050263f9fb3a02e9f67b7c3eb9b3b50a9f8fac715
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131648042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992401304be7488f22a8e8f0293fbc3785791ba4b3b9cc7e80c22db0d24d1290`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:41 GMT
ENV JETTY_VERSION=9.3.28.v20191105
# Fri, 07 Feb 2020 03:31:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:42 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:42 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:42 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:43 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.3.28.v20191105/jetty-distribution-9.3.28.v20191105.tar.gz
# Fri, 07 Feb 2020 03:31:43 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:49 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 07 Feb 2020 03:31:49 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:50 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:50 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:50 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:51 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3935c8de6542cd7600d4a4e305f1b014175391c21e65d8dbbf80fa8ba1a69b5`  
		Last Modified: Fri, 07 Feb 2020 03:33:43 GMT  
		Size: 17.7 MB (17741777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614595d66f444d3a99859f3c878e8770dc912e6b7eb1908d0299f0a5c80fb1c7`  
		Last Modified: Fri, 07 Feb 2020 03:33:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.3-jre8`

```console
$ docker pull jetty@sha256:5764ee83e5d1883791525985bbdf21743bfbb6144a531b6c479690f8510e67f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.3-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:d9b1d4baacb1179cfe364d5050263f9fb3a02e9f67b7c3eb9b3b50a9f8fac715
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131648042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992401304be7488f22a8e8f0293fbc3785791ba4b3b9cc7e80c22db0d24d1290`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:41 GMT
ENV JETTY_VERSION=9.3.28.v20191105
# Fri, 07 Feb 2020 03:31:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:42 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:42 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:42 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:43 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.3.28.v20191105/jetty-distribution-9.3.28.v20191105.tar.gz
# Fri, 07 Feb 2020 03:31:43 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:49 GMT
RUN set -xe 	&& mkdir /jetty-keys         && export GNUPGHOME=/jetty-keys;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done 	&& mkdir -p "$JETTY_HOME" 	&& cd $JETTY_HOME 	&& curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz 	&& curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc 	&& gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz 	&& tar -xvf jetty.tar.gz --strip-components=1 	&& sed -i '/jetty-logging/d' etc/jetty.conf 	&& rm -fr jetty.tar.gz* 	&& mkdir -p "$JETTY_BASE" 	&& cd $JETTY_BASE 	&& modules="$(grep -- ^--module= "$JETTY_HOME/start.ini" | cut -d= -f2 | paste -d, -s)" 	&& java -jar "$JETTY_HOME/start.jar" --add-to-startd="$modules" 	&& mkdir -p "$TMPDIR" 	&& groupadd -r jetty && useradd -r -g jetty jetty 	&& chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" 	&& rm -rf /tmp/hsperfdata_root
# Fri, 07 Feb 2020 03:31:49 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:50 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:50 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:50 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:51 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3935c8de6542cd7600d4a4e305f1b014175391c21e65d8dbbf80fa8ba1a69b5`  
		Last Modified: Fri, 07 Feb 2020 03:33:43 GMT  
		Size: 17.7 MB (17741777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614595d66f444d3a99859f3c878e8770dc912e6b7eb1908d0299f0a5c80fb1c7`  
		Last Modified: Fri, 07 Feb 2020 03:33:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.26`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4.26` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.26-jdk13`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4.26-jdk13` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.26-jdk13-slim`

```console
$ docker pull jetty@sha256:e4998d26d9d99541ff2aac2c9aeeb652d2261f937b9a35ac90465787bad5e70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4.26-jdk13-slim` - linux; amd64

```console
$ docker pull jetty@sha256:58158817c89337b2d6b94c5e5587f344547d1dae6be487bff21c1c28bc1df6e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236901291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4712a90fa46ac89985ac544a62fe6be657a08c1dce18337942e50291d9e98ca8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:25:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Sun, 02 Feb 2020 06:25:33 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:25:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_VERSION=13.0.2
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Sun, 02 Feb 2020 06:25:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:25:51 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:26:24 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV TMPDIR=/tmp/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Sun, 02 Feb 2020 21:26:38 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sun, 02 Feb 2020 21:26:39 GMT
WORKDIR /var/lib/jetty
# Sun, 02 Feb 2020 21:26:39 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Sun, 02 Feb 2020 21:26:39 GMT
USER jetty
# Sun, 02 Feb 2020 21:26:39 GMT
EXPOSE 8080
# Sun, 02 Feb 2020 21:26:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:26:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e615298152110cce920a0c9a2fee428cf50d77f2dd7fee4bc9e6aab96b3cd3`  
		Last Modified: Sun, 02 Feb 2020 06:34:28 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485e6161e84f226468239fee43881f9eee91c8008dcf21994bf0caf5e10ced9f`  
		Last Modified: Sun, 02 Feb 2020 06:34:55 GMT  
		Size: 196.7 MB (196675123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862739cc0ededd04d3cd4cef2ec210375d5b097a0b7e70f88d30c29e7771c95c`  
		Last Modified: Sun, 02 Feb 2020 21:27:35 GMT  
		Size: 9.9 MB (9883172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a629581c8f2594275309898a017b2497b90e9873fdb051829a8ff738c2398a5a`  
		Last Modified: Sun, 02 Feb 2020 21:27:34 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.26-jre11`

```console
$ docker pull jetty@sha256:6e49543d532dad941621a2991584c4f4914e8891bc54f8ca66e61f6f64d447fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4.26-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:c7aca2d93edd4d2266fbce3345046abcfc684fac05d7c7ae228fb62c042d0544
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125216930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaed0e4cbc8435dcd317dc869328f7ef52856e902e968520402610b166dd2bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:51:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 07 Feb 2020 01:51:11 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:51:13 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:51:13 GMT
ENV JAVA_VERSION=11.0.6
# Fri, 07 Feb 2020 01:51:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Fri, 07 Feb 2020 01:51:16 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Fri, 07 Feb 2020 01:51:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 07 Feb 2020 03:31:00 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Fri, 07 Feb 2020 03:31:00 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Fri, 07 Feb 2020 03:31:02 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:09 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 07 Feb 2020 03:31:09 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:10 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:10 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:10 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ac43bf1999125c26619f5c7cdcbf57c2fbe8887f057fe7d2f930537020cca`  
		Last Modified: Fri, 07 Feb 2020 01:58:04 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9599f5be1d383c74e1a8eaadcfbf7eed9b76337b4d11eb231bdab3694577ccbb`  
		Last Modified: Fri, 07 Feb 2020 01:58:14 GMT  
		Size: 41.9 MB (41894421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afd3bf31834cc7078ce8643ff858f0c8bc130e4b5872ac0430908592b29475`  
		Last Modified: Fri, 07 Feb 2020 03:32:49 GMT  
		Size: 9.6 MB (9603865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddcc2b6e1cdba0c9693d77eda9511058539c51bc6abeb01a43d8fb61622611e`  
		Last Modified: Fri, 07 Feb 2020 03:32:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4.26-jre11` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:5c2178da1b41a9de41c3c78271bc106d1df210d7cec32583b21d9a806bec5e1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122941895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871122cb6d38edf4988a9587f9a4e9af65119cbb7c8efd47cf7811a36590f459`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:50:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 14:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:57:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Feb 2020 14:57:59 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:58:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 26 Feb 2020 14:58:02 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 26 Feb 2020 14:58:03 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Wed, 26 Feb 2020 14:58:04 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 26 Feb 2020 14:58:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 27 Feb 2020 03:33:56 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Thu, 27 Feb 2020 03:33:56 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 27 Feb 2020 03:33:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 27 Feb 2020 03:33:58 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 27 Feb 2020 03:33:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 03:33:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Thu, 27 Feb 2020 03:33:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Thu, 27 Feb 2020 03:34:07 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 27 Feb 2020 03:34:08 GMT
WORKDIR /var/lib/jetty
# Thu, 27 Feb 2020 03:34:08 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Thu, 27 Feb 2020 03:34:09 GMT
USER jetty
# Thu, 27 Feb 2020 03:34:10 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 03:34:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 03:34:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f1ca8932d9ee1727375561698745fa548546f609956c4aca9fed0b48d41a1`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 7.7 MB (7681467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88425686f799f708ae776f78a6d01c179a52f55fc5b32de874db3c4ace2dd156`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 10.0 MB (9983767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509378047990c01dee0d00b6e45e3afa840f5f282b462298b73b8004cfbc80ed`  
		Last Modified: Wed, 26 Feb 2020 15:00:52 GMT  
		Size: 5.5 MB (5504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d62e5f5f1132320fdf5923d2468714d0ad0b037c69d870b6dcaaa46fa190e`  
		Last Modified: Wed, 26 Feb 2020 15:00:50 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009563b0d5b3cf85d035a1f2b1dd87a74c8d0edc1e5393db879e94ce82ae453`  
		Last Modified: Wed, 26 Feb 2020 15:01:03 GMT  
		Size: 41.0 MB (40996671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be07dfcba0717f823b012edd7bccf16e052abc403c09e782ff111810b1c457`  
		Last Modified: Thu, 27 Feb 2020 03:34:32 GMT  
		Size: 9.6 MB (9603996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fb972800f6b822bf03d3f0cc6d7f8b9dfbc181c284ce4846df581433cf4b8f`  
		Last Modified: Thu, 27 Feb 2020 03:34:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.26-jre11-slim`

```console
$ docker pull jetty@sha256:fd306b8a2c9b3120c40c2522a7af4c366433a691df6538cd6b124d68bec0f341
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4.26-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:88d5a4ae6845f34b4c3a1c7d184035fabee5092c2702853dfdf7ad1c7ca55427
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82400297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01cd9382621735125e80f09d9c0b896d68030cf6c2c531249b98aab2d19805c2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:26:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sun, 02 Feb 2020 06:26:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:26:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:26:41 GMT
ENV JAVA_VERSION=11.0.6
# Sun, 02 Feb 2020 06:27:49 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Sun, 02 Feb 2020 06:27:49 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Sun, 02 Feb 2020 06:28:07 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV TMPDIR=/tmp/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 21:25:42 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Sun, 02 Feb 2020 21:25:42 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Sun, 02 Feb 2020 21:25:56 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sun, 02 Feb 2020 21:25:56 GMT
WORKDIR /var/lib/jetty
# Sun, 02 Feb 2020 21:25:57 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Sun, 02 Feb 2020 21:25:57 GMT
USER jetty
# Sun, 02 Feb 2020 21:25:57 GMT
EXPOSE 8080
# Sun, 02 Feb 2020 21:25:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:25:57 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4d10a782b71ea3c226ce20c1acdfb0aeefb137fb5c5fa3100aaa275ec71cd`  
		Last Modified: Sun, 02 Feb 2020 06:35:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db4424ff27024b682967e5ca869ba018b8667fdc7cbd2718db9ebba95c5e601`  
		Last Modified: Sun, 02 Feb 2020 06:36:47 GMT  
		Size: 42.2 MB (42172493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90391924a5e59bc44cf9ef90cb0f0abca2acffc23e923d1cb39caa67252de309`  
		Last Modified: Sun, 02 Feb 2020 21:27:20 GMT  
		Size: 9.9 MB (9884807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c397836cf4ec5aae02b21743025e7e579fa7f8a73966311e0b3ff9afb4eab7a4`  
		Last Modified: Sun, 02 Feb 2020 21:27:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4.26-jre11-slim` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:3ae1ed5d8853996490ad156f6fbbce9ff1eadc30e3bd6c372ca3fbb635faf5a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80110979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3797cc47ed14b3f0d8c4b426d77be25adfba151f44c1f38c835a2565a1073d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:56:44 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:56:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Feb 2020 14:56:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:56:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 26 Feb 2020 14:56:48 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 26 Feb 2020 14:58:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Wed, 26 Feb 2020 14:58:22 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 26 Feb 2020 14:58:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 27 Feb 2020 03:33:08 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Thu, 27 Feb 2020 03:33:09 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 27 Feb 2020 03:33:09 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 27 Feb 2020 03:33:10 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 27 Feb 2020 03:33:11 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 03:33:11 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Thu, 27 Feb 2020 03:33:12 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Thu, 27 Feb 2020 03:33:45 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 27 Feb 2020 03:33:45 GMT
WORKDIR /var/lib/jetty
# Thu, 27 Feb 2020 03:33:46 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Thu, 27 Feb 2020 03:33:47 GMT
USER jetty
# Thu, 27 Feb 2020 03:33:47 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 03:33:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 03:33:49 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa702e5900f7e9b9cc9f5827bff3c63c77b495471757e961459c43e338147a`  
		Last Modified: Wed, 26 Feb 2020 15:00:01 GMT  
		Size: 3.1 MB (3101218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b200df05fed1b744d2e15b2ec347e0774604f6b6f8073c708edf529bba593b`  
		Last Modified: Wed, 26 Feb 2020 15:00:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15600e576d9b8eed5a2f6ecab52d8fc99bae589a21c82c26d9c6648486d488a`  
		Last Modified: Wed, 26 Feb 2020 15:01:25 GMT  
		Size: 41.3 MB (41271650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3654953d70524aca1a86522276d777bd7ecce623e55fbd2df88f061efa3ce5a0`  
		Last Modified: Thu, 27 Feb 2020 03:34:24 GMT  
		Size: 9.9 MB (9884922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd14054f6eed9929490dbecbc97ab84a6db8e227508185fb9a6b99f031262d4`  
		Last Modified: Thu, 27 Feb 2020 03:34:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4.26-jre8`

```console
$ docker pull jetty@sha256:3c43dbfe7d459e3b07bbdbd7836fc4c113c65abbd60c6cc70ed619e9aa4953bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4.26-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:38ba1d9e3e0aa0df06ca9a9381d2aee4c87c3df11683e7faa2de866d84229a1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123510115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fef4f0fb08f9ba16a07d92ffcaf15978adde6e3ff5621939db1e138dcb9054d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:17 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:17 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:17 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Fri, 07 Feb 2020 03:31:18 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:24 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 07 Feb 2020 03:31:24 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:25 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:25 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:25 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:26 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7534a779acb5cde730e4dc712e3b6dabc8557f6bb43b153144dc5477a4a053e4`  
		Last Modified: Fri, 07 Feb 2020 03:33:12 GMT  
		Size: 9.6 MB (9603852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d3d1f3ae6adfd2ddce30430fcb3156f0e6d8670e6b680865c7e690955b4b50`  
		Last Modified: Fri, 07 Feb 2020 03:32:55 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk13`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4-jdk13` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jdk13-slim`

```console
$ docker pull jetty@sha256:e4998d26d9d99541ff2aac2c9aeeb652d2261f937b9a35ac90465787bad5e70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4-jdk13-slim` - linux; amd64

```console
$ docker pull jetty@sha256:58158817c89337b2d6b94c5e5587f344547d1dae6be487bff21c1c28bc1df6e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236901291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4712a90fa46ac89985ac544a62fe6be657a08c1dce18337942e50291d9e98ca8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:25:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Sun, 02 Feb 2020 06:25:33 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:25:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_VERSION=13.0.2
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Sun, 02 Feb 2020 06:25:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:25:51 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:26:24 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV TMPDIR=/tmp/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Sun, 02 Feb 2020 21:26:38 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sun, 02 Feb 2020 21:26:39 GMT
WORKDIR /var/lib/jetty
# Sun, 02 Feb 2020 21:26:39 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Sun, 02 Feb 2020 21:26:39 GMT
USER jetty
# Sun, 02 Feb 2020 21:26:39 GMT
EXPOSE 8080
# Sun, 02 Feb 2020 21:26:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:26:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e615298152110cce920a0c9a2fee428cf50d77f2dd7fee4bc9e6aab96b3cd3`  
		Last Modified: Sun, 02 Feb 2020 06:34:28 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485e6161e84f226468239fee43881f9eee91c8008dcf21994bf0caf5e10ced9f`  
		Last Modified: Sun, 02 Feb 2020 06:34:55 GMT  
		Size: 196.7 MB (196675123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862739cc0ededd04d3cd4cef2ec210375d5b097a0b7e70f88d30c29e7771c95c`  
		Last Modified: Sun, 02 Feb 2020 21:27:35 GMT  
		Size: 9.9 MB (9883172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a629581c8f2594275309898a017b2497b90e9873fdb051829a8ff738c2398a5a`  
		Last Modified: Sun, 02 Feb 2020 21:27:34 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre11`

```console
$ docker pull jetty@sha256:6e49543d532dad941621a2991584c4f4914e8891bc54f8ca66e61f6f64d447fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:c7aca2d93edd4d2266fbce3345046abcfc684fac05d7c7ae228fb62c042d0544
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125216930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaed0e4cbc8435dcd317dc869328f7ef52856e902e968520402610b166dd2bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:51:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 07 Feb 2020 01:51:11 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:51:13 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:51:13 GMT
ENV JAVA_VERSION=11.0.6
# Fri, 07 Feb 2020 01:51:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Fri, 07 Feb 2020 01:51:16 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Fri, 07 Feb 2020 01:51:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 07 Feb 2020 03:31:00 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Fri, 07 Feb 2020 03:31:00 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Fri, 07 Feb 2020 03:31:02 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:09 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 07 Feb 2020 03:31:09 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:10 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:10 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:10 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ac43bf1999125c26619f5c7cdcbf57c2fbe8887f057fe7d2f930537020cca`  
		Last Modified: Fri, 07 Feb 2020 01:58:04 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9599f5be1d383c74e1a8eaadcfbf7eed9b76337b4d11eb231bdab3694577ccbb`  
		Last Modified: Fri, 07 Feb 2020 01:58:14 GMT  
		Size: 41.9 MB (41894421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afd3bf31834cc7078ce8643ff858f0c8bc130e4b5872ac0430908592b29475`  
		Last Modified: Fri, 07 Feb 2020 03:32:49 GMT  
		Size: 9.6 MB (9603865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddcc2b6e1cdba0c9693d77eda9511058539c51bc6abeb01a43d8fb61622611e`  
		Last Modified: Fri, 07 Feb 2020 03:32:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4-jre11` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:5c2178da1b41a9de41c3c78271bc106d1df210d7cec32583b21d9a806bec5e1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122941895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871122cb6d38edf4988a9587f9a4e9af65119cbb7c8efd47cf7811a36590f459`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:50:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 14:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:57:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Feb 2020 14:57:59 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:58:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 26 Feb 2020 14:58:02 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 26 Feb 2020 14:58:03 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Wed, 26 Feb 2020 14:58:04 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 26 Feb 2020 14:58:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 27 Feb 2020 03:33:56 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Thu, 27 Feb 2020 03:33:56 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 27 Feb 2020 03:33:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 27 Feb 2020 03:33:58 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 27 Feb 2020 03:33:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 03:33:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Thu, 27 Feb 2020 03:33:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Thu, 27 Feb 2020 03:34:07 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 27 Feb 2020 03:34:08 GMT
WORKDIR /var/lib/jetty
# Thu, 27 Feb 2020 03:34:08 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Thu, 27 Feb 2020 03:34:09 GMT
USER jetty
# Thu, 27 Feb 2020 03:34:10 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 03:34:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 03:34:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f1ca8932d9ee1727375561698745fa548546f609956c4aca9fed0b48d41a1`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 7.7 MB (7681467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88425686f799f708ae776f78a6d01c179a52f55fc5b32de874db3c4ace2dd156`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 10.0 MB (9983767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509378047990c01dee0d00b6e45e3afa840f5f282b462298b73b8004cfbc80ed`  
		Last Modified: Wed, 26 Feb 2020 15:00:52 GMT  
		Size: 5.5 MB (5504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d62e5f5f1132320fdf5923d2468714d0ad0b037c69d870b6dcaaa46fa190e`  
		Last Modified: Wed, 26 Feb 2020 15:00:50 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009563b0d5b3cf85d035a1f2b1dd87a74c8d0edc1e5393db879e94ce82ae453`  
		Last Modified: Wed, 26 Feb 2020 15:01:03 GMT  
		Size: 41.0 MB (40996671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be07dfcba0717f823b012edd7bccf16e052abc403c09e782ff111810b1c457`  
		Last Modified: Thu, 27 Feb 2020 03:34:32 GMT  
		Size: 9.6 MB (9603996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fb972800f6b822bf03d3f0cc6d7f8b9dfbc181c284ce4846df581433cf4b8f`  
		Last Modified: Thu, 27 Feb 2020 03:34:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre11-slim`

```console
$ docker pull jetty@sha256:fd306b8a2c9b3120c40c2522a7af4c366433a691df6538cd6b124d68bec0f341
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9.4-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:88d5a4ae6845f34b4c3a1c7d184035fabee5092c2702853dfdf7ad1c7ca55427
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82400297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01cd9382621735125e80f09d9c0b896d68030cf6c2c531249b98aab2d19805c2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:26:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sun, 02 Feb 2020 06:26:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:26:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:26:41 GMT
ENV JAVA_VERSION=11.0.6
# Sun, 02 Feb 2020 06:27:49 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Sun, 02 Feb 2020 06:27:49 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Sun, 02 Feb 2020 06:28:07 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV TMPDIR=/tmp/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 21:25:42 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Sun, 02 Feb 2020 21:25:42 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Sun, 02 Feb 2020 21:25:56 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sun, 02 Feb 2020 21:25:56 GMT
WORKDIR /var/lib/jetty
# Sun, 02 Feb 2020 21:25:57 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Sun, 02 Feb 2020 21:25:57 GMT
USER jetty
# Sun, 02 Feb 2020 21:25:57 GMT
EXPOSE 8080
# Sun, 02 Feb 2020 21:25:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:25:57 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4d10a782b71ea3c226ce20c1acdfb0aeefb137fb5c5fa3100aaa275ec71cd`  
		Last Modified: Sun, 02 Feb 2020 06:35:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db4424ff27024b682967e5ca869ba018b8667fdc7cbd2718db9ebba95c5e601`  
		Last Modified: Sun, 02 Feb 2020 06:36:47 GMT  
		Size: 42.2 MB (42172493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90391924a5e59bc44cf9ef90cb0f0abca2acffc23e923d1cb39caa67252de309`  
		Last Modified: Sun, 02 Feb 2020 21:27:20 GMT  
		Size: 9.9 MB (9884807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c397836cf4ec5aae02b21743025e7e579fa7f8a73966311e0b3ff9afb4eab7a4`  
		Last Modified: Sun, 02 Feb 2020 21:27:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9.4-jre11-slim` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:3ae1ed5d8853996490ad156f6fbbce9ff1eadc30e3bd6c372ca3fbb635faf5a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80110979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3797cc47ed14b3f0d8c4b426d77be25adfba151f44c1f38c835a2565a1073d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:56:44 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:56:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Feb 2020 14:56:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:56:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 26 Feb 2020 14:56:48 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 26 Feb 2020 14:58:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Wed, 26 Feb 2020 14:58:22 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 26 Feb 2020 14:58:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 27 Feb 2020 03:33:08 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Thu, 27 Feb 2020 03:33:09 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 27 Feb 2020 03:33:09 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 27 Feb 2020 03:33:10 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 27 Feb 2020 03:33:11 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 03:33:11 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Thu, 27 Feb 2020 03:33:12 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Thu, 27 Feb 2020 03:33:45 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 27 Feb 2020 03:33:45 GMT
WORKDIR /var/lib/jetty
# Thu, 27 Feb 2020 03:33:46 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Thu, 27 Feb 2020 03:33:47 GMT
USER jetty
# Thu, 27 Feb 2020 03:33:47 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 03:33:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 03:33:49 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa702e5900f7e9b9cc9f5827bff3c63c77b495471757e961459c43e338147a`  
		Last Modified: Wed, 26 Feb 2020 15:00:01 GMT  
		Size: 3.1 MB (3101218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b200df05fed1b744d2e15b2ec347e0774604f6b6f8073c708edf529bba593b`  
		Last Modified: Wed, 26 Feb 2020 15:00:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15600e576d9b8eed5a2f6ecab52d8fc99bae589a21c82c26d9c6648486d488a`  
		Last Modified: Wed, 26 Feb 2020 15:01:25 GMT  
		Size: 41.3 MB (41271650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3654953d70524aca1a86522276d777bd7ecce623e55fbd2df88f061efa3ce5a0`  
		Last Modified: Thu, 27 Feb 2020 03:34:24 GMT  
		Size: 9.9 MB (9884922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd14054f6eed9929490dbecbc97ab84a6db8e227508185fb9a6b99f031262d4`  
		Last Modified: Thu, 27 Feb 2020 03:34:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9.4-jre8`

```console
$ docker pull jetty@sha256:3c43dbfe7d459e3b07bbdbd7836fc4c113c65abbd60c6cc70ed619e9aa4953bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9.4-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:38ba1d9e3e0aa0df06ca9a9381d2aee4c87c3df11683e7faa2de866d84229a1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123510115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fef4f0fb08f9ba16a07d92ffcaf15978adde6e3ff5621939db1e138dcb9054d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:17 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:17 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:17 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Fri, 07 Feb 2020 03:31:18 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:24 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 07 Feb 2020 03:31:24 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:25 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:25 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:25 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:26 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7534a779acb5cde730e4dc712e3b6dabc8557f6bb43b153144dc5477a4a053e4`  
		Last Modified: Fri, 07 Feb 2020 03:33:12 GMT  
		Size: 9.6 MB (9603852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d3d1f3ae6adfd2ddce30430fcb3156f0e6d8670e6b680865c7e690955b4b50`  
		Last Modified: Fri, 07 Feb 2020 03:32:55 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk13`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9-jdk13` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jdk13-slim`

```console
$ docker pull jetty@sha256:e4998d26d9d99541ff2aac2c9aeeb652d2261f937b9a35ac90465787bad5e70d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9-jdk13-slim` - linux; amd64

```console
$ docker pull jetty@sha256:58158817c89337b2d6b94c5e5587f344547d1dae6be487bff21c1c28bc1df6e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236901291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4712a90fa46ac89985ac544a62fe6be657a08c1dce18337942e50291d9e98ca8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:25:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Sun, 02 Feb 2020 06:25:33 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:25:34 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_VERSION=13.0.2
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:25:34 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Sun, 02 Feb 2020 06:25:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:25:51 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:26:24 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV TMPDIR=/tmp/jetty
# Sun, 02 Feb 2020 21:26:25 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Sun, 02 Feb 2020 21:26:25 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Sun, 02 Feb 2020 21:26:38 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sun, 02 Feb 2020 21:26:39 GMT
WORKDIR /var/lib/jetty
# Sun, 02 Feb 2020 21:26:39 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Sun, 02 Feb 2020 21:26:39 GMT
USER jetty
# Sun, 02 Feb 2020 21:26:39 GMT
EXPOSE 8080
# Sun, 02 Feb 2020 21:26:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:26:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e615298152110cce920a0c9a2fee428cf50d77f2dd7fee4bc9e6aab96b3cd3`  
		Last Modified: Sun, 02 Feb 2020 06:34:28 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485e6161e84f226468239fee43881f9eee91c8008dcf21994bf0caf5e10ced9f`  
		Last Modified: Sun, 02 Feb 2020 06:34:55 GMT  
		Size: 196.7 MB (196675123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862739cc0ededd04d3cd4cef2ec210375d5b097a0b7e70f88d30c29e7771c95c`  
		Last Modified: Sun, 02 Feb 2020 21:27:35 GMT  
		Size: 9.9 MB (9883172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a629581c8f2594275309898a017b2497b90e9873fdb051829a8ff738c2398a5a`  
		Last Modified: Sun, 02 Feb 2020 21:27:34 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre11`

```console
$ docker pull jetty@sha256:6e49543d532dad941621a2991584c4f4914e8891bc54f8ca66e61f6f64d447fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9-jre11` - linux; amd64

```console
$ docker pull jetty@sha256:c7aca2d93edd4d2266fbce3345046abcfc684fac05d7c7ae228fb62c042d0544
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125216930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aaed0e4cbc8435dcd317dc869328f7ef52856e902e968520402610b166dd2bf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:51:11 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Fri, 07 Feb 2020 01:51:11 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:51:13 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:51:13 GMT
ENV JAVA_VERSION=11.0.6
# Fri, 07 Feb 2020 01:51:16 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Fri, 07 Feb 2020 01:51:16 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Fri, 07 Feb 2020 01:51:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Fri, 07 Feb 2020 03:31:00 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Fri, 07 Feb 2020 03:31:00 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:02 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Fri, 07 Feb 2020 03:31:02 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:09 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 07 Feb 2020 03:31:09 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:10 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:10 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:10 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ac43bf1999125c26619f5c7cdcbf57c2fbe8887f057fe7d2f930537020cca`  
		Last Modified: Fri, 07 Feb 2020 01:58:04 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9599f5be1d383c74e1a8eaadcfbf7eed9b76337b4d11eb231bdab3694577ccbb`  
		Last Modified: Fri, 07 Feb 2020 01:58:14 GMT  
		Size: 41.9 MB (41894421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2afd3bf31834cc7078ce8643ff858f0c8bc130e4b5872ac0430908592b29475`  
		Last Modified: Fri, 07 Feb 2020 03:32:49 GMT  
		Size: 9.6 MB (9603865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddcc2b6e1cdba0c9693d77eda9511058539c51bc6abeb01a43d8fb61622611e`  
		Last Modified: Fri, 07 Feb 2020 03:32:40 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9-jre11` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:5c2178da1b41a9de41c3c78271bc106d1df210d7cec32583b21d9a806bec5e1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122941895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871122cb6d38edf4988a9587f9a4e9af65119cbb7c8efd47cf7811a36590f459`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:50:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 14:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:57:57 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:57:58 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Feb 2020 14:57:59 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:58:02 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 26 Feb 2020 14:58:02 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 26 Feb 2020 14:58:03 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Wed, 26 Feb 2020 14:58:04 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 26 Feb 2020 14:58:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 27 Feb 2020 03:33:56 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Thu, 27 Feb 2020 03:33:56 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 27 Feb 2020 03:33:57 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 27 Feb 2020 03:33:58 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 27 Feb 2020 03:33:58 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 03:33:59 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Thu, 27 Feb 2020 03:33:59 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Thu, 27 Feb 2020 03:34:07 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 27 Feb 2020 03:34:08 GMT
WORKDIR /var/lib/jetty
# Thu, 27 Feb 2020 03:34:08 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Thu, 27 Feb 2020 03:34:09 GMT
USER jetty
# Thu, 27 Feb 2020 03:34:10 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 03:34:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 03:34:11 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f1ca8932d9ee1727375561698745fa548546f609956c4aca9fed0b48d41a1`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 7.7 MB (7681467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88425686f799f708ae776f78a6d01c179a52f55fc5b32de874db3c4ace2dd156`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 10.0 MB (9983767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509378047990c01dee0d00b6e45e3afa840f5f282b462298b73b8004cfbc80ed`  
		Last Modified: Wed, 26 Feb 2020 15:00:52 GMT  
		Size: 5.5 MB (5504391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d62e5f5f1132320fdf5923d2468714d0ad0b037c69d870b6dcaaa46fa190e`  
		Last Modified: Wed, 26 Feb 2020 15:00:50 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009563b0d5b3cf85d035a1f2b1dd87a74c8d0edc1e5393db879e94ce82ae453`  
		Last Modified: Wed, 26 Feb 2020 15:01:03 GMT  
		Size: 41.0 MB (40996671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42be07dfcba0717f823b012edd7bccf16e052abc403c09e782ff111810b1c457`  
		Last Modified: Thu, 27 Feb 2020 03:34:32 GMT  
		Size: 9.6 MB (9603996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fb972800f6b822bf03d3f0cc6d7f8b9dfbc181c284ce4846df581433cf4b8f`  
		Last Modified: Thu, 27 Feb 2020 03:34:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre11-slim`

```console
$ docker pull jetty@sha256:fd306b8a2c9b3120c40c2522a7af4c366433a691df6538cd6b124d68bec0f341
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9-jre11-slim` - linux; amd64

```console
$ docker pull jetty@sha256:88d5a4ae6845f34b4c3a1c7d184035fabee5092c2702853dfdf7ad1c7ca55427
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82400297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01cd9382621735125e80f09d9c0b896d68030cf6c2c531249b98aab2d19805c2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:26:39 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Sun, 02 Feb 2020 06:26:40 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:26:41 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:26:41 GMT
ENV JAVA_VERSION=11.0.6
# Sun, 02 Feb 2020 06:27:49 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Sun, 02 Feb 2020 06:27:49 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Sun, 02 Feb 2020 06:28:07 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV JETTY_BASE=/var/lib/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV TMPDIR=/tmp/jetty
# Sun, 02 Feb 2020 21:25:41 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 21:25:42 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Sun, 02 Feb 2020 21:25:42 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Sun, 02 Feb 2020 21:25:56 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Sun, 02 Feb 2020 21:25:56 GMT
WORKDIR /var/lib/jetty
# Sun, 02 Feb 2020 21:25:57 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Sun, 02 Feb 2020 21:25:57 GMT
USER jetty
# Sun, 02 Feb 2020 21:25:57 GMT
EXPOSE 8080
# Sun, 02 Feb 2020 21:25:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 21:25:57 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:bc51dd8edc1b1132bb97827ed6bd16aac332b03fb03d4c02d2088067a5fbb499`  
		Last Modified: Sat, 01 Feb 2020 17:26:19 GMT  
		Size: 27.1 MB (27092260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d06863bb82bdc3f4cd17d49c0dee8720f91c4d9e40cce1b4a691f9459266be`  
		Last Modified: Sun, 02 Feb 2020 06:31:53 GMT  
		Size: 3.2 MB (3249109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf4d10a782b71ea3c226ce20c1acdfb0aeefb137fb5c5fa3100aaa275ec71cd`  
		Last Modified: Sun, 02 Feb 2020 06:35:40 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db4424ff27024b682967e5ca869ba018b8667fdc7cbd2718db9ebba95c5e601`  
		Last Modified: Sun, 02 Feb 2020 06:36:47 GMT  
		Size: 42.2 MB (42172493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90391924a5e59bc44cf9ef90cb0f0abca2acffc23e923d1cb39caa67252de309`  
		Last Modified: Sun, 02 Feb 2020 21:27:20 GMT  
		Size: 9.9 MB (9884807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c397836cf4ec5aae02b21743025e7e579fa7f8a73966311e0b3ff9afb4eab7a4`  
		Last Modified: Sun, 02 Feb 2020 21:27:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9-jre11-slim` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:3ae1ed5d8853996490ad156f6fbbce9ff1eadc30e3bd6c372ca3fbb635faf5a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80110979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b3797cc47ed14b3f0d8c4b426d77be25adfba151f44c1f38c835a2565a1073d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:56:44 GMT
ENV LANG=C.UTF-8
# Wed, 26 Feb 2020 14:56:44 GMT
ENV JAVA_HOME=/usr/local/openjdk-11
# Wed, 26 Feb 2020 14:56:45 GMT
ENV PATH=/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 14:56:47 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 26 Feb 2020 14:56:48 GMT
ENV JAVA_VERSION=11.0.6
# Wed, 26 Feb 2020 14:58:22 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk11-upstream-binaries/releases/download/jdk-11.0.6%2B10/OpenJDK11U-jre_
# Wed, 26 Feb 2020 14:58:22 GMT
ENV JAVA_URL_VERSION=11.0.6_10
# Wed, 26 Feb 2020 14:58:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java --version
# Thu, 27 Feb 2020 03:33:08 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Thu, 27 Feb 2020 03:33:09 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 27 Feb 2020 03:33:09 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 27 Feb 2020 03:33:10 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 27 Feb 2020 03:33:11 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 03:33:11 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Thu, 27 Feb 2020 03:33:12 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Thu, 27 Feb 2020 03:33:45 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 		gnupg 		curl 		;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 27 Feb 2020 03:33:45 GMT
WORKDIR /var/lib/jetty
# Thu, 27 Feb 2020 03:33:46 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Thu, 27 Feb 2020 03:33:47 GMT
USER jetty
# Thu, 27 Feb 2020 03:33:47 GMT
EXPOSE 8080
# Thu, 27 Feb 2020 03:33:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Feb 2020 03:33:49 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa702e5900f7e9b9cc9f5827bff3c63c77b495471757e961459c43e338147a`  
		Last Modified: Wed, 26 Feb 2020 15:00:01 GMT  
		Size: 3.1 MB (3101218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b200df05fed1b744d2e15b2ec347e0774604f6b6f8073c708edf529bba593b`  
		Last Modified: Wed, 26 Feb 2020 15:00:00 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15600e576d9b8eed5a2f6ecab52d8fc99bae589a21c82c26d9c6648486d488a`  
		Last Modified: Wed, 26 Feb 2020 15:01:25 GMT  
		Size: 41.3 MB (41271650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3654953d70524aca1a86522276d777bd7ecce623e55fbd2df88f061efa3ce5a0`  
		Last Modified: Thu, 27 Feb 2020 03:34:24 GMT  
		Size: 9.9 MB (9884922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd14054f6eed9929490dbecbc97ab84a6db8e227508185fb9a6b99f031262d4`  
		Last Modified: Thu, 27 Feb 2020 03:34:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:9-jre8`

```console
$ docker pull jetty@sha256:3c43dbfe7d459e3b07bbdbd7836fc4c113c65abbd60c6cc70ed619e9aa4953bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:9-jre8` - linux; amd64

```console
$ docker pull jetty@sha256:38ba1d9e3e0aa0df06ca9a9381d2aee4c87c3df11683e7faa2de866d84229a1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123510115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fef4f0fb08f9ba16a07d92ffcaf15978adde6e3ff5621939db1e138dcb9054d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 07 Feb 2020 01:51:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:51:11 GMT
ENV LANG=C.UTF-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 07 Feb 2020 01:52:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 01:52:07 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_VERSION=8u242
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jre_
# Fri, 07 Feb 2020 01:52:08 GMT
ENV JAVA_URL_VERSION=8u242b08
# Fri, 07 Feb 2020 01:52:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64) upstreamArch='x64' ;; 		arm64) upstreamArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture: $dpkgArch" ;; 	esac; 		wget -O openjdk.tgz.asc "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz.sign"; 	wget -O openjdk.tgz "${JAVA_BASE_URL}${upstreamArch}_linux_${JAVA_URL_VERSION}.tar.gz" --progress=dot:giga; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 			{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 07 Feb 2020 03:31:16 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 07 Feb 2020 03:31:17 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 07 Feb 2020 03:31:17 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Feb 2020 03:31:17 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Fri, 07 Feb 2020 03:31:18 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Fri, 07 Feb 2020 03:31:24 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 07 Feb 2020 03:31:24 GMT
WORKDIR /var/lib/jetty
# Fri, 07 Feb 2020 03:31:25 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Fri, 07 Feb 2020 03:31:25 GMT
USER jetty
# Fri, 07 Feb 2020 03:31:25 GMT
EXPOSE 8080
# Fri, 07 Feb 2020 03:31:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Feb 2020 03:31:26 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f003f5c25f68e76d7a30f14f5dce60cfe3d74d6bf050d6dbb55356835ac85acf`  
		Last Modified: Fri, 07 Feb 2020 01:58:05 GMT  
		Size: 5.5 MB (5529324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92ee316420dc43acf210e0105c2778dd97000bb031079e33e38dbed6b55f1e2`  
		Last Modified: Fri, 07 Feb 2020 02:00:03 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a95be757d026695b0295c756dad4e045f668920a953df392432155f49fad15`  
		Last Modified: Fri, 07 Feb 2020 02:00:12 GMT  
		Size: 40.2 MB (40187618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7534a779acb5cde730e4dc712e3b6dabc8557f6bb43b153144dc5477a4a053e4`  
		Last Modified: Fri, 07 Feb 2020 03:33:12 GMT  
		Size: 9.6 MB (9603852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d3d1f3ae6adfd2ddce30430fcb3156f0e6d8670e6b680865c7e690955b4b50`  
		Last Modified: Fri, 07 Feb 2020 03:32:55 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:jdk13`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:jdk13` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jetty:latest`

```console
$ docker pull jetty@sha256:1db22bf78cf9f5de4c0e6ecf81513f3a19220c73ab017eb68d7980076fc99272
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jetty:latest` - linux; amd64

```console
$ docker pull jetty@sha256:c88295fa22a0dd4603800403089df6507c1f98842421e3d3d7d980105f020fd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.5 MB (263497606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ceb730f24ef32e6bd8bb0332fa09cc1536803f20534e3e72b50773fb39d87a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Tue, 28 Jan 2020 21:36:05 GMT
ADD file:a320cfe017a986947ac6b09db573e476eacafc80311e517efcc5e965fcc445fb in / 
# Tue, 28 Jan 2020 21:36:06 GMT
CMD ["/bin/bash"]
# Tue, 28 Jan 2020 21:53:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 28 Jan 2020 21:53:09 GMT
ENV LANG=en_US.UTF-8
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Tue, 28 Jan 2020 21:58:14 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 21:58:14 GMT
ENV JAVA_VERSION=13.0.2
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Tue, 28 Jan 2020 21:58:15 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Tue, 28 Jan 2020 21:58:47 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Tue, 28 Jan 2020 21:58:47 GMT
CMD ["jshell"]
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_VERSION=9.4.26.v20200117
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 28 Jan 2020 22:21:15 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 28 Jan 2020 22:21:16 GMT
ENV PATH=/usr/local/jetty/bin:/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.26.v20200117/jetty-home-9.4.26.v20200117.tar.gz
# Tue, 28 Jan 2020 22:21:16 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E
# Tue, 28 Jan 2020 22:21:20 GMT
RUN set -xe ;         export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ;         for key in $JETTY_GPG_KEYS; do                 for server in                         ha.pool.sks-keyservers.net                         p80.pool.sks-keyservers.net:80                         ipv4.pool.sks-keyservers.net                         pgp.mit.edu ;                 do                         if gpg --batch --keyserver "$server" --recv-keys "$key"; then                                 break;                         fi;                 done;         done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 28 Jan 2020 22:21:21 GMT
WORKDIR /var/lib/jetty
# Tue, 28 Jan 2020 22:21:21 GMT
COPY multi:b8b1838b39ef7d9df547fe9a734d87e1a3923c8022961091b24ee37feff4d404 in / 
# Tue, 28 Jan 2020 22:21:21 GMT
USER jetty
# Tue, 28 Jan 2020 22:21:21 GMT
EXPOSE 8080
# Tue, 28 Jan 2020 22:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Jan 2020 22:21:22 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:86607bb85307f4e017c6cc236573951482f1de084e0987480fecea9295c2f923`  
		Last Modified: Tue, 28 Jan 2020 21:37:18 GMT  
		Size: 42.7 MB (42725283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d217c4e16034b1dca5abb6ea80aabded93c73f35686d806d9f2aa8555743da`  
		Last Modified: Tue, 28 Jan 2020 22:00:21 GMT  
		Size: 14.8 MB (14793339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595022a553604b9baa8a02558174325cd4be3fb6b7920f86a7e425fc4539de5`  
		Last Modified: Tue, 28 Jan 2020 22:01:41 GMT  
		Size: 196.4 MB (196372674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c14f949cd943246f628a13af0a9c4403a70c2e6be8238df47d75e2286b0`  
		Last Modified: Tue, 28 Jan 2020 22:21:42 GMT  
		Size: 9.6 MB (9604896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091f93b27e22086d814ccdd64fd1a3830c831da6ee6c43ec1c5496a182194aef`  
		Last Modified: Tue, 28 Jan 2020 22:21:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
