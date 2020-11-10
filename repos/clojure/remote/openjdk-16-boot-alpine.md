## `clojure:openjdk-16-boot-alpine`

```console
$ docker pull clojure@sha256:8e38dc1f49a423f61030ca6547fc96389ce8694481b8a36ce6b37c5693b1a7cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-boot-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:8505e1e8ce40a6051f15220aefa3fe8391df3a039762294a3310492f5963d6a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.6 MB (247629425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f8c160ec4ee64c31ded1ba1984129ba115dc58cfe0d3437d5d5c68c0233054`
-	Default Command: `["boot","repl"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:36:52 GMT
RUN apk add --no-cache java-cacerts
# Thu, 22 Oct 2020 02:36:52 GMT
ENV JAVA_HOME=/opt/openjdk-16
# Thu, 22 Oct 2020 02:36:52 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Nov 2020 00:22:52 GMT
ENV JAVA_VERSION=16-ea+23
# Tue, 10 Nov 2020 00:23:56 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		x86_64) 			downloadUrl=https://download.java.net/java/early_access/alpine/23/binaries/openjdk-16-ea+23_linux-x64-musl_bin.tar.gz; 			downloadSha256=4e1d9054a4407e63fbb74155b247cf3926cffe9491074ace6d8a51d78dd0958d; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 10 Nov 2020 00:23:57 GMT
CMD ["jshell"]
# Tue, 10 Nov 2020 00:46:12 GMT
ENV BOOT_VERSION=2.8.3
# Tue, 10 Nov 2020 00:46:12 GMT
ENV BOOT_INSTALL=/usr/local/bin/
# Tue, 10 Nov 2020 00:46:12 GMT
WORKDIR /tmp
# Tue, 10 Nov 2020 00:46:13 GMT
RUN apk add --update --no-cache bash openssl && mkdir -p $BOOT_INSTALL && wget -q https://github.com/boot-clj/boot-bin/releases/download/latest/boot.sh && echo "Comparing installer checksum..." && sha256sum boot.sh && echo "0ccd697f2027e7e1cd3be3d62721057cbc841585740d0aaa9fbb485d7b1f17c3 *boot.sh" | sha256sum -c - && mv boot.sh $BOOT_INSTALL/boot && chmod 0755 $BOOT_INSTALL/boot && apk del openssl
# Tue, 10 Nov 2020 00:46:13 GMT
ENV PATH=/opt/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/bin/
# Tue, 10 Nov 2020 00:46:14 GMT
ENV BOOT_AS_ROOT=yes
# Tue, 10 Nov 2020 00:46:33 GMT
RUN boot
# Tue, 10 Nov 2020 00:46:34 GMT
CMD ["boot" "repl"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d4961e1b84bb83aca8e1aadcad45ff59be8b1b7e2040c1004a1a4e4dd330b`  
		Last Modified: Thu, 22 Oct 2020 02:46:10 GMT  
		Size: 926.4 KB (926394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b79399f6b51192648fbb46ca61c9141a7c433df0a44ffabbb7ca5857fb15bd`  
		Last Modified: Tue, 10 Nov 2020 00:26:34 GMT  
		Size: 184.3 MB (184293637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9b03134887c076e01cd61aff8c6e467fd9a4f0066f0dbd011f2b1c9a1e17e3`  
		Last Modified: Tue, 10 Nov 2020 00:48:33 GMT  
		Size: 792.3 KB (792319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8c6e7af1b10acf33121c7aef90c28bb32d0f25dfb0024f5584aace76bb18a5`  
		Last Modified: Tue, 10 Nov 2020 00:48:38 GMT  
		Size: 58.8 MB (58820215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
