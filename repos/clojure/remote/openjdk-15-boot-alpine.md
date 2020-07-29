## `clojure:openjdk-15-boot-alpine`

```console
$ docker pull clojure@sha256:4e4406433955c3391abb02172bbccbc4a9421836a7de8a0c533c57cb9cb62071
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:595e13f72b5f0a64128ab27d5c145b535265c2a75a28105cf6622dc27978b7a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.1 MB (260127970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e3625466edd0c621f269c3de7aeea7b96fee979b15250edb47dcf719f9da94`
-	Default Command: `["boot","repl"]`

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
# Wed, 29 Jul 2020 02:12:37 GMT
ENV BOOT_VERSION=2.8.3
# Wed, 29 Jul 2020 02:12:37 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Wed, 29 Jul 2020 02:12:37 GMT
WORKDIR /tmp
# Wed, 29 Jul 2020 02:12:39 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Wed, 29 Jul 2020 02:12:39 GMT
ENV PATH=/opt/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Wed, 29 Jul 2020 02:12:39 GMT
ENV BOOT_AS_ROOT=yes
# Wed, 29 Jul 2020 02:12:57 GMT
RUN boot
# Wed, 29 Jul 2020 02:12:57 GMT
CMD ["boot" "repl"]
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
	-	`sha256:5adc76b8fed903c335022532726042117cf3a0238d33f236a858d17f1f01439e`  
		Last Modified: Wed, 29 Jul 2020 02:18:06 GMT  
		Size: 792.3 KB (792334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabe1e28fa58dbd8125545b5e91dd0fed09e42c70ecd2c28385b3deade2e373d`  
		Last Modified: Wed, 29 Jul 2020 02:18:14 GMT  
		Size: 58.8 MB (58820003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
