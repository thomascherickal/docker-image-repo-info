## `clojure:openjdk-8-boot-2.8.3-slim-bullseye`

```console
$ docker pull clojure@sha256:54981e302ab5901114d1e905d66067f26bfa4586827f932999b9f9010b27ac30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-8-boot-2.8.3-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:1b7671506a0223500775a43594852e3ba0a7fc78f50ceb699bf78bca3eb02e64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.3 MB (198317471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6137956d523a81e5f4c83af586c13f98697c243de23779cbfd51420503bf438`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:41:28 GMT
ENV JAVA_HOME=/usr/local/openjdk-8
# Fri, 03 Sep 2021 08:41:29 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ] # backwards compatibility
# Fri, 03 Sep 2021 08:41:29 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:41:29 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 08:41:29 GMT
ENV JAVA_VERSION=8u302
# Fri, 03 Sep 2021 08:41:46 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'arm64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	wget --progress=dot:giga -O openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/jre/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		javac -version; 	java -version
# Thu, 09 Sep 2021 19:26:23 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Sep 2021 19:26:23 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Sep 2021 19:26:23 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:26:27 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Sep 2021 19:26:27 GMT
ENV PATH=/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Sep 2021 19:26:28 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Sep 2021 19:26:47 GMT
RUN boot
# Thu, 09 Sep 2021 19:26:47 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:f8416d8bac72cefc0ce17bd2dc0c03aa43e123d309db92ee23be9382192cf2ed`  
		Last Modified: Fri, 03 Sep 2021 01:27:25 GMT  
		Size: 31.4 MB (31368702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ae0b0c4c13e1ebacfd091b8e226cc8aa92df8937632e3bec2b03a877bf2d87`  
		Last Modified: Fri, 03 Sep 2021 08:49:03 GMT  
		Size: 1.6 MB (1582002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098f9d3d8dab5a269d2e9252501b6c6d034bcb6debc0e8e7cb388002034df175`  
		Last Modified: Fri, 03 Sep 2021 09:05:50 GMT  
		Size: 208.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bd97f1dba1d1c9adb7383afa4ff1f571593dbf1ee23bd74b43beb994743c3d`  
		Last Modified: Fri, 03 Sep 2021 09:06:01 GMT  
		Size: 106.3 MB (106261868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69458d47d930e9ea7540fe3eaa69a214169cce296bd6b3c1a27fa2057a08cd0b`  
		Last Modified: Thu, 09 Sep 2021 19:43:01 GMT  
		Size: 284.2 KB (284246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9275db0d6f7c8a0bca362083eb60aaa8c6e30f1ee1fb413ef2ce7932ff1361d0`  
		Last Modified: Thu, 09 Sep 2021 19:43:04 GMT  
		Size: 58.8 MB (58820445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
