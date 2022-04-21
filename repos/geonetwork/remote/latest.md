## `geonetwork:latest`

```console
$ docker pull geonetwork@sha256:5d11d35efa4ccb9df755686c19251ec02a5393d74c1ae8a998d4f88dfd111062
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `geonetwork:latest` - linux; amd64

```console
$ docker pull geonetwork@sha256:766574efe3bae767044d627d4d9fbb364128088a16b3ef2c0c65a4c44a7af501
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.3 MB (484292017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74591f1934710f42d6003e7ab3f60546cba472857e4c3020b97d329bcebbbdf6`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:57:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:55:59 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 20 Apr 2022 10:55:59 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 20 Apr 2022 10:55:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 10:55:59 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 10:55:59 GMT
ENV JAVA_VERSION=8u322
# Wed, 20 Apr 2022 10:56:05 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 21 Apr 2022 01:39:28 GMT
ENV JETTY_VERSION=9.4.46.v20220331
# Thu, 21 Apr 2022 01:39:28 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 21 Apr 2022 01:39:28 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 21 Apr 2022 01:39:28 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 21 Apr 2022 01:39:28 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 21 Apr 2022 01:39:28 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.46.v20220331/jetty-home-9.4.46.v20220331.tar.gz
# Thu, 21 Apr 2022 01:39:28 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 21 Apr 2022 01:39:37 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 21 Apr 2022 01:39:37 GMT
WORKDIR /var/lib/jetty
# Thu, 21 Apr 2022 01:39:38 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Thu, 21 Apr 2022 01:39:38 GMT
USER jetty
# Thu, 21 Apr 2022 01:39:38 GMT
EXPOSE 8080
# Thu, 21 Apr 2022 01:39:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Apr 2022 01:39:38 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Thu, 21 Apr 2022 11:57:51 GMT
ENV DATA_DIR=/catalogue-data
# Thu, 21 Apr 2022 11:57:51 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Thu, 21 Apr 2022 11:57:51 GMT
USER root
# Thu, 21 Apr 2022 11:57:54 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Thu, 21 Apr 2022 11:57:54 GMT
USER jetty
# Thu, 21 Apr 2022 11:57:54 GMT
ENV GN_FILE=geonetwork.war
# Thu, 21 Apr 2022 11:57:54 GMT
ENV GN_VERSION=4.0.6
# Thu, 21 Apr 2022 11:57:54 GMT
ENV GN_DOWNLOAD_MD5=793732cb9c723e73857a4da73b78451b
# Thu, 21 Apr 2022 11:58:28 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Thu, 21 Apr 2022 11:58:29 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Thu, 21 Apr 2022 11:58:29 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Thu, 21 Apr 2022 11:58:30 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Thu, 21 Apr 2022 11:58:30 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967757d5652770cfa81b6cc7577d65e06d336173da116d1fb5b2d349d5d44127`  
		Last Modified: Wed, 20 Apr 2022 07:05:43 GMT  
		Size: 5.2 MB (5155716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357e2c68cb3bf1e98dcb3eb6ceb16837253db71535921d6993c594588bffe04`  
		Last Modified: Wed, 20 Apr 2022 07:05:45 GMT  
		Size: 10.9 MB (10874928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ccb680c1c472c36a4595e2d4a2b4d1a434c377feb1ec57942b4006051064e6`  
		Last Modified: Wed, 20 Apr 2022 11:12:20 GMT  
		Size: 5.7 MB (5657427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8878e24fd9e707ced7ce1489388fd559b17000f5c28a4829bcb49f29d3cca6`  
		Last Modified: Wed, 20 Apr 2022 11:15:58 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811f4d5a35b1413e3e201c97e98ccbed53dbe4185273b45abdf27cbb0c40e18`  
		Last Modified: Wed, 20 Apr 2022 11:16:03 GMT  
		Size: 41.4 MB (41387518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8f9289e1409b4fe8699050890b13ba613a735e5a206d664937593f7ecbb8fb`  
		Last Modified: Thu, 21 Apr 2022 01:50:22 GMT  
		Size: 9.9 MB (9907489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518bb9471bd9004426aa1d26b35ca16c827152356ffdd0aee9957c1b6dbcc625`  
		Last Modified: Thu, 21 Apr 2022 01:50:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e36a5debfbc133cf1058d33493547f4e7bf6f68614b9789f4d88b3d6f9ed1b`  
		Last Modified: Thu, 21 Apr 2022 11:59:34 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8e6e135931654e6b2f5d6bc9e1f90cf214c903dbda9c4eafc1f285e9c201c5`  
		Last Modified: Thu, 21 Apr 2022 11:59:53 GMT  
		Size: 356.4 MB (356364046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e78c6fcf2d176e84314dd03482cd6869eac5195f722dd9757416024b8c7bae`  
		Last Modified: Thu, 21 Apr 2022 11:59:35 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `geonetwork:latest` - linux; arm64 variant v8

```console
$ docker pull geonetwork@sha256:fdd84f65785abd8846b2b935345ee09cf5e806d6500a24d65d6472f83c5e0143
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **481.8 MB (481807871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778149f647b49f26cb235e09864b77ab50edd5ca06702f4bbb0e50bb2208f6e8`
-	Entrypoint: `["\/geonetwork-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 09:07:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 09:09:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Wed, 30 Mar 2022 09:09:58 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Wed, 30 Mar 2022 09:09:59 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 09:10:00 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 09:10:01 GMT
ENV JAVA_VERSION=8u322
# Wed, 30 Mar 2022 09:10:08 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_x64_linux_8u322b06.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jre_aarch64_linux_8u322b06.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Tue, 05 Apr 2022 17:49:09 GMT
ENV JETTY_VERSION=9.4.46.v20220331
# Tue, 05 Apr 2022 17:49:10 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 05 Apr 2022 17:49:11 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 05 Apr 2022 17:49:12 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 05 Apr 2022 17:49:13 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 17:49:14 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.46.v20220331/jetty-home-9.4.46.v20220331.tar.gz
# Tue, 05 Apr 2022 17:49:15 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 05 Apr 2022 17:49:25 GMT
RUN set -xe ; 	mkdir -p $TMPDIR ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		gpg --batch --keyserver "hkps://keyserver.ubuntu.com" --recv-keys "$key"; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 05 Apr 2022 17:49:25 GMT
WORKDIR /var/lib/jetty
# Tue, 05 Apr 2022 17:49:27 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Tue, 05 Apr 2022 17:49:27 GMT
USER jetty
# Tue, 05 Apr 2022 17:49:28 GMT
EXPOSE 8080
# Tue, 05 Apr 2022 17:49:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 Apr 2022 17:49:30 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 05 Apr 2022 19:15:46 GMT
ENV DATA_DIR=/catalogue-data
# Tue, 05 Apr 2022 19:15:47 GMT
ENV JAVA_OPTS=-Dorg.eclipse.jetty.annotations.AnnotationParser.LEVEL=OFF         -Djava.security.egd=file:/dev/./urandom -Djava.awt.headless=true         -Xms512M -Xss512M -Xmx2G -XX:+UseConcMarkSweepGC         -Dgeonetwork.resources.dir=/catalogue-data/resources         -Dgeonetwork.data.dir=/catalogue-data         -Dgeonetwork.codeList.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/codelist         -Dgeonetwork.schema.dir=/var/lib/jetty/webapps/geonetwork/WEB-INF/data/config/schema_plugins
# Tue, 05 Apr 2022 19:15:48 GMT
USER root
# Tue, 05 Apr 2022 19:15:52 GMT
RUN apt-get -y update &&     apt-get -y install curl &&     rm -rf /var/lib/apt/lists/* &&     mkdir -p /${DATA_DIR} &&     chown -R jetty:jetty ${DATA_DIR} &&     mkdir -p /var/lib/jetty/webapps/geonetwork &&     chown -R jetty:jetty /var/lib/jetty/webapps/geonetwork
# Tue, 05 Apr 2022 19:15:52 GMT
USER jetty
# Tue, 05 Apr 2022 19:15:53 GMT
ENV GN_FILE=geonetwork.war
# Tue, 05 Apr 2022 19:15:54 GMT
ENV GN_VERSION=4.0.6
# Tue, 05 Apr 2022 19:15:55 GMT
ENV GN_DOWNLOAD_MD5=793732cb9c723e73857a4da73b78451b
# Tue, 05 Apr 2022 19:17:14 GMT
RUN cd /var/lib/jetty/webapps/geonetwork/ &&      curl -fSL -o geonetwork.war      https://sourceforge.net/projects/geonetwork/files/GeoNetwork_opensource/v${GN_VERSION}/${GN_FILE}/download &&      echo "${GN_DOWNLOAD_MD5} *geonetwork.war" | md5sum -c &&      unzip -q geonetwork.war &&      rm geonetwork.war
# Tue, 05 Apr 2022 19:17:15 GMT
COPY file:ca46ab251df3dfc253cb04cf962e7266e42428fab31ad2f583a7c86b06d5f778 in /geonetwork-entrypoint.sh 
# Tue, 05 Apr 2022 19:17:15 GMT
ENTRYPOINT ["/geonetwork-entrypoint.sh"]
# Tue, 05 Apr 2022 19:17:16 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
# Tue, 05 Apr 2022 19:17:17 GMT
VOLUME [/catalogue-data]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7231566decf8fbce03d4780325fa68b475237a1f9fa0638d4178aa8c09aa71`  
		Last Modified: Wed, 30 Mar 2022 09:31:31 GMT  
		Size: 5.6 MB (5649049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7d2aecfeabca96ca23febcdac6ae00782336d0eca6ae914bbbe4e77ee86bd7`  
		Last Modified: Wed, 30 Mar 2022 09:34:37 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112cd66392a9cb85905ca9fa430b7dd08123fa3fdf678b82a1e7c386df8e5255`  
		Last Modified: Wed, 30 Mar 2022 09:34:42 GMT  
		Size: 40.7 MB (40653745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7dc0e30be4dabf0ab31630b9cf2b9fedc37a8877e2a93c927cea6f179c50c5`  
		Last Modified: Tue, 05 Apr 2022 18:16:14 GMT  
		Size: 9.9 MB (9907182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e847d799b3b8d2ec3d63d127dd138c5516aac483e9a9c878d191c43951f78af`  
		Last Modified: Tue, 05 Apr 2022 18:16:13 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaa97543c39ebd8d357a0249f390b815758a8a61d5a172014802d7e604f98fb`  
		Last Modified: Tue, 05 Apr 2022 19:17:55 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d4b42ea40764617971d073808447f88b845db1a715daa2b9f9b8a4f21ecc6`  
		Last Modified: Tue, 05 Apr 2022 19:18:20 GMT  
		Size: 356.4 MB (356365728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c82e6b14a777b84b88ad6a0cf4d948378462f6f1bf664abf6a5f56e27afa7`  
		Last Modified: Tue, 05 Apr 2022 19:17:55 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
