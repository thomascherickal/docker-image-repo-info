## `openjdk:15-jdk-slim-buster`

```console
$ docker pull openjdk@sha256:36a289255f848aef117f2b746807e52a987f2b4de872d92bd98042d3ff27b0bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:15-jdk-slim-buster` - linux; amd64

```console
$ docker pull openjdk@sha256:479113eb9646df167d7d9349dbe8b1ec30bef94abdbe354ae443f6fa7f6a8013
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.7 MB (222710480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81e4d0ad168a9813c5134639b81e59c6556ef69f4226e2696ead0c0bb8e820c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 21:00:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 21:00:03 GMT
ENV LANG=C.UTF-8
# Fri, 15 May 2020 21:00:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 15 May 2020 21:00:04 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 21:00:05 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 15 May 2020 21:00:05 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 15 May 2020 21:00:05 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz
# Fri, 15 May 2020 21:00:06 GMT
ENV JAVA_SHA256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0
# Fri, 15 May 2020 21:00:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 15 May 2020 21:00:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee19e84e8bd1140527176689c9c1a75f28c0462c0c714e549536452708cbfb64`  
		Last Modified: Fri, 15 May 2020 21:07:16 GMT  
		Size: 3.2 MB (3249166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337e2ad6cc28f75db2e56f69cadbd0229b730550706f322b80ca8ad45ce205dd`  
		Last Modified: Fri, 15 May 2020 21:07:15 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284dbc7d417e87922e7f8dc2de9fd8d541ca46c57f67a3d419e84d8f72f13d03`  
		Last Modified: Fri, 15 May 2020 21:07:34 GMT  
		Size: 192.4 MB (192362347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
