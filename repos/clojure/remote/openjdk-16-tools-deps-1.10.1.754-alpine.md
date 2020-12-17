## `clojure:openjdk-16-tools-deps-1.10.1.754-alpine`

```console
$ docker pull clojure@sha256:38a80585f19ff92b8bceb75e46a2002e859f96e7f39bf8d7512d35fc4464dea7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-tools-deps-1.10.1.754-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:37c2a8edd08b6c278b74794accb6b3836cc80a7495d218bf44b8788964889124
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210574295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8fa11137f8286399c1a5e5f15f29767f7032fb6bffe20f21ca860f5c1d3a81`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:15:27 GMT
RUN apk add --no-cache java-cacerts
# Thu, 17 Dec 2020 13:15:27 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Thu, 17 Dec 2020 13:15:28 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:15:28 GMT
ENV JAVA_VERSION=16-ea+23
# Thu, 17 Dec 2020 13:16:13 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/23/binaries/openjdk-16-ea+23_linux-x64-musl_bin.tar.gz; 			downloadSha256=4e1d9054a4407e63fbb74155b247cf3926cffe9491074ace6d8a51d78dd0958d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Dec 2020 13:16:14 GMT
CMD ["jshell"]
# Thu, 17 Dec 2020 19:23:27 GMT
ENV CLOJURE_VERSION=1.10.1.754
# Thu, 17 Dec 2020 19:23:27 GMT
WORKDIR /tmp
# Thu, 17 Dec 2020 19:23:36 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1c623dd76ea75cb89623ffc71a5ec59297c785c0c19fc5c2fa0fe9428efe8a3d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Thu, 17 Dec 2020 19:23:36 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7f0194508bfdf90c2d4c810091723a528db557a8f15dc3342de6f146b13a31`  
		Last Modified: Thu, 17 Dec 2020 13:21:09 GMT  
		Size: 927.2 KB (927220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12c6ae52764c63121af92fc8ae8af14d42a3a2cbbd239516e262a14c7aca7ac`  
		Last Modified: Thu, 17 Dec 2020 13:21:43 GMT  
		Size: 184.3 MB (184293978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dd5e6ac406086df0fa9d55ffb15cac6282cc5f2bb9293d7a5bb8175c440149`  
		Last Modified: Thu, 17 Dec 2020 19:26:42 GMT  
		Size: 22.6 MB (22554031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
