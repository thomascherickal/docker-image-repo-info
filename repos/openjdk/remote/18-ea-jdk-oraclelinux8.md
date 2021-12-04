## `openjdk:18-ea-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:21ac219bd5a6e676840232353fa14e0de28bffe5025d1a031d5f27a704ba12e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:8d39657b60a32f4d3515337d42635aeb59569deed9cfa46cab2be084d507985d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244180548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fc98b1d321ff72af7d53cd853ffb749e3b56acebda113ae4e83c56553ed52e`
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
# Fri, 03 Dec 2021 23:46:23 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:46:34 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='fdf145c2819ef28edee67b7a6605bee89aefc505a1abea1686bec03fcba87c70'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='14e35be6e99a093bd4d5666bd4d557ebb94ab9e03eab9e9ae0eb69fc7b3e662b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Dec 2021 23:46:35 GMT
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
	-	`sha256:cf8c056da97f7756063ca4f6d174c216b0cc2f0d63fd8b21c58b6c02c60435b6`  
		Last Modified: Fri, 03 Dec 2021 23:53:23 GMT  
		Size: 188.6 MB (188570918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ec7e89427a4c12512a0bfc3264726d985fdd435c1660d2786eaf86dc599107cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.8 MB (243817536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e2a9898f7ab33e8a5221b786861ce840a7cf4d36ba0a40ff699c5ef57f022c`
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
# Fri, 03 Dec 2021 23:07:55 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:08:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='fdf145c2819ef28edee67b7a6605bee89aefc505a1abea1686bec03fcba87c70'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='14e35be6e99a093bd4d5666bd4d557ebb94ab9e03eab9e9ae0eb69fc7b3e662b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Dec 2021 23:08:16 GMT
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
	-	`sha256:1f24184cec8ab581b1dd6ac165ad3d9bfdc0b67e6dd169e3b9194b342a3f2061`  
		Last Modified: Fri, 03 Dec 2021 23:19:48 GMT  
		Size: 187.5 MB (187505210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
