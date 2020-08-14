## `clojure:openjdk-16-buster`

```console
$ docker pull clojure@sha256:f7b493c7339749b3d53336afc7b914c310da6553ef14f43b1bb033a065f9c920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-buster` - linux; amd64

```console
$ docker pull clojure@sha256:83c2172ff0a6f16056b37549b7566ec6af43235b3cf23f8f05a0cdac69a3f0a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.3 MB (348344904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ce7bfe9909f828f0179d56354fb249d33038d8b65ff868a60fcdfcd78c343f`
-	Default Command: `["lein","repl"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:33 GMT
ADD file:4b03b5f551e3fbdf47ec609712007327828f7530cc3455c43bbcdcaf449a75a9 in / 
# Tue, 04 Aug 2020 15:42:34 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:26:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:26:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:40:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 				ca-certificates p11-kit 				binutils 		fontconfig libfreetype6 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 00:40:17 GMT
ENV LANG=C.UTF-8
# Wed, 05 Aug 2020 00:40:17 GMT
ENV JAVA_HOME=/usr/local/openjdk-16
# Wed, 05 Aug 2020 00:40:17 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:40:18 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Fri, 14 Aug 2020 21:34:38 GMT
ENV JAVA_VERSION=16-ea+11
# Fri, 14 Aug 2020 21:34:53 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/11/GPL/openjdk-16-ea+11_linux-aarch64_bin.tar.gz; 			downloadSha256=4c29bf2f7773d5eced73448f29bfa171fb19d66b4428f606aaedc4aba2675ab5; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/11/GPL/openjdk-16-ea+11_linux-x64_bin.tar.gz; 			downloadSha256=05c97ccd24ab86dffb7d31d04a331abd3b1556a25ad8dbc164767e6dfc39c151; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Fri, 14 Aug 2020 21:34:53 GMT
CMD ["jshell"]
# Fri, 14 Aug 2020 22:36:34 GMT
ENV LEIN_VERSION=2.9.3
# Fri, 14 Aug 2020 22:36:35 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 14 Aug 2020 22:36:35 GMT
WORKDIR /tmp
# Fri, 14 Aug 2020 22:36:41 GMT
RUN apt-get update && apt-get install -y gnupg && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg
# Fri, 14 Aug 2020 22:36:41 GMT
ENV PATH=/usr/local/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 14 Aug 2020 22:36:41 GMT
ENV LEIN_ROOT=1
# Fri, 14 Aug 2020 22:36:45 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 14 Aug 2020 22:36:46 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:d6ff36c9ec4822c9ff8953560f7ba41653b348a9c1136755e653575f58fbded7`  
		Last Modified: Tue, 04 Aug 2020 15:48:55 GMT  
		Size: 50.4 MB (50396000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c958d65b3090aefea91284d018b2a86530a3c8174b72616c4e76993c696a5797`  
		Last Modified: Tue, 04 Aug 2020 23:39:28 GMT  
		Size: 7.8 MB (7811570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf0a6b092f5673ec05b40edb606ce58881b2f40494251117d31805225ef064`  
		Last Modified: Tue, 04 Aug 2020 23:39:27 GMT  
		Size: 10.0 MB (9996337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80931cf6881673fd161a3fd73e8971fe4a569fd7fbb44e956d261ca58d97dfab`  
		Last Modified: Tue, 04 Aug 2020 23:39:45 GMT  
		Size: 51.8 MB (51829826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5ed57a778ea7eb4059433e847154a27357e6d5eb35018019feeba2d665a29a`  
		Last Modified: Wed, 05 Aug 2020 00:47:46 GMT  
		Size: 13.9 MB (13920152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2541bf853c1176f4c750573077846621cbb2ff3d39ef25fb8ca2127893ba91d5`  
		Last Modified: Wed, 05 Aug 2020 00:47:44 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750fc036fce4db44825e940fddd3a8ce23994286df9f2a28e39f4f50b2383831`  
		Last Modified: Fri, 14 Aug 2020 21:39:45 GMT  
		Size: 196.7 MB (196681939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef303fff6326f22185387d1595a0543560a36b0309d111b362b242adb563a29a`  
		Last Modified: Fri, 14 Aug 2020 22:40:44 GMT  
		Size: 13.5 MB (13540652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8aedd542ef80dea6824b8c86206f3e9c64057dca38cabd8a508176540ea667`  
		Last Modified: Fri, 14 Aug 2020 22:40:44 GMT  
		Size: 4.2 MB (4168217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
