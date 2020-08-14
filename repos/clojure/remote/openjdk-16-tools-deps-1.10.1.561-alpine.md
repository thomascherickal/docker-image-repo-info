## `clojure:openjdk-16-tools-deps-1.10.1.561-alpine`

```console
$ docker pull clojure@sha256:434c19e284b2708dc3a7e644210efb2e03fe3f0c05a0ec0883cad1d9389de9a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-tools-deps-1.10.1.561-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:d05fb00a3f7854f750bacc80a5fe1d7e6950c910746e7a75c97cf110782038d2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223703187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df168c7df63524040ea6a45445a6e2cc27cd8b978d51e15a271b152fac473f86`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Fri, 14 Aug 2020 21:26:39 GMT
ENV CLOJURE_VERSION=1.10.1.619
# Fri, 14 Aug 2020 21:26:40 GMT
WORKDIR /tmp
# Fri, 14 Aug 2020 21:26:56 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "28b1652686426cdf856f83551b8ca01ff949b03bc9a533d270204d6511a8ca9d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Fri, 14 Aug 2020 21:26:57 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:44549619b2a481aa885e8ef23df4acb9b3d073e1170538cbc8becd67cdc5f910`  
		Last Modified: Fri, 14 Aug 2020 21:30:42 GMT  
		Size: 22.5 MB (22522742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
