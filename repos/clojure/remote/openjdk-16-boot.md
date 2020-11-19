## `clojure:openjdk-16-boot`

```console
$ docker pull clojure@sha256:94a17845fb60ef5675d393744908de77134acabdad5364813e2655015e28dae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot` - linux; amd64

```console
$ docker pull clojure@sha256:741df94628b92608b5bcfa812b5bd75c76c919a1bdfe25f54de4b9078f76431f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.4 MB (273372754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ef876552c3e5e52aa574dcf3c6c6b8491bcd7c9432c1d72968c74038702406`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:14:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:14:56 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 00:14:57 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 18 Nov 2020 00:14:57 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 00:14:59 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 18 Nov 2020 00:14:59 GMT
ENV JAVA_VERSION=16-ea+24
# Wed, 18 Nov 2020 00:16:13 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/24/GPL/openjdk-16-ea+24_linux-aarch64_bin.tar.gz; 			downloadSha256=9085bbb4f9e4d70ac385f85fbd706ab1fa570417beb28d09ff71e4908684cd8c; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/24/GPL/openjdk-16-ea+24_linux-x64_bin.tar.gz; 			downloadSha256=ad1e33e43f923a8cde6e611e8ada1b76047f156d44b981d16daa440251f71823; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 Nov 2020 00:16:13 GMT
CMD ["jshell"]
# Wed, 18 Nov 2020 19:35:15 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 18 Nov 2020 19:35:16 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 18 Nov 2020 19:35:16 GMT
WORKDIR /tmp
# Wed, 18 Nov 2020 19:35:21 GMT
RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/* && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apt-get purge -y --auto-remove wget
# Wed, 18 Nov 2020 19:35:21 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 18 Nov 2020 19:35:21 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 18 Nov 2020 19:35:38 GMT
RUN boot
# Wed, 18 Nov 2020 19:35:38 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef17c1a944643971956760785cd2fdb1ae360b47af01d997bd7580f32b8b3512`  
		Last Modified: Wed, 18 Nov 2020 00:22:53 GMT  
		Size: 3.2 MB (3248467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f372ea5b91612afd4a4eedf6685a7aca438c668a5c19bc23dcb12519c861fb2`  
		Last Modified: Wed, 18 Nov 2020 00:22:51 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b9b962b40966fdc98e248f6efb928d59107db89d744e181c92d103b8081377`  
		Last Modified: Wed, 18 Nov 2020 00:23:29 GMT  
		Size: 183.9 MB (183919017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3591051dc2ae9b4c962f64c5b62c6b81e3c172777a168661710c27ddd00d6e`  
		Last Modified: Wed, 18 Nov 2020 19:40:47 GMT  
		Size: 279.5 KB (279542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc8685761dcba55b92a21e16754ec5f5aaa0e219f18ec6892113f3c8a9992e7`  
		Last Modified: Wed, 18 Nov 2020 19:40:52 GMT  
		Size: 58.8 MB (58820033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
