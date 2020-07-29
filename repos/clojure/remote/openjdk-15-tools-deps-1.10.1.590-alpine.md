## `clojure:openjdk-15-tools-deps-1.10.1.590-alpine`

```console
$ docker pull clojure@sha256:ecd825e174d8d88166686401f5a7f105c36ad4fd460d935076f1381b9cf0b9ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-15-tools-deps-1.10.1.590-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:b863778366cdff94e9de3a4084053a3eee7b42a04f333e418ccf2454179e1904
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.0 MB (223036342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8edc0758b047403302a675fca4f70f2d7aa77f9dd51d1e2b19afce62edeb1d`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Wed, 29 Jul 2020 02:13:02 GMT
ENV CLOJURE_VERSION=1.10.1.590
# Wed, 29 Jul 2020 02:13:02 GMT
WORKDIR /tmp
# Wed, 29 Jul 2020 02:13:11 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "92a606c1b373ddee338c209f9fecd6f0a40b3354b5eb762962b9cc64f226ce53 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Wed, 29 Jul 2020 02:13:11 GMT
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
	-	`sha256:fc5eabcede3645338ce4f48b82a9c70a12f11b8d569a562c1ce54a7e670b0e98`  
		Last Modified: Wed, 29 Jul 2020 01:34:52 GMT  
		Size: 196.8 MB (196791691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bc22842ae75ee7cc34ee9036f603358c61e91143947b568ebbffd0683967c1`  
		Last Modified: Wed, 29 Jul 2020 02:18:19 GMT  
		Size: 22.5 MB (22520709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
