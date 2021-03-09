## `clojure:openjdk-17-tools-deps-1.10.2.796-alpine`

```console
$ docker pull clojure@sha256:d2cacf93a7309d5e7149fb21462eb21b255b54e49d7dc77ebf5e96be084d2ff6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-tools-deps-1.10.2.796-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:9589c627dbc85ef76cee5b5f4dc34703b732da2af11bab62fcd2f82285b2e6fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.3 MB (213270679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5945d6e958bcba493e4c31e6a27b961edd7623b0ca678a88c1d03a56a8d19ea8`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 09 Mar 2021 20:57:21 GMT
RUN apk add --no-cache java-cacerts
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Tue, 09 Mar 2021 20:57:21 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Mar 2021 20:57:21 GMT
ENV JAVA_VERSION=17-ea+10
# Tue, 09 Mar 2021 20:58:11 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/10/binaries/openjdk-17-ea+10_linux-x64-musl_bin.tar.gz'; 			downloadSha256='fc3ea4225030a5df6191b6027051e705e6c34b72115dfdb36d170d735cb409d5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 09 Mar 2021 20:58:11 GMT
CMD ["jshell"]
# Tue, 09 Mar 2021 21:55:37 GMT
ENV CLOJURE_VERSION=1.10.2.796
# Tue, 09 Mar 2021 21:55:37 GMT
WORKDIR /tmp
# Tue, 09 Mar 2021 21:55:43 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "0ea8633c7f53eb76098132d4a4536169395be24bbdc253cff4d10251e2ea6e45 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 09 Mar 2021 21:55:44 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b1e51638093d53268f8affa33c76d79b5f585556917511babcc02780047d7b`  
		Last Modified: Tue, 09 Mar 2021 21:11:38 GMT  
		Size: 928.4 KB (928404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fccea66d261db26595f6c615d2361af9b26994c460c6b0736185a09e1cb602a`  
		Last Modified: Tue, 09 Mar 2021 21:11:53 GMT  
		Size: 186.9 MB (186889693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd83eeb13d1f8558cdf7b0002432c8ffbd42b0feb80beb4e5741858c006f17`  
		Last Modified: Tue, 09 Mar 2021 22:11:22 GMT  
		Size: 22.6 MB (22640925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
