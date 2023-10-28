## `openjdk:22-ea-oracle`

```console
$ docker pull openjdk@sha256:38649d2d5c25b262578390c2ef721abaf760048f3cc515a3677eec66ec185447
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:8d71e0613a5de7caa0fd47e8a3cd26dd31b9243a767754c80e9fa6476ab3bad2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.8 MB (264810174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c782015b7992a3d6a2b38437e2999f43a073e9a45a4ba7df3ae62c0d91ce1cf`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 20 Oct 2023 18:27:20 GMT
ADD file:0f45bdf93b14a2ab9389b71d23b6c7f6d2935c8016e3b6422814f8fc79bef986 in / 
# Fri, 20 Oct 2023 18:27:20 GMT
CMD ["/bin/bash"]
# Fri, 20 Oct 2023 18:45:06 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 20 Oct 2023 18:45:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 20 Oct 2023 18:45:06 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Oct 2023 18:45:06 GMT
ENV LANG=C.UTF-8
# Sat, 28 Oct 2023 00:37:00 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e0176adc18c476bdfcc701f01cda5acf49bc8e6d7fadac8072091a43fafbb25`  
		Last Modified: Fri, 20 Oct 2023 18:28:56 GMT  
		Size: 44.3 MB (44279620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7fcefe71b24cef619772a3adab6474d1dee79d5ec55a8ac900504be9b669d3`  
		Last Modified: Fri, 20 Oct 2023 18:46:04 GMT  
		Size: 15.0 MB (15016123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2eda46ed558be826c06a3023da2ed44c51204652a9d80353d72f96b0183c26`  
		Last Modified: Sat, 28 Oct 2023 00:39:20 GMT  
		Size: 205.5 MB (205514431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:75d9f99b1aee18d584c49ddd91298e156df870405ea3fdc9d24763aeb8562021
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.1 MB (263056937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beb2da786c6f04bb4ae37407693c48106d7b5d3c86eb9f8056d0ff84233787bb`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 20 Oct 2023 18:39:12 GMT
ADD file:e189ba41c54c386435a3292026b75a1386976d3222102c16a725f58f594f284e in / 
# Fri, 20 Oct 2023 18:39:12 GMT
CMD ["/bin/bash"]
# Fri, 20 Oct 2023 19:20:37 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 20 Oct 2023 19:20:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 20 Oct 2023 19:20:38 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Oct 2023 19:20:38 GMT
ENV LANG=C.UTF-8
# Sat, 28 Oct 2023 00:36:49 GMT
ENV JAVA_VERSION=22-ea+21
# Sat, 28 Oct 2023 00:37:02 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='cefe6f9697801dd2a7abebdbd5b7bd36ad489794589e838562da46bde434ae5e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/21/GPL/openjdk-22-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='b77e7f170973c91690aa64a028f2e991828fde5092eabc29b602e26824216797'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 28 Oct 2023 00:37:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e39ec8f010eb75816ae2c21b014f7fdecffb48374079b6f1bce017214e2a45cd`  
		Last Modified: Fri, 20 Oct 2023 18:40:29 GMT  
		Size: 43.7 MB (43672784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4910a471f6760b5f0bc0ef155e7afd624a4c1ea6f09bb680d43c1041cfd4fd`  
		Last Modified: Fri, 20 Oct 2023 19:21:34 GMT  
		Size: 15.7 MB (15660393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53ceb6960f4f54706d46eef157cc36e08813d97bde37cecd72bca1f718163cb`  
		Last Modified: Sat, 28 Oct 2023 00:39:14 GMT  
		Size: 203.7 MB (203723760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
