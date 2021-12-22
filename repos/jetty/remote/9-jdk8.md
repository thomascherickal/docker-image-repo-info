## `jetty:9-jdk8`

```console
$ docker pull jetty@sha256:da1413c794a908508ccf97eee0d38ea581a1ea4c7f929dfa89f86676c5e7b911
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `jetty:9-jdk8` - linux; amd64

```console
$ docker pull jetty@sha256:fb0bdf40eb1653f44bbea0fa1a111804b016cdcae7ecfd0976d38f441141e35a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.8 MB (246825130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8236854441b7c69e471b3fab0111da5473b286ad9b8c9e77e826729e59f22921`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:07 GMT
ADD file:e777355768c63f735e5458c7e0ada7f556f27d0493b3af35dc7c34f9c4294ea9 in / 
# Thu, 02 Dec 2021 02:48:08 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:39:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:39:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:40:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:34:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:39:04 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 02 Dec 2021 11:39:06 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 02 Dec 2021 11:39:06 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:39:07 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 11:39:07 GMT
ENV JAVA_VERSION=8u312
# Thu, 02 Dec 2021 11:39:18 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Fri, 03 Dec 2021 13:38:31 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Fri, 03 Dec 2021 13:38:31 GMT
ENV JETTY_HOME=/usr/local/jetty
# Fri, 03 Dec 2021 13:38:31 GMT
ENV JETTY_BASE=/var/lib/jetty
# Fri, 03 Dec 2021 13:38:31 GMT
ENV TMPDIR=/tmp/jetty
# Fri, 03 Dec 2021 13:38:31 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Dec 2021 13:38:32 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Fri, 03 Dec 2021 13:38:32 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Fri, 03 Dec 2021 13:38:38 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Fri, 03 Dec 2021 13:38:39 GMT
WORKDIR /var/lib/jetty
# Fri, 03 Dec 2021 13:38:39 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Fri, 03 Dec 2021 13:38:39 GMT
USER jetty
# Fri, 03 Dec 2021 13:38:39 GMT
EXPOSE 8080
# Fri, 03 Dec 2021 13:38:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 03 Dec 2021 13:38:40 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:5e0b432e8ba9d9029a000e627840b98ffc1ed0c5172075b7d3e869be0df0fe9b`  
		Last Modified: Thu, 02 Dec 2021 02:53:18 GMT  
		Size: 54.9 MB (54932878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84cfd68b5cea612a8343c346bfa5bd6c486769010d12f7ec86b23c74887feb2`  
		Last Modified: Thu, 02 Dec 2021 03:49:22 GMT  
		Size: 5.2 MB (5153424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b8f2315954535f1e27cd13d777e73da4a787b0aebf4241d225beff3c91cbb1`  
		Last Modified: Thu, 02 Dec 2021 03:49:23 GMT  
		Size: 10.9 MB (10871995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fa43a7e793a76c198e8d45d8810394e1cfc943b2673d7fcf5a6fdc4f45b3`  
		Last Modified: Thu, 02 Dec 2021 03:49:46 GMT  
		Size: 54.6 MB (54567844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d35e3be804184359e0904389b149de16f159e30436d7a8a970aef67a4d155b`  
		Last Modified: Thu, 02 Dec 2021 11:54:46 GMT  
		Size: 5.4 MB (5420076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc526d02f40c8231c1f1a646ef714ef67cb72fbb9dd50ec2cee620314bc04f5d`  
		Last Modified: Thu, 02 Dec 2021 11:59:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f9f735b512422e868ee645f9d91e75398934c69b7bb87133bc5b6724662873`  
		Last Modified: Thu, 02 Dec 2021 12:00:00 GMT  
		Size: 106.0 MB (105998944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e403e65b873f7d7e5fe7441da428e4074fbdebc5ac589e3c002ccb12b08a6782`  
		Last Modified: Fri, 03 Dec 2021 13:44:45 GMT  
		Size: 9.9 MB (9878317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61fc4184a80a204d3e7a47c02f8f425e9c0bb05b7343bb04c4084d289281af1`  
		Last Modified: Fri, 03 Dec 2021 13:44:45 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `jetty:9-jdk8` - linux; arm64 variant v8

```console
$ docker pull jetty@sha256:808602e9fcf3632212109a8ecbcc788239b85e29ef8760fb65ba91a0c87608d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244381696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb411d6c9dce7032b4b0bf6277071830e5889f4d787cc6c1203eb79c6c60f93`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:59:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				fontconfig libfreetype6 				ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:04:13 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Tue, 21 Dec 2021 03:04:14 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Tue, 21 Dec 2021 03:04:15 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:04:16 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:04:17 GMT
ENV JAVA_VERSION=8u312
# Tue, 21 Dec 2021 03:04:27 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_8u312b07.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_8u312b07.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Tue, 21 Dec 2021 23:54:40 GMT
ENV JETTY_VERSION=9.4.44.v20210927
# Tue, 21 Dec 2021 23:54:41 GMT
ENV JETTY_HOME=/usr/local/jetty
# Tue, 21 Dec 2021 23:54:42 GMT
ENV JETTY_BASE=/var/lib/jetty
# Tue, 21 Dec 2021 23:54:43 GMT
ENV TMPDIR=/tmp/jetty
# Tue, 21 Dec 2021 23:54:44 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 23:54:45 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.44.v20210927/jetty-home-9.4.44.v20210927.tar.gz
# Tue, 21 Dec 2021 23:54:46 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Tue, 21 Dec 2021 23:54:52 GMT
RUN set -xe ; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	mkdir -p "$TMPDIR" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Tue, 21 Dec 2021 23:54:53 GMT
WORKDIR /var/lib/jetty
# Tue, 21 Dec 2021 23:54:55 GMT
COPY multi:a6bf79f83e3ff0c7dc5946cd61ca0413cd3191ce9671725a647923d97a115fae in / 
# Tue, 21 Dec 2021 23:54:55 GMT
USER jetty
# Tue, 21 Dec 2021 23:54:56 GMT
EXPOSE 8080
# Tue, 21 Dec 2021 23:54:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 23:54:58 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42dee876d81600359b18717394ceadea4e48ff2cf2ba9dbbcaa45763547c2c93`  
		Last Modified: Tue, 21 Dec 2021 03:25:46 GMT  
		Size: 5.4 MB (5420215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c93670a883a2973baaa5d76e9a839fa38f32535ebbf40514bc83df25eeeea7d`  
		Last Modified: Tue, 21 Dec 2021 03:30:45 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec98c142552ba44d2ccf8b5f638891a2657e1cd7210298bcdd5cd870629fc58`  
		Last Modified: Tue, 21 Dec 2021 03:30:56 GMT  
		Size: 105.0 MB (105010866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aeae593e9047b83aebb7f1ae298bd83a33a74d0fd3a6e657dd3dedbdcaa232b`  
		Last Modified: Wed, 22 Dec 2021 00:02:56 GMT  
		Size: 9.9 MB (9878031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550bef9ef6611dd9766144f61a4d2772a6455107acd3ff79200532c789c1982a`  
		Last Modified: Wed, 22 Dec 2021 00:02:54 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
