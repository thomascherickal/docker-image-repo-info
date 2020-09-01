## `clojure:openjdk-16-tools-deps-1.10.1.561-alpine`

```console
$ docker pull clojure@sha256:9bf9d24a534f7fbac9e03ffad9b2d4762394ed7e7c1bf08bcd78fb31f10ce45e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-tools-deps-1.10.1.561-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:27e644d94829b0fbd02572ae7b88b664186d6f28f2380e1b986e931c77301624
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223703249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3760945a40b7afec5d2ea468939736e602bd292dc56226cec17be75994c26b19`
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
# Tue, 01 Sep 2020 01:44:22 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/5/binaries/openjdk-16-ea+5_linux-x64-musl_bin.tar.gz; 			downloadSha256=1ec940bea148a7ececda635c209de3836fe4e6511f5d49d4248cf6d52c77aac8; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 01 Sep 2020 01:44:22 GMT
CMD ["jshell"]
# Tue, 01 Sep 2020 21:19:47 GMT
ENV CLOJURE_VERSION=1.10.1.619
# Tue, 01 Sep 2020 21:19:48 GMT
WORKDIR /tmp
# Tue, 01 Sep 2020 21:19:56 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "28b1652686426cdf856f83551b8ca01ff949b03bc9a533d270204d6511a8ca9d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 01 Sep 2020 21:19:56 GMT
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
	-	`sha256:db897018b4b7f77d0385f8d927829815841e840a5c7b293a8f540a58a2420aaa`  
		Last Modified: Tue, 01 Sep 2020 01:55:28 GMT  
		Size: 197.5 MB (197456532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f515ff78161a0b36be8da421e10c9efc93f6ebdffab7059d259e74668576af57`  
		Last Modified: Tue, 01 Sep 2020 21:24:28 GMT  
		Size: 22.5 MB (22522775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
