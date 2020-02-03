## `clojure:openjdk-14-lein-buster`

```console
$ docker pull clojure@sha256:40266994fcb5bc3bace969421865ef8288c45d4b90878c48cf71d306dff00628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-lein-buster` - linux; amd64

```console
$ docker pull clojure@sha256:3f35f8aa1f3b7a18b7299541e218187d10a19804d624f08ef1a92b322b120103
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.4 MB (350376135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27b32d71265eebb50d8320f890d396d73f905baeb7f446ee79dc993ff4848e36`
-	Default Command: `["lein","repl"]`

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
# Sun, 02 Feb 2020 06:20:25 GMT
ENV JAVA_VERSION=14-ea+34
# Sun, 02 Feb 2020 06:20:25 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk14/34/GPL/openjdk-14-ea+34_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:20:26 GMT
ENV JAVA_SHA256=51d9dd2161a912ab7bd2bf2e08043cdd175ce22b28608442e0d06bc777286158
# Sun, 02 Feb 2020 06:22:42 GMT
RUN set -eux; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:22:43 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:43:39 GMT
ENV LEIN_VERSION=2.9.1
# Sun, 02 Feb 2020 21:43:39 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:43:39 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 21:43:44 GMT
RUN mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha1sum lein-pkg && echo "93be2c23ab4ff2fc4fcf531d7510ca4069b8d24a *lein-pkg" | sha1sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver pool.sks-keyservers.net --recv-key 2B72BF956E23DE5E830D50F6002AF007D1A7CC18 && echo "Verifying Jar file signature ..." && gpg --verify leiningen-$LEIN_VERSION-standalone.zip.asc && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar
# Sun, 02 Feb 2020 21:43:44 GMT
ENV PATH=/usr/java/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 21:43:44 GMT
ENV LEIN_ROOT=1
# Sun, 02 Feb 2020 21:43:48 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Sun, 02 Feb 2020 21:43:48 GMT
CMD ["lein" "repl"]
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
	-	`sha256:e481abbc9f0cfcc942cb29092a353e674adffeffb6e87a6cd570c7e7d81404a4`  
		Last Modified: Sun, 02 Feb 2020 06:32:52 GMT  
		Size: 199.2 MB (199171026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3953b2816c0f2b21b34b20643088a56d0bbcbcd10e903eee186e019ebd223aeb`  
		Last Modified: Sun, 02 Feb 2020 21:50:05 GMT  
		Size: 13.1 MB (13137776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ce7d866b5ce84f03c624bd2847f0d243f1feab7936eadb5f5ea32fd7ad62e5`  
		Last Modified: Sun, 02 Feb 2020 21:50:04 GMT  
		Size: 4.2 MB (4168177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
