## `clojure:openjdk-17-boot-alpine`

```console
$ docker pull clojure@sha256:e1531c1b8b7933fb377c92fe83cde710eea60f6a963128261897dd0e1e023e15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-17-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:22103db2c9278f631586604d0e1ea17cd52e9bcd2422c4ca6128955ea200153a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250187357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1355cf66c0bcfd573993e3aab8787d5d9b1f4fbc74f7ce02d3f28db9aaaf4f0f`
-	Default Command: `["boot","repl"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Tue, 22 Jun 2021 21:40:57 GMT
RUN apk add --no-cache java-cacerts
# Tue, 22 Jun 2021 21:40:57 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Tue, 22 Jun 2021 21:40:57 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Jun 2021 21:40:58 GMT
ENV JAVA_VERSION=17-ea+14
# Tue, 22 Jun 2021 21:41:09 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Jun 2021 21:41:09 GMT
CMD ["jshell"]
# Tue, 22 Jun 2021 22:20:42 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 22 Jun 2021 22:20:43 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 22 Jun 2021 22:20:43 GMT
WORKDIR /tmp
# Tue, 22 Jun 2021 22:20:45 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 22 Jun 2021 22:20:45 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 22 Jun 2021 22:20:45 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 22 Jun 2021 22:21:05 GMT
RUN boot
# Tue, 22 Jun 2021 22:21:05 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c9466125e464fed5626bde7b7a0f91aab09905f0a07e9ad4e930ae72e0fc63`  
		Last Modified: Tue, 22 Jun 2021 21:51:51 GMT  
		Size: 928.4 KB (928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d715783b80cab158f5bf9726bcada5265c1624b64ca2bb46f42f94998d4662`  
		Last Modified: Tue, 22 Jun 2021 21:52:05 GMT  
		Size: 186.8 MB (186798299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb6251b4f79391cce666477516e344d70785e8d7cf91984c4d632aec12dfda1`  
		Last Modified: Tue, 22 Jun 2021 22:25:25 GMT  
		Size: 828.8 KB (828780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb4cdbd5a3ae28a002f3de15f3a22e6d3ec1cf9926dba98ee7522ea7b266586`  
		Last Modified: Tue, 22 Jun 2021 22:25:28 GMT  
		Size: 58.8 MB (58820364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
