## `clojure:openjdk-18-boot-slim-bullseye`

```console
$ docker pull clojure@sha256:8838c614e461d7ec85abde7fb0ee632a7ac53be67f6c191c9b06850689447949
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-boot-slim-bullseye` - linux; amd64

```console
$ docker pull clojure@sha256:e7f181155b54c4a7a824575a17e1ef2ce05b6d1cd74bd00332093cd2999a4f3b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.8 MB (279835833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af116af49d66b43000249c542ca87fd3d22af2288d48151f0d545e269d87a64`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:21 GMT
ADD file:19d7ba0fceddd7fc78b5fb96cf8110e5d10e0e5d2554030dfe640d161379cb79 in / 
# Fri, 03 Sep 2021 01:21:21 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 08:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:31:20 GMT
ENV JAVA_HOME=/usr/local/openjdk-18
# Fri, 03 Sep 2021 08:31:20 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 08:31:20 GMT
ENV LANG=C.UTF-8
# Sat, 04 Sep 2021 09:42:18 GMT
ENV JAVA_VERSION=18-ea+13
# Sat, 04 Sep 2021 09:42:31 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-x64_bin.tar.gz'; 			downloadSha256='396584ea555ad439176473f4e22c146817290a8eeaad02e3072dfb398ba786e0'; 			;; 		'arm64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/13/GPL/openjdk-18-ea+13_linux-aarch64_bin.tar.gz'; 			downloadSha256='4601ee9811daa3bf282753e1fa6b8caffd869d0e56c9acfe95e1670bc580ed34'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget --progress=dot:giga -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$JAVA_HOME/lib/security/cacerts"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 04 Sep 2021 09:42:32 GMT
CMD ["jshell"]
# Thu, 09 Sep 2021 19:33:40 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Sep 2021 19:33:40 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Sep 2021 19:33:40 GMT
WORKDIR /tmp
# Thu, 09 Sep 2021 19:33:44 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Thu, 09 Sep 2021 19:33:44 GMT
ENV PATH=/usr/local/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 09 Sep 2021 19:33:44 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 09 Sep 2021 19:34:02 GMT
RUN boot
# Thu, 09 Sep 2021 19:34:02 GMT
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
	-	`sha256:25baa4d26f4c51077d9f4064945d9e80538961a0548091534e19f6b026db4374`  
		Last Modified: Sat, 04 Sep 2021 09:51:04 GMT  
		Size: 187.8 MB (187781630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d019a6616b4bd5c7e65e4034cd0b11f3befedd335fcb45c620d428ca0bf738`  
		Last Modified: Thu, 09 Sep 2021 19:50:19 GMT  
		Size: 283.0 KB (283048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a96c21dffc9894916922a45b82316db008308b0bd03eee28cb535b0d14e221c`  
		Last Modified: Thu, 09 Sep 2021 19:50:22 GMT  
		Size: 58.8 MB (58820451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
