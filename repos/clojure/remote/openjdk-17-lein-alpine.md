## `clojure:openjdk-17-lein-alpine`

```console
$ docker pull clojure@sha256:c67b9d8a6521b9edac031a922feab3c4b5f6d5a1128934856c02c1ea5afcfb72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-lein-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:ebaf802e6691b2291fe38ff0fddf1fe9e8d7e3fc6792ff4cfa1e15697eccbfd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207170309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd6287bde67d2d98f7bc98e2acc927e312eff39ae8e4614d0650c33d0bf50a9`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Thu, 18 Feb 2021 05:42:40 GMT
RUN apk add --no-cache java-cacerts
# Thu, 18 Feb 2021 05:42:40 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Thu, 18 Feb 2021 05:42:40 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Feb 2021 23:23:06 GMT
ENV JAVA_VERSION=17-ea+10
# Thu, 18 Feb 2021 23:23:53 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 18 Feb 2021 23:23:53 GMT
CMD ["jshell"]
# Mon, 22 Feb 2021 22:27:09 GMT
ENV LEIN_VERSION=2.9.5
# Mon, 22 Feb 2021 22:27:09 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Mon, 22 Feb 2021 22:27:10 GMT
WORKDIR /tmp
# Mon, 22 Feb 2021 22:27:13 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Mon, 22 Feb 2021 22:27:13 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Mon, 22 Feb 2021 22:27:13 GMT
ENV LEIN_ROOT=1
# Wed, 24 Feb 2021 18:28:30 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.2"]])' > project.clj   && lein deps && rm project.clj
# Wed, 24 Feb 2021 18:28:30 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155cb13c45d5b09951cf0b8e75c365b37550dce6b8ca7c5532d4bd491dd8f3f6`  
		Last Modified: Thu, 18 Feb 2021 05:48:13 GMT  
		Size: 928.2 KB (928245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f816cf83573c02fcf997a8bb0bae3065810e052f3e24cd800d48eb88ebd6b9`  
		Last Modified: Thu, 18 Feb 2021 23:29:59 GMT  
		Size: 186.9 MB (186889522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fc747e17bd0bf041e67fc0c76d3c6d24ed8d594822d9e245c63fcedecc95e`  
		Last Modified: Mon, 22 Feb 2021 22:32:35 GMT  
		Size: 12.3 MB (12335868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240fdc7d24645175d2d7dc95d61e6ab56106e41e3a8752ad238354c333360fbd`  
		Last Modified: Wed, 24 Feb 2021 18:34:57 GMT  
		Size: 4.2 MB (4205017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
