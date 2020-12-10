## `clojure:openjdk-16-tools-deps-1.10.1.754-alpine`

```console
$ docker pull clojure@sha256:c48cfddec51c8fb1a3aee2df4099d5c81c7097acea453c39a71d0876f3d6bc79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `clojure:openjdk-16-tools-deps-1.10.1.754-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:dc864a8b6c7a390c17269c318956e195e74de31c773e2b169ff6e1f7df7cab1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210570933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f0788e7054ca82e9ea8c7b0058a7591a3499d3b23f1ead2898cab82bbe262e5`
-	Default Command: `["sh","-c","sleep 1 && exec clj"]`

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
# Thu, 10 Dec 2020 16:28:52 GMT
ENV CLOJURE_VERSION=1.10.1.754
# Thu, 10 Dec 2020 16:28:52 GMT
WORKDIR /tmp
# Thu, 10 Dec 2020 16:29:01 GMT
RUN apk add --update --no-cache curl bash make && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "1c623dd76ea75cb89623ffc71a5ec59297c785c0c19fc5c2fa0fe9428efe8a3d *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Thu, 10 Dec 2020 16:29:01 GMT
CMD ["sh" "-c" "sleep 1 && exec clj"]
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
	-	`sha256:371917f51dad1d5986d5c4fb2b8aa0acb2f72e7f7e0e893b5e631fc33bf71f90`  
		Last Modified: Thu, 10 Dec 2020 16:33:02 GMT  
		Size: 22.6 MB (22554042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
