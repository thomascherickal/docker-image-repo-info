## `clojure:openjdk-16-boot-alpine`

```console
$ docker pull clojure@sha256:a402711b3c3ae1c5d6d87a6b321dcb65a280a3d0d52fa74015fc09b4e5b344ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:aa2d59e181a734393e18c5bca8a20caa1f9143d315627618cf55d43996a174a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.8 MB (260793117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a6e2556938267a650ea1a03c172634ad23715544d3e79856a691f25f8e4e7db`
-	Default Command: `["boot","repl"]`

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
# Fri, 14 Aug 2020 21:25:52 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 14 Aug 2020 21:25:52 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 14 Aug 2020 21:25:53 GMT
WORKDIR /tmp
# Fri, 14 Aug 2020 21:25:55 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 14 Aug 2020 21:25:55 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 14 Aug 2020 21:25:56 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 14 Aug 2020 21:26:31 GMT
RUN boot
# Fri, 14 Aug 2020 21:26:32 GMT
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
	-	`sha256:3ad14fdcda01da7c472fc488405c040d3b90afda31db2232d0a657edf2a86ab2`  
		Last Modified: Wed, 29 Jul 2020 01:33:12 GMT  
		Size: 197.5 MB (197456503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be848cbbd911885260c54db59002ffa2c2a93879b47e4b1b1df03f40eebe8155`  
		Last Modified: Fri, 14 Aug 2020 21:30:30 GMT  
		Size: 792.3 KB (792325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb6bc9451559514f61bd4fea914dec543197faadbd7fa42b189cf1c556fa4dd`  
		Last Modified: Fri, 14 Aug 2020 21:30:35 GMT  
		Size: 58.8 MB (58820347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
