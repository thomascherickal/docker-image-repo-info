## `clojure:openjdk-16-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:ae369d156456ab618493f9021c85cf1b315ff2cee91b39beba6ad45946560b32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:42c14b9a0bca8d429a6994a927aeaf24f18a2cd512d03e71133dfe9732a9a653
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.4 MB (286359696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573f42bfe038272c04457dbf9ef17af818f291e945476a842f04c4e2e2c7d018`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:58:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:58:53 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 08:58:53 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Tue, 13 Oct 2020 08:58:54 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 08:58:55 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 13 Oct 2020 08:58:55 GMT
ENV JAVA_VERSION=16-ea+19
# Tue, 13 Oct 2020 08:59:15 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-aarch64_bin.tar.gz; 			downloadSha256=9e7094e0dcba61b6b8111f48934cb7395e6dafb1d1ddea7d2296cb0872d67d66; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-x64_bin.tar.gz; 			downloadSha256=487e44f1ec92106437a96f8af07a83ac314dee51dfd46838c23657e550bc616f; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 08:59:15 GMT
CMD ["jshell"]
# Wed, 14 Oct 2020 05:38:02 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 14 Oct 2020 05:38:02 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 14 Oct 2020 05:38:02 GMT
WORKDIR /tmp
# Wed, 14 Oct 2020 05:38:07 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 14 Oct 2020 05:38:07 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 14 Oct 2020 05:38:07 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 14 Oct 2020 05:38:24 GMT
RUN boot
# Wed, 14 Oct 2020 05:38:24 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00028440d132be6f9dd59a787bc5d1372d575a539c19954651757f12912f2e65`  
		Last Modified: Tue, 13 Oct 2020 09:08:08 GMT  
		Size: 3.2 MB (3248445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d3f9016801bc943373bbb1397fe32a0219af3d56f3a8361ffae543191883ce`  
		Last Modified: Tue, 13 Oct 2020 09:08:07 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80728a7db788564206df390d369abe82d5620798b7751315d6c11b9611840301`  
		Last Modified: Tue, 13 Oct 2020 09:08:26 GMT  
		Size: 196.9 MB (196919138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71ae83b35a3219f4513328e86ba39bac75c3ff926eac06f1029db568a948686`  
		Last Modified: Wed, 14 Oct 2020 05:47:49 GMT  
		Size: 279.5 KB (279540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26aaccda8518a3cb9ad0c48ba096419b99aa63427bdb74550ee63ab8559598ff`  
		Last Modified: Wed, 14 Oct 2020 05:47:50 GMT  
		Size: 58.8 MB (58820134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
