## `clojure:openjdk-14-lein-2.9.3`

```console
$ docker pull clojure@sha256:dc842c682c3076acb883787e26175f470e1cf6b25b219ed3a578ccc03d969834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-14-lein-2.9.3` - linux; amd64

```console
$ docker pull clojure@sha256:7b04f3312796e039a77dfee91cf79a25ab3942dbe5d2a7e2d953b547a464ec1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.4 MB (247437326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058e4f36bc76abe0b4969b676a3a5b726fd7149412af83ed5c45512d5b9a4826`
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
# Wed, 05 Aug 2020 00:43:56 GMT
ENV JAVA_HOME=/usr/local/openjdk-14
# Wed, 05 Aug 2020 00:43:57 GMT
ENV PATH=/usr/local/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Aug 2020 00:43:57 GMT
RUN { echo '#/bin/sh'; echo 'echo "$JAVA_HOME"'; } > /usr/local/bin/docker-java-home && chmod +x /usr/local/bin/docker-java-home && [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Wed, 05 Aug 2020 00:43:58 GMT
ENV JAVA_VERSION=14.0.2
# Tue, 01 Sep 2020 01:49:24 GMT
RUN set -eux; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk14.0.2/205943a0976c4ed48cb16f1043c5c647/12/GPL/openjdk-14.0.2_linux-x64_bin.tar.gz; 			downloadSha256=91310200f072045dc6cef2c8c23e7e6387b37c46e9de49623ce0fa461a24623d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O openjdk.tgz "$downloadUrl" --progress=dot:giga; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		{ 		echo '#!/usr/bin/env bash'; 		echo 'set -Eeuo pipefail'; 		echo 'if ! [ -d "$JAVA_HOME" ]; then echo >&2 "error: missing JAVA_HOME environment variable"; exit 1; fi'; 		echo 'cacertsFile=; for f in "$JAVA_HOME/lib/security/cacerts" "$JAVA_HOME/jre/lib/security/cacerts"; do if [ -e "$f" ]; then cacertsFile="$f"; break; fi; done'; 		echo 'if [ -z "$cacertsFile" ] || ! [ -f "$cacertsFile" ]; then echo >&2 "error: failed to find cacerts file in $JAVA_HOME"; exit 1; fi'; 		echo 'trust extract --overwrite --format=java-cacerts --filter=ca-anchors --purpose=server-auth "$cacertsFile"'; 	} > /etc/ca-certificates/update.d/docker-openjdk; 	chmod +x /etc/ca-certificates/update.d/docker-openjdk; 	/etc/ca-certificates/update.d/docker-openjdk; 		find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf; 	ldconfig; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 01 Sep 2020 01:49:24 GMT
CMD ["jshell"]
# Tue, 01 Sep 2020 21:12:21 GMT
ENV LEIN_VERSION=2.9.3
# Tue, 01 Sep 2020 21:12:21 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 01 Sep 2020 21:12:21 GMT
WORKDIR /tmp
# Tue, 01 Sep 2020 21:12:31 GMT
RUN apt-get update && apt-get install -y gnupg wget && rm -rf /var/lib/apt/lists/* && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apt-get purge -y --auto-remove gnupg wget
# Tue, 01 Sep 2020 21:12:31 GMT
ENV PATH=/usr/local/openjdk-14/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 01 Sep 2020 21:12:31 GMT
ENV LEIN_ROOT=1
# Tue, 01 Sep 2020 21:12:35 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Tue, 01 Sep 2020 21:12:35 GMT
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
	-	`sha256:082613a53f6f3cc6ad3fd90239b67d05131147909cfc0d1b075a7262a295ed0f`  
		Last Modified: Wed, 05 Aug 2020 00:50:11 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb778f76db35302bb48fef9517abc09b6ff8ad7f6985f482b2ccbfa48c6e800`  
		Last Modified: Tue, 01 Sep 2020 02:00:01 GMT  
		Size: 199.5 MB (199465062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f94548dacf5982ad86fac0ec24e2d2cb581e9dd223bbfe04cc3eca21b5f096f`  
		Last Modified: Tue, 01 Sep 2020 21:21:52 GMT  
		Size: 13.5 MB (13463340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc88d75d38a90805bf13e7e571b04dbb17f74557c2afc1d8e0dd72376fb10d6`  
		Last Modified: Tue, 01 Sep 2020 21:21:52 GMT  
		Size: 4.2 MB (4168161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
