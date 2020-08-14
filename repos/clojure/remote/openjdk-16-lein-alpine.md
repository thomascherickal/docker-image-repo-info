## `clojure:openjdk-16-lein-alpine`

```console
$ docker pull clojure@sha256:8db6816fbaf5f64301491564e24570c24e1e37cbfd76de6d42570d397fc901e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-lein-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:0fbf50c7056c7b19c4a02518ad15f561a776370d6694b4f073dda58c8f749639
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.3 MB (219315493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc69ba6b24fca56978b74c2904a7f52d2a433907a23a16cde6746387b7608745`
-	Default Command: `["lein","repl"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:05:44 GMT
RUN apk add --no-cache java-cacerts
# Wed, 22 Jul 2020 01:05:44 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Wed, 22 Jul 2020 01:05:45 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 01:05:45 GMT
ENV JAVA_VERSION=16-ea+5
# Wed, 29 Jul 2020 01:24:50 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/5/binaries/openjdk-16-ea+5_linux-x64-musl_bin.tar.gz; 			downloadSha256=1ec940bea148a7ececda635c209de3836fe4e6511f5d49d4248cf6d52c77aac8; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		javac --version; 	java --version
# Wed, 29 Jul 2020 01:24:51 GMT
CMD ["jshell"]
# Fri, 14 Aug 2020 21:25:33 GMT
ENV LEIN_VERSION=2.9.3
# Fri, 14 Aug 2020 21:25:33 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 14 Aug 2020 21:25:33 GMT
WORKDIR /tmp
# Fri, 14 Aug 2020 21:25:38 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "42e18e8a833b863ddfba1c5565bd5d78b54bcee661ec86e94a8bdc67b1733e63 *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Fri, 14 Aug 2020 21:25:38 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 14 Aug 2020 21:25:39 GMT
ENV LEIN_ROOT=1
# Fri, 14 Aug 2020 21:25:46 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Fri, 14 Aug 2020 21:25:46 GMT
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
	-	`sha256:3ad14fdcda01da7c472fc488405c040d3b90afda31db2232d0a657edf2a86ab2`  
		Last Modified: Wed, 29 Jul 2020 01:33:12 GMT  
		Size: 197.5 MB (197456503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6347f44589e858b8ac43a1ab0eb54b75724bfa7d3f92b9d11c1ac5ce0b9b07fe`  
		Last Modified: Fri, 14 Aug 2020 21:30:25 GMT  
		Size: 14.0 MB (13966809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ed9b03755683b262050a5654a57f9230af47f2ae7398f26cda660ed8b1fb3b`  
		Last Modified: Fri, 14 Aug 2020 21:30:24 GMT  
		Size: 4.2 MB (4168239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
