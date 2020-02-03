## `clojure:openjdk-14-boot-slim-buster`

```console
$ docker pull clojure@sha256:87b910347e583a2be898813906f9ab8ad7a764794f50fbc1d63a958461194582
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-boot-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:2ab61171ee38f19ede9be1a523ff0cb1bd11d1bfdc9c20bca2ffb0c76c38ff03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.9 MB (288880826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:619962cc9c39bbb4944ca3567399690ae8629a9007656bee50547fd5adc537a5`
-	Default Command: `["boot","repl"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:54 GMT
ADD file:ba0c39345ccc4a882289d473ae8a67087056aa4475a26f3492fff75933d707de in / 
# Sat, 01 Feb 2020 17:20:54 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 06:19:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 06:19:43 GMT
ENV LANG=C.UTF-8
# Sun, 02 Feb 2020 06:22:53 GMT
ENV JAVA_HOME=/usr/java/openjdk-14
# Sun, 02 Feb 2020 06:22:53 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:22:55 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:22:55 GMT
ENV JAVA_VERSION=14-ea+34
# Sun, 02 Feb 2020 06:22:56 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/34/GPL/openjdk-14-ea+34_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:22:56 GMT
ENV JAVA_SHA256=51d9dd2161a912ab7bd2bf2e08043cdd175ce22b28608442e0d06bc777286158
# Sun, 02 Feb 2020 06:23:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:23:23 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:43:52 GMT
ENV BOOT_VERSION=2.8.3
# Sun, 02 Feb 2020 21:43:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:43:53 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 21:43:58 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get remove -y --purge wget && apt-get autoremove -y
# Sun, 02 Feb 2020 21:43:58 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 21:43:58 GMT
ENV BOOT_AS_ROOT=yes
# Sun, 02 Feb 2020 21:44:48 GMT
RUN boot
# Sun, 02 Feb 2020 21:44:48 GMT
CMD ["boot" "repl"]
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
	-	`sha256:7d3094a8803afb0148c3b1bb33abefbd6178d7e6fd2d074897735fbdcdc55ed4`  
		Last Modified: Sun, 02 Feb 2020 06:33:00 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2040ee43278f388deb957b072be36f7d1052eafb082ec91819c30df88e9dd4`  
		Last Modified: Sun, 02 Feb 2020 06:33:29 GMT  
		Size: 199.4 MB (199438691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07927efba9ca915befbbf80959a93351cbd2742122173e14c682c386d4e07a9e`  
		Last Modified: Sun, 02 Feb 2020 21:50:13 GMT  
		Size: 279.5 KB (279502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769b885b54631e8b8ff08f8ab5df343bbb42bf3ebcd08cedfdbfd71383a75351`  
		Last Modified: Sun, 02 Feb 2020 21:50:23 GMT  
		Size: 58.8 MB (58821052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
