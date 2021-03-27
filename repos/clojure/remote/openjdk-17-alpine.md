## `clojure:openjdk-17-alpine`

```console
$ docker pull clojure@sha256:0c7d75cf5dd03535cbe51cca0f43ddcfacca158f26e27bd64bc522a8be4cb6aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:cfbcdcf77332d39c8679d01f7a17a97baf305b5ccd42f7075cedc03d4bb21a28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.1 MB (207077983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2392d7f8dee29c0cfcaa05bd041dce403c6d9743f525adb97c7665a6abadf5ee`
-	Default Command: `["lein","repl"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:43:36 GMT
RUN apk add --no-cache java-cacerts
# Fri, 26 Mar 2021 05:43:36 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Fri, 26 Mar 2021 05:43:36 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 05:43:37 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 26 Mar 2021 05:43:50 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 05:43:51 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:13:51 GMT
ENV LEIN_VERSION=2.9.5
# Fri, 26 Mar 2021 20:13:51 GMT
ENV LEIN_INSTALL=/usr/local/bin/
# Fri, 26 Mar 2021 20:13:52 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:13:57 GMT
RUN apk add --update --no-cache ca-certificates bash tar openssl gnupg && mkdir -p $LEIN_INSTALL && wget -q https://raw.githubusercontent.com/technomancy/leiningen/$LEIN_VERSION/bin/lein-pkg && echo "Comparing lein-pkg checksum ..." && sha256sum lein-pkg && echo "3601d55c4b5ac5c654e4ebd0d75abf7ad683f48cba8a7af1a8730b6590187b8a *lein-pkg" | sha256sum -c - && mv lein-pkg $LEIN_INSTALL/lein && chmod 0755 $LEIN_INSTALL/lein && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip && wget -q https://github.com/technomancy/leiningen/releases/download/$LEIN_VERSION/leiningen-$LEIN_VERSION-standalone.zip.asc && gpg --batch --keyserver keys.openpgp.org --recv-key 20242BACBBE95ADA22D0AFD7808A33D379C806C3 && echo "Verifying file PGP signature..." && gpg --batch --verify leiningen-$LEIN_VERSION-standalone.zip.asc leiningen-$LEIN_VERSION-standalone.zip && rm leiningen-$LEIN_VERSION-standalone.zip.asc && mkdir -p /usr/share/java && mv leiningen-$LEIN_VERSION-standalone.zip /usr/share/java/leiningen-$LEIN_VERSION-standalone.jar && apk del ca-certificates tar openssl gnupg
# Fri, 26 Mar 2021 20:13:57 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Mar 2021 20:13:57 GMT
ENV LEIN_ROOT=1
# Fri, 26 Mar 2021 20:14:01 GMT
RUN echo '(defproject dummy "" :dependencies [[org.clojure/clojure "1.10.3"]])' > project.clj   && lein deps && rm project.clj
# Fri, 26 Mar 2021 20:14:02 GMT
CMD ["lein" "repl"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dcb53f37ee333acb4da15f3a4b5ffb66f4b09ce5572a4289f76c2812b07695`  
		Last Modified: Fri, 26 Mar 2021 05:51:31 GMT  
		Size: 928.4 KB (928432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2be41bd5e99b388651a581c5d5b7bd81fcdab12764553d7e30e126e19d6b5bc`  
		Last Modified: Fri, 26 Mar 2021 05:51:50 GMT  
		Size: 186.8 MB (186798158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7d843407a9018598fcb2c966b08bb9af87afb085710451fedc0f13cd728d57`  
		Last Modified: Fri, 26 Mar 2021 20:24:07 GMT  
		Size: 12.3 MB (12335993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b9af227df14b990fa67d69e7843f9a623d6241f88c838968d17b5be112425b`  
		Last Modified: Fri, 26 Mar 2021 20:24:05 GMT  
		Size: 4.2 MB (4203719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
