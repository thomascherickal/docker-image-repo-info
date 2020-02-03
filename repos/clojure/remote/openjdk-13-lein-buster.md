## `clojure:openjdk-13-lein-buster`

```console
$ docker pull clojure@sha256:38b4f9ac410d73332a35052397f37605a2878ef243bea0bfe66ac71cbc829920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-13-lein-buster` - linux; amd64

```console
$ docker pull clojure@sha256:923dc55992047835a84e670f8c21026786bb4c9a5114ed0f9fc69cdbd774649e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.6 MB (347613307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79ec109f199de939c7114517effb2ade8a318297fecf4ea926e89e98c38e0ec8`
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
# Sun, 02 Feb 2020 06:23:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-13
# Sun, 02 Feb 2020 06:23:50 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 06:23:51 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Sun, 02 Feb 2020 06:23:52 GMT
ENV JAVA_VERSION=13.0.2
# Sun, 02 Feb 2020 06:23:52 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_linux-x64_bin.tar.gz
# Sun, 02 Feb 2020 06:23:54 GMT
ENV JAVA_SHA256=acc7a6aabced44e62ec3b83e3b5959df2b1aa6b3d610d58ee45f0c21a7821a71
# Sun, 02 Feb 2020 06:25:23 GMT
RUN set -eux; 		wget -O openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		javac --version; 	java --version
# Sun, 02 Feb 2020 06:25:23 GMT
CMD ["jshell"]
# Sun, 02 Feb 2020 21:39:23 GMT
ENV LEIN_VERSION=2.9.1
# Sun, 02 Feb 2020 21:39:23 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Sun, 02 Feb 2020 21:39:23 GMT
WORKDIR /tmp
# Sun, 02 Feb 2020 21:40:23 GMT
RUN mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha1sum lein-pkg && echo "93be2c23ab4ff2fc4fcf531d7510ca4069b8d24a *lein-pkg" | sha1sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver pool.sks-keyservers.net --recv-key 2B72BF956E23DE5E830D50F6002AF007D1A7CC18 && echo "Verifying Jar file signature ..." && gpg --verify leiningen-$LEIN_VERSION-standalone.zip.asc && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar
# Sun, 02 Feb 2020 21:40:24 GMT
ENV PATH=/usr/java/openjdk-13/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Sun, 02 Feb 2020 21:40:24 GMT
ENV LEIN_ROOT=1
# Sun, 02 Feb 2020 21:40:28 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Sun, 02 Feb 2020 21:40:29 GMT
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
	-	`sha256:01286c8a7cf2926a8de065c8ab0c4b20bebe6e4c657cf1ba5a3a72cb7ab08f87`  
		Last Modified: Sun, 02 Feb 2020 06:33:51 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81d7b0358c3372af6ed349a23cbe8375ec66186f14e7b7882477debdd5775e9`  
		Last Modified: Sun, 02 Feb 2020 06:34:17 GMT  
		Size: 196.4 MB (196408144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb9dde83ae927e055f82813ca5aa14cbb8151d96574d88a3391b0246e435b83`  
		Last Modified: Sun, 02 Feb 2020 21:49:14 GMT  
		Size: 13.1 MB (13137772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff8f3757c86aecd9c20ee3904b7b1008206cf6fd8f1843699ca01506cffea6`  
		Last Modified: Sun, 02 Feb 2020 21:49:11 GMT  
		Size: 4.2 MB (4168232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
