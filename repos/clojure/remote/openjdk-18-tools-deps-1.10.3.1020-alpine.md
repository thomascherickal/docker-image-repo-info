## `clojure:openjdk-18-tools-deps-1.10.3.1020-alpine`

```console
$ docker pull clojure@sha256:3a45feff707d411311daaae3c868e05789309fd3b535587c0933bcc0b99b8c33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-tools-deps-1.10.3.1020-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:87068c2044d39014950a303b747ff56a0293b18edfb572c301432f9539297c02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.4 MB (218397486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb218e0924ebd153e1187c7d3d2743a1d87159a1f66dbc856e78671c19fdd674`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Wed, 10 Nov 2021 19:30:21 GMT
ENV CLOJURE_VERSION=1.10.3.1020
# Wed, 10 Nov 2021 19:30:22 GMT
WORKDIR /tmp
# Wed, 10 Nov 2021 19:30:27 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "afc87e2c8cfbf87e43553439c69a4c8e36bc2094405d08f39ca542b4cca0920a *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 10 Nov 2021 19:30:27 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:9c00a7b207d996b9ee9f27b4c51c810dbc539e04bc03f4a39cb7111cdb73b4b8`  
		Last Modified: Wed, 10 Nov 2021 19:43:21 GMT  
		Size: 26.0 MB (25954967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
