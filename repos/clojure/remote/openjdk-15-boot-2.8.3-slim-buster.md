## `clojure:openjdk-15-boot-2.8.3-slim-buster`

```console
$ docker pull clojure@sha256:92505e837cba134603cc0ce1e3e5af6d2b2fac62dd0d28f81fad2cdd6d85e7c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-boot-2.8.3-slim-buster` - linux; amd64

```console
$ docker pull clojure@sha256:d56b0c248bc20d856871eae360cf8f5acb459492991c98633526cca2e70c500e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.5 MB (285497865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385b34ffbff8e6315064bb75651e56717aa9cc9a08aa6d3d09d194d709dbceb2`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 16:34:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 16:34:37 GMT
ENV LANG=C.UTF-8
# Tue, 09 Jun 2020 16:34:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Tue, 09 Jun 2020 16:34:37 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Jun 2020 16:34:38 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Mon, 15 Jun 2020 21:24:52 GMT
ENV JAVA_VERSION=15-ea+27
# Mon, 15 Jun 2020 21:25:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/27/GPL/openjdk-15-ea+27_linux-aarch64_bin.tar.gz; 			downloadSha256=9195473bcb8e4ceaf0113cdb7b3dad468f3c045ebb9c0ce326bf01818c089269; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/27/GPL/openjdk-15-ea+27_linux-x64_bin.tar.gz; 			downloadSha256=db20094a26993699a0c6beb10dc5d07d9e708ab1fc0bfb7aff637944c3319374; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Mon, 15 Jun 2020 21:25:08 GMT
CMD ["jshell"]
# Mon, 15 Jun 2020 21:45:51 GMT
ENV BOOT_VERSION=2.8.3
# Mon, 15 Jun 2020 21:45:51 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Mon, 15 Jun 2020 21:45:52 GMT
WORKDIR /tmp
# Mon, 15 Jun 2020 21:45:57 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get remove -y --purge wget && apt-get autoremove -y
# Mon, 15 Jun 2020 21:45:57 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 15 Jun 2020 21:45:57 GMT
ENV BOOT_AS_ROOT=yes
# Mon, 15 Jun 2020 21:46:15 GMT
RUN boot
# Mon, 15 Jun 2020 21:46:15 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65306eca6b8ea03d29cd8d10a31e9d7a6a1cf8766fe4ca3913e75e00fc47be79`  
		Last Modified: Tue, 09 Jun 2020 16:41:33 GMT  
		Size: 3.2 MB (3248452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483b95dcfbd46dbdc1240666a5cb96e2881dbdecfff2f75f23bd5932127de1bd`  
		Last Modified: Tue, 09 Jun 2020 16:41:33 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cdf469058b65eae268ebfc2b4da5091fdc6e7298330e7bd7b167145ccb2a1c`  
		Last Modified: Mon, 15 Jun 2020 21:27:57 GMT  
		Size: 196.1 MB (196051237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c0a08eaebcda2d125136a485bd31f20fab52f2f2a70cecba4627889fd20f59`  
		Last Modified: Mon, 15 Jun 2020 21:48:24 GMT  
		Size: 279.6 KB (279602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec02e2eceae90c383c7cda17d12ab065d6abd6f4f7631c1a813e33ddf37c593b`  
		Last Modified: Mon, 15 Jun 2020 21:48:27 GMT  
		Size: 58.8 MB (58820099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
