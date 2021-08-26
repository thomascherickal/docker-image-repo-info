## `jetty:9-jre8-slim`

```console
$ docker pull jetty@sha256:3eb6cb2bb2815eda010f9b7107364228d07bbdb5420c3f75856b3b144d626002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jetty:9-jre8-slim` - linux; amd64

```console
$ docker pull jetty@sha256:8b6ff3144734148d74dcf6dc42e63b53d3f9ae1860b971c6503232da60dad03b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.7 MB (84713189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455373e370adfb726c545fa3b744ca71fb8eb88bf149c16ab46fd3715e6a019e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["java","-jar","\/usr\/local\/jetty\/start.jar"]`

```dockerfile
# Tue, 17 Aug 2021 01:23:40 GMT
ADD file:5e8343ab9a73edc27c2889634896e792ab289b85c206de0fc31183fdc0a32ac7 in / 
# Tue, 17 Aug 2021 01:23:41 GMT
CMD ["bash"]
# Thu, 26 Aug 2021 00:33:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Aug 2021 00:38:12 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Thu, 26 Aug 2021 00:38:13 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Thu, 26 Aug 2021 00:38:13 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 00:38:13 GMT
ENV LANG=C.UTF-8
# Thu, 26 Aug 2021 00:38:13 GMT
ENV JAVA_VERSION=8u302
# Thu, 26 Aug 2021 00:39:00 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -version
# Thu, 26 Aug 2021 01:46:00 GMT
ENV JETTY_VERSION=9.4.43.v20210629
# Thu, 26 Aug 2021 01:46:01 GMT
ENV JETTY_HOME=/usr/local/jetty
# Thu, 26 Aug 2021 01:46:01 GMT
ENV JETTY_BASE=/var/lib/jetty
# Thu, 26 Aug 2021 01:46:01 GMT
ENV TMPDIR=/tmp/jetty
# Thu, 26 Aug 2021 01:46:01 GMT
ENV PATH=/usr/local/jetty/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 01:46:01 GMT
ENV JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/9.4.43.v20210629/jetty-home-9.4.43.v20210629.tar.gz
# Thu, 26 Aug 2021 01:46:02 GMT
ENV JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E 	F254B35617DC255D9344BCFA873A8E86B4372146
# Thu, 26 Aug 2021 01:46:18 GMT
RUN set -xe ; 	export savedAptMark="$(apt-mark showmanual)" ; 	mkdir -p $TMPDIR ; 	apt-get update ; 	apt-get install -y --no-install-recommends 		ca-certificates 		p11-kit 		gnupg 		curl 		; 	export GNUPGHOME=/jetty-keys ; 	mkdir -p "$GNUPGHOME" ; 	for key in $JETTY_GPG_KEYS; do 		for server in 			ha.pool.sks-keyservers.net 			pgp.mit.edu 			hkp://p80.pool.sks-keyservers.net:80 			hkp://keyserver.ubuntu.com:80 			keyserver.pgp.com 			ipv4.pool.sks-keyservers.net ; 		do 			if gpg --batch --keyserver "$server" --recv-keys "$key"; then 				break; 			fi; 		done; 	done ; 	mkdir -p "$JETTY_HOME" ; 	cd $JETTY_HOME ; 	curl -SL "$JETTY_TGZ_URL" -o jetty.tar.gz ; 	curl -SL "$JETTY_TGZ_URL.asc" -o jetty.tar.gz.asc ; 	gpg --batch --verify jetty.tar.gz.asc jetty.tar.gz ; 	tar -xvf jetty.tar.gz --strip-components=1 ; 	sed -i '/jetty-logging/d' etc/jetty.conf ; 	mkdir -p "$JETTY_BASE" ; 	cd $JETTY_BASE ; 	java -jar "$JETTY_HOME/start.jar" --create-startd 		--add-to-start="server,http,deploy,jsp,jstl,ext,resources,websocket" ; 	groupadd -r jetty && useradd -r -g jetty jetty ; 	chown -R jetty:jetty "$JETTY_HOME" "$JETTY_BASE" "$TMPDIR" ; 	usermod -d $JETTY_BASE jetty ; 	apt-mark auto '.*' > /dev/null ; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null ; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false ; 	rm -rf /var/lib/apt/lists/* ; 	rm -rf /tmp/hsperfdata_root ; 	rm -fr $JETTY_HOME/jetty.tar.gz* ; 	rm -fr /jetty-keys $GNUPGHOME ; 	rm -rf /tmp/hsperfdata_root ; 	java -jar "$JETTY_HOME/start.jar" --list-config ;
# Thu, 26 Aug 2021 01:46:18 GMT
WORKDIR /var/lib/jetty
# Thu, 26 Aug 2021 01:46:18 GMT
COPY multi:aa77a0f6aef2add1a97bf742e5d8ca9322cda3f66ea7673ea49c33da7e5b0889 in / 
# Thu, 26 Aug 2021 01:46:18 GMT
USER jetty
# Thu, 26 Aug 2021 01:46:18 GMT
EXPOSE 8080
# Thu, 26 Aug 2021 01:46:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 26 Aug 2021 01:46:19 GMT
CMD ["java" "-jar" "/usr/local/jetty/start.jar"]
```

-	Layers:
	-	`sha256:99046ad9247f8a1cbd1048d9099d026191ad9cda63c08aadeb704b7000a51717`  
		Last Modified: Tue, 17 Aug 2021 01:29:35 GMT  
		Size: 31.4 MB (31361314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97c10298fea9915576e7ff72c6eca3d7c589aaafd6bc6481a5814c4271d2251`  
		Last Modified: Thu, 26 Aug 2021 00:43:26 GMT  
		Size: 1.6 MB (1581998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12127b9e959d71cc3433b3b0fadff2350394a628f731a4573086dab33730b236`  
		Last Modified: Thu, 26 Aug 2021 00:50:14 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6b7b86bdf62cb45e87be0b8e9a59e96c4d4e9ebfd06c912c37feae54d97a96`  
		Last Modified: Thu, 26 Aug 2021 00:51:12 GMT  
		Size: 41.6 MB (41632788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1c8125b1eef7acc3edfa4037aaa132cb3a9816dc15d638236e44740afdf48`  
		Last Modified: Thu, 26 Aug 2021 01:51:29 GMT  
		Size: 10.1 MB (10135428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42502c48b76d512b72d80af9098d5a17f4dd4c6fc2a9cf3ea673364db3ce9b9`  
		Last Modified: Thu, 26 Aug 2021 01:51:28 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
