## `clojure:openjdk-14-boot-2.8.3-buster`

```console
$ docker pull clojure@sha256:9787e62790bede92fb8f16a626361128d9a75913beec328ebd79831c303a39cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-boot-2.8.3-buster` - linux; amd64

```console
$ docker pull clojure@sha256:c60199deee8df8c5072e75c13989e76b7d063688873b96baf2c4b081d4351ebc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.9 MB (391897992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e4ef05ad21dfc5ecd00f09e5bf39e76a54228f7846e9fe1a9c8d668edee3406`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:19:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:17:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:17:00 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:20:23 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Sun, 02 Feb 2020 06:20:23 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:20:25 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 11 Feb 2020 01:25:42 GMT
ENV JAVA_VERSION=14
# Tue, 11 Feb 2020 01:25:42 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk14/076bab302c7b4508975440c56f6cc26a/36/GPL/openjdk-14_linux-x64_bin.tar.gz
# Tue, 11 Feb 2020 01:25:43 GMT
ENV JAVA_SHA256=c7006154dfb8b66328c6475447a396feb0042608ee07a96956547f574a911c09
# Tue, 11 Feb 2020 01:25:53 GMT
RUN set -eux; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Tue, 11 Feb 2020 01:25:53 GMT
CMD ["jshell"]
# Tue, 11 Feb 2020 01:56:47 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 11 Feb 2020 01:56:47 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 11 Feb 2020 01:56:47 GMT
WORKDIR /tmp
# Tue, 11 Feb 2020 01:56:48 GMT
RUN mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot
# Tue, 11 Feb 2020 01:56:48 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 11 Feb 2020 01:56:48 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 11 Feb 2020 02:02:10 GMT
RUN boot
# Tue, 11 Feb 2020 02:02:10 GMT
CMD ["boot" "repl"]
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
	-	`sha256:8ac92ddf84b35dac36ef6632f8d5a0c9c2d7038f6018f2d4fa1be056d90bd366`  
		Last Modified: Sun, 02 Feb 2020 00:38:05 GMT  
		Size: 51.8 MB (51791113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171ac08b2613fc7531bea75c3b44590d543c67657eb7fb03c5132a4a59091995`  
		Last Modified: Sun, 02 Feb 2020 06:31:24 GMT  
		Size: 13.9 MB (13920140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93999c29a7f5759064280f3f2fed9bf1fa9127d385ddef43c11261b9baca34de`  
		Last Modified: Sun, 02 Feb 2020 06:32:28 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd37e08c596733dabbeaa8d6c3e6f041323f918e128e3fed122ae3c9db1588b3`  
		Last Modified: Tue, 11 Feb 2020 01:30:19 GMT  
		Size: 199.2 MB (199170930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f312ff5dd610d163d071f36a693d8b69c9a2df80b575dcb8daefa96f6c33ef3e`  
		Last Modified: Tue, 11 Feb 2020 02:04:06 GMT  
		Size: 6.9 KB (6894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3e7036ff3b37dd4a9a876c2069531fea1e0dc26674587c1a9f24e9abcee4ae`  
		Last Modified: Tue, 11 Feb 2020 02:04:09 GMT  
		Size: 58.8 MB (58821012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
