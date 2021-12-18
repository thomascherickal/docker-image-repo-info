## `openjdk:18-ea-oracle`

```console
$ docker pull openjdk@sha256:9d288cf36a1b6490314963bab09a651f9fb268992e528c8a737dfa7d193fc5ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:bec53a3193fc2c3afe2da73d28ea9f8007538e9c9ed895b11932372ffbd712b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244240658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8244159bb89818829b75896a1045ca54161fe10590221bc45da37d48033cb`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 19 Nov 2021 03:08:35 GMT
ADD file:d27591ceabbe39902d88042ebe31aecc38844787fafa004cdeb0080da29c1623 in / 
# Fri, 19 Nov 2021 03:08:35 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 03:25:16 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 19 Nov 2021 03:25:17 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 19 Nov 2021 03:25:17 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Nov 2021 03:25:17 GMT
ENV LANG=C.UTF-8
# Sat, 18 Dec 2021 04:09:53 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 04:10:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 18 Dec 2021 04:10:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:28587b6e64756a60a354301d011190fb69ea1eed25d7a5180811dab252e16a21`  
		Last Modified: Fri, 19 Nov 2021 03:09:27 GMT  
		Size: 42.1 MB (42097812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1655352c888337fbd3af21c25aa26d4561a0b9b6035a8b22c9ee0c8ae9a3784`  
		Last Modified: Fri, 19 Nov 2021 03:31:40 GMT  
		Size: 13.5 MB (13511818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b234b6e4c7a438373f40fd8180a5b2a410e5bb8ebe6d03abb153db0faa14a97`  
		Last Modified: Sat, 18 Dec 2021 04:22:22 GMT  
		Size: 188.6 MB (188631028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3a1703be7dc563d787f2c1aac428fe71f7db4d611d90b2c9c1c7ce050ee9eb6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243880426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb4fbe2e7790a80cdb1702add5174f8226b0a759be16fad0c68851ee3452259a`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 19 Nov 2021 02:35:27 GMT
ADD file:31ec2bba02fab51f683553c78815a422089e6227bd4a65d33f35bc15588da3f7 in / 
# Fri, 19 Nov 2021 02:35:27 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 02:52:30 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 19 Nov 2021 02:52:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 19 Nov 2021 02:52:31 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 19 Nov 2021 02:52:32 GMT
ENV LANG=C.UTF-8
# Fri, 17 Dec 2021 23:43:00 GMT
ENV JAVA_VERSION=18-ea+28
# Fri, 17 Dec 2021 23:43:17 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='7e5f0e54c799f8c155a934e61d88f4fef3a70a641c1636c925158622c7bd9341'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/28/GPL/openjdk-18-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='e29aa39763ebcfe5f037cc4fe47c6b9eb34cbe482f6ea57e93de89070255e22b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 17 Dec 2021 23:43:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c621c1ca8ceb7b3c3055633f5e537023039566ffcde238e41463f74eb6396051`  
		Last Modified: Fri, 19 Nov 2021 02:36:28 GMT  
		Size: 42.0 MB (42011387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d87024ee2f6936bf9ad81953e5ec643cddc67e7055ec11cf737242c60e2c9b`  
		Last Modified: Fri, 19 Nov 2021 03:04:14 GMT  
		Size: 14.3 MB (14300939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fb542a47ad77404628905b19179ce1fb5b4bc56c8941076afe9ae0d61e0a22`  
		Last Modified: Sat, 18 Dec 2021 00:01:08 GMT  
		Size: 187.6 MB (187568100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
