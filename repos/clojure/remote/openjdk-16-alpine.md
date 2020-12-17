## `clojure:openjdk-16-alpine`

```console
$ docker pull clojure@sha256:f36709ec90e844b49f9af544b90c26fd15e662ed109c13b7bbd4e231e2c84501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:e3354f2dc0cf8497903fa0ce1f1b57558215352c73298224d999edc1b8f8800c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.5 MB (204502025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03430e112be01352ecc6c9bb3d4d1497178c2b1cc6af519d243724f6aba1cd68`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:15:27 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Dec 2020 13:15:27 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Thu, 17 Dec 2020 13:15:28 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:15:28 GMT
ENV JAVA_VERSION=16-ea+23
# Thu, 17 Dec 2020 13:16:13 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/23/binaries/openjdk-16-ea+23_linux-x64-musl_bin.tar.gz; 			downloadSha256=4e1d9054a4407e63fbb74155b247cf3926cffe9491074ace6d8a51d78dd0958d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Dec 2020 13:16:14 GMT
CMD ["jshell"]
# Thu, 17 Dec 2020 19:22:47 GMT
ENV LEIN_VERSION=2.9.5
# Thu, 17 Dec 2020 19:22:47 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Thu, 17 Dec 2020 19:22:48 GMT
WORKDIR /tmp
# Thu, 17 Dec 2020 19:22:51 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Thu, 17 Dec 2020 19:22:51 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 17 Dec 2020 19:22:52 GMT
ENV LEIN_ROOT=1
# Thu, 17 Dec 2020 19:22:56 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.1"]])' > project.clj   && lein deps && rm project.clj
# Thu, 17 Dec 2020 19:22:56 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7f0194508bfdf90c2d4c810091723a528db557a8f15dc3342de6f146b13a31`  
		Last Modified: Thu, 17 Dec 2020 13:21:09 GMT  
		Size: 927.2 KB (927220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12c6ae52764c63121af92fc8ae8af14d42a3a2cbbd239516e262a14c7aca7ac`  
		Last Modified: Thu, 17 Dec 2020 13:21:43 GMT  
		Size: 184.3 MB (184293978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2276b91699348ad858fc6e33cc8604bbfc22f7585ddeae488a95842eb882d1`  
		Last Modified: Thu, 17 Dec 2020 19:26:22 GMT  
		Size: 12.3 MB (12301556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e550778b4d0c7a22dfb1cfa8aca15c1f3a72c8942569066316f4c4bcff9441`  
		Last Modified: Thu, 17 Dec 2020 19:26:21 GMT  
		Size: 4.2 MB (4180205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
