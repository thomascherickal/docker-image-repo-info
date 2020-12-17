## `clojure:openjdk-16-boot-alpine`

```console
$ docker pull clojure@sha256:0d35ce5b64da87aa255906fe7c82ef424559f2b36defcaff5fa3feab4b39d222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:6b8d474f0df7adc541b375cc8bbfd81e418ebde194c0a28fbcd0e5ffc5c3fb4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.6 MB (247632661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486613d7983309f10be5f9fb7f6bb6fceafeca99c69509b16ff8af06ccd9a4cc`
-	Default Command: `["boot","repl"]`

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
# Thu, 17 Dec 2020 19:23:01 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 17 Dec 2020 19:23:01 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 17 Dec 2020 19:23:02 GMT
WORKDIR /tmp
# Thu, 17 Dec 2020 19:23:03 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Thu, 17 Dec 2020 19:23:03 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Thu, 17 Dec 2020 19:23:03 GMT
ENV BOOT_AS_ROOT=yes
# Thu, 17 Dec 2020 19:23:22 GMT
RUN boot
# Thu, 17 Dec 2020 19:23:22 GMT
CMD ["boot" "repl"]
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
	-	`sha256:58faa70223fb1630fb6f678a2341039d3899912332ee1268457b811c551a7a74`  
		Last Modified: Thu, 17 Dec 2020 19:26:30 GMT  
		Size: 792.3 KB (792332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b3e9b5568fab1653879ea25b1de8cec951d716b227ab758525a6d572ca1836`  
		Last Modified: Thu, 17 Dec 2020 19:26:34 GMT  
		Size: 58.8 MB (58820065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
