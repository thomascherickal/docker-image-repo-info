## `clojure:openjdk-18-alpine`

```console
$ docker pull clojure@sha256:97670001fd2c9f67df858b2a313529865b003cc47ed93909e03512c1ccae5934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `clojure:openjdk-18-alpine` - linux; amd64

```console
$ docker pull clojure@sha256:05f4cb92ab40e59387cde3fd313a26937c28e1a948fdc68bb0f3d97950127952
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.9 MB (221864269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa69b348cf7d5365eb7da8d421337177b2c6a936342aff5a8e7d27ceafb2aef8`
-	Entrypoint: `["entrypoint"]`
-	Default Command: `["-M","--repl"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:45:32 GMT
RUN apk add --no-cache java-cacerts
# Tue, 30 Nov 2021 04:45:32 GMT
ENV JAVA_HOME=/opt/openjdk-18
# Tue, 30 Nov 2021 04:45:32 GMT
ENV PATH=/opt/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 04:45:32 GMT
ENV JAVA_VERSION=18-ea+11
# Tue, 30 Nov 2021 04:45:45 GMT
RUN set -eux; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			downloadUrl='https://download.java.net/java/early_access/alpine/11/binaries/openjdk-18-ea+11_linux-x64-musl_bin.tar.gz'; 			downloadSha256='86fad9069587a5e9dd003e7354a69b2f720a05c12706d2f2345a0c8d90e56c47'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		wget -O openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/ssl/certs/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Nov 2021 04:45:46 GMT
CMD ["jshell"]
# Tue, 01 Feb 2022 01:30:48 GMT
ENV CLOJURE_VERSION=1.10.3.1069
# Tue, 01 Feb 2022 01:30:48 GMT
WORKDIR /tmp
# Tue, 01 Feb 2022 01:30:54 GMT
RUN apk add --no-cache curl bash make git && wget https://download.clojure.org/install/linux-install-$CLOJURE_VERSION.sh && sha256sum linux-install-$CLOJURE_VERSION.sh && echo "e9e8382971bf179048fc6b171a6216283e19a880b271e489d4b677ad4d4894a6 *linux-install-$CLOJURE_VERSION.sh" | sha256sum -c - && chmod +x linux-install-$CLOJURE_VERSION.sh && ./linux-install-$CLOJURE_VERSION.sh && rm linux-install-$CLOJURE_VERSION.sh && clojure -e "(clojure-version)" && apk del curl
# Tue, 01 Feb 2022 01:30:55 GMT
COPY file:b0aef3ea203de7b5c2ea645debf58c8231445a2e3070b72749b54614f4a89b82 in /usr/local/bin/rlwrap 
# Tue, 01 Feb 2022 01:30:55 GMT
COPY file:137b40904568e30898cd031ef34f77e7f132846ba4eec91d04ae4b93dddfbb8d in /usr/local/bin/entrypoint 
# Tue, 01 Feb 2022 01:30:55 GMT
ENTRYPOINT ["entrypoint"]
# Tue, 01 Feb 2022 01:30:55 GMT
CMD ["-M" "--repl"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ae5de21b2241a24b653013bdda639de16f984789b28bbcb7108523b460d1e4`  
		Last Modified: Tue, 30 Nov 2021 04:55:25 GMT  
		Size: 932.2 KB (932205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3048de22201addf91c8f64e5382a33c2791d3c21a0906eefce3c4cb08d875839`  
		Last Modified: Tue, 30 Nov 2021 04:55:48 GMT  
		Size: 188.7 MB (188699653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a92ff1a0cd11ca95c12a4d4774fadbfbceb5be15aa2079b5a43a66b5249d5`  
		Last Modified: Tue, 01 Feb 2022 01:40:14 GMT  
		Size: 29.4 MB (29412971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5107d44bf14e5e8712346f37052a290d61f99db4c47dd857a37208430238e70c`  
		Last Modified: Tue, 01 Feb 2022 01:40:11 GMT  
		Size: 624.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bb4700f6afb624fe1cbf7c103e9b88f069385edd6f3d3a078b84a306764afa`  
		Last Modified: Tue, 01 Feb 2022 01:40:11 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
