## `clojure:openjdk-18-tools-deps-alpine`

```console
$ docker pull clojure@sha256:14f6eb9b7e6b7e52aaf4c7e9798abe894106db84fa2c5057e70366d8b5b79e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-tools-deps-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:8409bdcc77fc7631b0ff04e29301c5758a1a419d217f837663ead194e8f1afd1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.4 MB (218354758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ace53af496724c93525b3102d6e0470a4fc0977fc1ba06b11ad9d8d487aef091`
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
# Mon, 01 Nov 2021 22:27:10 GMT
ENV CLOJURE_VERSION=1.10.3.998
# Mon, 01 Nov 2021 22:27:10 GMT
WORKDIR /tmp
# Mon, 01 Nov 2021 22:27:16 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "c58df29f0c919b90282ace43e92fffd914ba50ba619c837d232bbf686f6ee4a8 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Mon, 01 Nov 2021 22:27:16 GMT
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
	-	`sha256:d5dbb4bf9e3fccb7e26690fe6714f81249b8de56f950b1fd185592b68a77e05f`  
		Last Modified: Mon, 01 Nov 2021 22:35:27 GMT  
		Size: 25.9 MB (25912239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
