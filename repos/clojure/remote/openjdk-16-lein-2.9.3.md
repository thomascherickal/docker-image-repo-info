## `clojure:openjdk-16-lein-2.9.3`

```console
$ docker pull clojure@sha256:3357c07e5fd5c6f6a8d60b6938aa48633bb514c0f1e05a5bf747e358c5862772
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-lein-2.9.3` - linux; amd64

```console
$ docker pull clojure@sha256:f9cbf5bee1a2f57f3ea4548782f4268c71a1b445a8edd75aeeb8a4f6fbb6e56a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.9 MB (244920404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cc5de158b93491218004f511c95bfd461aaddb96775d25fa54af4055889177d`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 00:41:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates p11-kit 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:41:10 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:41:10 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 05 Aug 2020 00:41:10 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:41:11 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 14 Aug 2020 21:35:00 GMT
ENV JAVA_VERSION=16-ea+11
# Fri, 14 Aug 2020 21:35:19 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/11/GPL/openjdk-16-ea+11_linux-aarch64_bin.tar.gz; 			downloadSha256=4c29bf2f7773d5eced73448f29bfa171fb19d66b4428f606aaedc4aba2675ab5; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/11/GPL/openjdk-16-ea+11_linux-x64_bin.tar.gz; 			downloadSha256=05c97ccd24ab86dffb7d31d04a331abd3b1556a25ad8dbc164767e6dfc39c151; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 14 Aug 2020 21:35:20 GMT
CMD ["jshell"]
# Fri, 14 Aug 2020 22:36:16 GMT
ENV LEIN_VERSION=2.9.3
# Fri, 14 Aug 2020 22:36:16 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 14 Aug 2020 22:36:16 GMT
WORKDIR /tmp
# Fri, 14 Aug 2020 22:36:25 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Fri, 14 Aug 2020 22:36:25 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 14 Aug 2020 22:36:25 GMT
ENV LEIN_ROOT=1
# Fri, 14 Aug 2020 22:36:30 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 14 Aug 2020 22:36:30 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092c9b8e633fd73a2b448815d56f09aebf34c733300cd7747008b81fe7724a02`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 3.2 MB (3248431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f811f0c47b7b271400f9827cb66bce990712143e46c11a9ded3e27403fed9485`  
		Last Modified: Wed, 05 Aug 2020 00:48:13 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e638fe599aa87a65e3f7503a9b6976428471bab36753b93737abc31034e10958`  
		Last Modified: Fri, 14 Aug 2020 21:40:10 GMT  
		Size: 196.9 MB (196948141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddf617d399a1c21301b97a872f01d3aa39ea8f947c755029e845cb56acac4d9`  
		Last Modified: Fri, 14 Aug 2020 22:40:36 GMT  
		Size: 13.5 MB (13463343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f196f1188152b70a4b5a378579e0be88c8567c9d7bde58359c9b30d2069f5ec3`  
		Last Modified: Fri, 14 Aug 2020 22:40:35 GMT  
		Size: 4.2 MB (4168157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
