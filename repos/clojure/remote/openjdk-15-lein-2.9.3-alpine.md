## `clojure:openjdk-15-lein-2.9.3-alpine`

```console
$ docker pull clojure@sha256:733430553abe17f95ea6d47de1510123685f59ead7e09663f6b9e46c0a711a1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-lein-2.9.3-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:d6a03ef67e1d15bc276c52750da971fd6725162e7d93042b69fb500caeee0aa2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218650678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21ba9fa563359bd96fbaa84f6a79e8455bb452bac781605d7b29921aa43ffb51`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:05:44 GMT
RUN apk add --no-cache java-cacerts
# Wed, 22 Jul 2020 01:07:14 GMT
ENV JAVA_HOME=/opt/openjdk-15
# Wed, 22 Jul 2020 01:07:14 GMT
ENV PATH=/opt/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 01:07:14 GMT
ENV JAVA_VERSION=15-ea+31
# Wed, 29 Jul 2020 01:27:32 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/31/binaries/openjdk-15-ea+31_linux-x64-musl_bin.tar.gz; 			downloadSha256=da7abd4d3b3511ed2da8aba25b7ff67863261a0c8b5e7e771cf0fbfadcc7f4fd; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		javac --version; 	java --version
# Wed, 29 Jul 2020 01:27:32 GMT
CMD ["jshell"]
# Wed, 29 Jul 2020 02:12:25 GMT
ENV LEIN_VERSION=2.9.3
# Wed, 29 Jul 2020 02:12:25 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Wed, 29 Jul 2020 02:12:25 GMT
WORKDIR /tmp
# Wed, 29 Jul 2020 02:12:28 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Wed, 29 Jul 2020 02:12:28 GMT
ENV PATH=/opt/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Jul 2020 02:12:28 GMT
ENV LEIN_ROOT=1
# Wed, 29 Jul 2020 02:12:32 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Wed, 29 Jul 2020 02:12:33 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a2e4aad8c98294e53534e7aef0572d7a04cc37264f1b4b75d0878244e59c7f`  
		Last Modified: Wed, 22 Jul 2020 01:13:01 GMT  
		Size: 926.4 KB (926401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5eabcede3645338ce4f48b82a9c70a12f11b8d569a562c1ce54a7e670b0e98`  
		Last Modified: Wed, 29 Jul 2020 01:34:52 GMT  
		Size: 196.8 MB (196791691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ca9b7c8992a0cfe5e0920b71127740ddd93ba508c43e527e8ca1964416c1ed`  
		Last Modified: Wed, 29 Jul 2020 02:18:02 GMT  
		Size: 14.0 MB (13966825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260e0d77976108126bc9c2b3a07f26ffff869cf0f30c9994ad590bc77ab9957d`  
		Last Modified: Wed, 29 Jul 2020 02:18:02 GMT  
		Size: 4.2 MB (4168220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
