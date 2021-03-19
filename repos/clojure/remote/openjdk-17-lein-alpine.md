## `clojure:openjdk-17-lein-alpine`

```console
$ docker pull clojure@sha256:f5df5fd2b25c1e30c4ca7f34ca0c152ba0963817f1343f2b364deb20641f794f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-lein-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:b7a26998ce5ff34d6e9d3473387dba444e37bc703e064c7cab475f40d816b2d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.2 MB (207169439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dc1ee4a68518b17fcc81b5f2fd62899a6211f37accd1d25038911d9c1c9a032`
-	Default Command: `["lein","repl"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 20:57:21 GMT
RUN apk add --no-cache java-cacerts
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Tue, 09 Mar 2021 20:57:21 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_VERSION=17-ea+10
# Tue, 09 Mar 2021 20:58:11 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:58:11 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:54:58 GMT
ENV LEIN_VERSION=2.9.5
# Tue, 09 Mar 2021 21:54:58 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Tue, 09 Mar 2021 21:54:58 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:55:04 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Tue, 09 Mar 2021 21:55:04 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 09 Mar 2021 21:55:04 GMT
ENV LEIN_ROOT=1
# Fri, 19 Mar 2021 18:59:06 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 19 Mar 2021 18:59:06 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b1e51638093d53268f8affa33c76d79b5f585556917511babcc02780047d7b`  
		Last Modified: Tue, 09 Mar 2021 21:11:38 GMT  
		Size: 928.4 KB (928404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fccea66d261db26595f6c615d2361af9b26994c460c6b0736185a09e1cb602a`  
		Last Modified: Tue, 09 Mar 2021 21:11:53 GMT  
		Size: 186.9 MB (186889693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae2fedc6e1ac0e0b37ab96e8bb8b617e54656dc90aef86e07a204bde3779fb2`  
		Last Modified: Tue, 09 Mar 2021 22:10:44 GMT  
		Size: 12.3 MB (12335959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd240dc2c7f3ddb537e405f580ab6ea5b3f1e5475b385a606b2c0948c6d34150`  
		Last Modified: Fri, 19 Mar 2021 19:09:36 GMT  
		Size: 4.2 MB (4203726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
