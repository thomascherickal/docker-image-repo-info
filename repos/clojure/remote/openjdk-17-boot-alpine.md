## `clojure:openjdk-17-boot-alpine`

```console
$ docker pull clojure@sha256:cafa08d907739dc33ec2d3dbebe592675820ab8211b494d3d882bc3394886fda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-17-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:2738f5629174b8a1e5060d93528cbc17c81a3b9c69b2fe5898d5aeedd2aab043
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250187138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf2b5b90596f2b2ef9e01117822020d4211bcedbeb7fb2306375caf00c597cfd`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 05:43:36 GMT
RUN apk add --no-cache java-cacerts
# Fri, 26 Mar 2021 05:43:36 GMT
ENV JAVA_HOME=/opt/openjdk-17
# Fri, 26 Mar 2021 05:43:36 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Mar 2021 05:43:37 GMT
ENV JAVA_VERSION=17-ea+14
# Fri, 26 Mar 2021 05:43:50 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/14/binaries/openjdk-17-ea+14_linux-x64-musl_bin.tar.gz'; 			downloadSha256='f07a1ac921333dafac1cd886ad49600ce143be7efebd32e1a02599a8a0829dd4'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 Mar 2021 05:43:51 GMT
CMD ["jshell"]
# Fri, 26 Mar 2021 20:14:05 GMT
ENV BOOT_VERSION=2.8.3
# Fri, 26 Mar 2021 20:14:06 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Fri, 26 Mar 2021 20:14:06 GMT
WORKDIR /tmp
# Fri, 26 Mar 2021 20:14:08 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Fri, 26 Mar 2021 20:14:08 GMT
ENV PATH=/opt/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Fri, 26 Mar 2021 20:14:08 GMT
ENV BOOT_AS_ROOT=yes
# Fri, 26 Mar 2021 20:14:31 GMT
RUN boot
# Fri, 26 Mar 2021 20:14:31 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dcb53f37ee333acb4da15f3a4b5ffb66f4b09ce5572a4289f76c2812b07695`  
		Last Modified: Fri, 26 Mar 2021 05:51:31 GMT  
		Size: 928.4 KB (928432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2be41bd5e99b388651a581c5d5b7bd81fcdab12764553d7e30e126e19d6b5bc`  
		Last Modified: Fri, 26 Mar 2021 05:51:50 GMT  
		Size: 186.8 MB (186798158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726385d0fa545dbc6278ad55ad186d62a70a4be55bba29c3a4bfe020841369c7`  
		Last Modified: Fri, 26 Mar 2021 20:24:28 GMT  
		Size: 828.4 KB (828429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc02a9f35c2d3440ac696336ee09b1a7c71ceb42a120bb2b377f355d9293109`  
		Last Modified: Fri, 26 Mar 2021 20:24:35 GMT  
		Size: 58.8 MB (58820438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
