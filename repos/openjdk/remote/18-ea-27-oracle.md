## `openjdk:18-ea-27-oracle`

```console
$ docker pull openjdk@sha256:a47f48ead567e3714f4a3f841d34fb81e5e16a5b1b32b150fc16c317d43a0d9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-27-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:c5046cbdf94ce11e7a800d1d3c889175fc610f008e5a6a109e46d620e7092d01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244188653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ddca46d7f4b91163aad90d2bbe1fe183fc2f4ab6e46fd0cae251279b084894`
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
# Fri, 10 Dec 2021 21:20:03 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:20:14 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:20:15 GMT
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
	-	`sha256:65bd140ea9628dcba7d36d069b7ef4a270868a27e6c4acc2948a48d337ca57ff`  
		Last Modified: Fri, 10 Dec 2021 21:26:48 GMT  
		Size: 188.6 MB (188579023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-27-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:dab042aec18c1e2abe63083e2640a8c99d366dd0ac91375402cec81fb8013028
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243812548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b88994a72de29464ad41cf29580b7b5a0ed2f54185d27ccaf90b8d1b8c4e76d1`
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
# Fri, 10 Dec 2021 21:51:50 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:52:02 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:52:02 GMT
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
	-	`sha256:eafd2f1b1047c7fb12c4774ab3a88d12b8d95c7572a9a761dbac1c06b3a6798a`  
		Last Modified: Fri, 10 Dec 2021 22:03:44 GMT  
		Size: 187.5 MB (187500222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
