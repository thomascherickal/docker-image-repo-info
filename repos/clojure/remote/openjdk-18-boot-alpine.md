## `clojure:openjdk-18-boot-alpine`

```console
$ docker pull clojure@sha256:274f6cbe2c5a21bf434867921452a65805a6af1fe2966feb3e0b0932211c90d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:84f4cc535fa0003158e9bfc6307987f2f8bd42c7975cd43cbe6991853a1b7ed3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252091593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb048cc72773c2ee23ec89d42029d164ed961f483c82017734fe58577718d1b`
-	Default Command: `["boot","repl"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 17:32:24 GMT
RUN apk add --no-cache java-cacerts
# Fri, 27 Aug 2021 17:32:24 GMT
ENV JAVA_HOME=/opt/openjdk-18
# Fri, 27 Aug 2021 17:32:24 GMT
ENV PATH=/opt/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 17:32:25 GMT
ENV JAVA_VERSION=18-ea+11
# Fri, 27 Aug 2021 17:32:36 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/11/binaries/openjdk-18-ea+11_linux-x64-musl_bin.tar.gz'; 			downloadSha256='86fad9069587a5e9dd003e7354a69b2f720a05c12706d2f2345a0c8d90e56c47'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 27 Aug 2021 17:32:36 GMT
CMD ["jshell"]
# Thu, 09 Sep 2021 19:35:20 GMT
ENV BOOT_VERSION=2.8.3
# Thu, 09 Sep 2021 19:35:20 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Thu, 09 Sep 2021 19:35:20 GMT
WORKDIR /tmp
# Wed, 29 Sep 2021 08:21:19 GMT
RUN apk add --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Wed, 29 Sep 2021 08:21:19 GMT
ENV PATH=/opt/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Sep 2021 08:21:19 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 29 Sep 2021 08:21:39 GMT
RUN boot
# Wed, 29 Sep 2021 08:21:39 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79fb3f4ca2289d42dd52c21c56c23417196696f2696abbcdedada7306f552ca`  
		Last Modified: Fri, 27 Aug 2021 17:42:52 GMT  
		Size: 928.4 KB (928417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d1a4c2ebf908279e849340d10f4eb1cb7fdd9fc8468e6ab2f77544ec171985`  
		Last Modified: Fri, 27 Aug 2021 17:43:11 GMT  
		Size: 188.7 MB (188699656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03a4d54dda17664c4c998dd28ddb41a28035c09ffc3a7000ae99eb87c1bf97a`  
		Last Modified: Wed, 29 Sep 2021 08:42:35 GMT  
		Size: 828.8 KB (828800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e318df884867a8a0c58409ce25336271877e9ef7aa28af82af5018a38b92b368`  
		Last Modified: Wed, 29 Sep 2021 08:42:38 GMT  
		Size: 58.8 MB (58820274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
