## `clojure:openjdk-13-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:ac95ffbf1dd3fb7cea5ff05eb659b9284afdd5c25f2a883e949b1c6035e4e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-13-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:1336cf6a4a57e4de5353dfb3093f11adcc1b4b69899e10f1d4b47402ae8563a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286117545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:847ba15e8b9b47e695ca07c5faf131f451ed85fb27e989ecb7ced16f6c83bf84`
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
# Sun, 02 Feb 2020 21:40:38 GMT
ENV BOOT_VERSION=2.8.3
# Sun, 02 Feb 2020 21:40:38 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:40:38 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 21:40:43 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && echo "f717ef381f2863a4cad47bf0dcc61e923b3d2afb *boot.sh" | sha1sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get remove -y --purge wget && apt-get autoremove -y
# Sun, 02 Feb 2020 21:40:43 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 21:40:43 GMT
ENV BOOT_AS_ROOT=yes
# Sun, 02 Feb 2020 21:41:35 GMT
RUN boot
# Sun, 02 Feb 2020 21:41:36 GMT
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
	-	`sha256:42e615298152110cce920a0c9a2fee428cf50d77f2dd7fee4bc9e6aab96b3cd3`  
		Last Modified: Sun, 02 Feb 2020 06:34:28 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485e6161e84f226468239fee43881f9eee91c8008dcf21994bf0caf5e10ced9f`  
		Last Modified: Sun, 02 Feb 2020 06:34:55 GMT  
		Size: 196.7 MB (196675123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a01a3675c6631f9b97b7f4c4e7008226a446100c5e44b4ff5df01d1aafcd80`  
		Last Modified: Sun, 02 Feb 2020 21:49:18 GMT  
		Size: 279.6 KB (279588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c709162ec695a6bb88c26d7dfddb6efbfe7ee4e88bd81a5639164b157d729b`  
		Last Modified: Sun, 02 Feb 2020 21:49:23 GMT  
		Size: 58.8 MB (58821253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
