## `openjdk:19-ea-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:8c310aa14204cab2a2c8e70f09781c7ecebd454c46f47ddd92fda3d107352409
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:32db8d1d213c996ec156b8aff308f4b4717366eea41663f31b221d06378387b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.1 MB (245085315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835f79997a580a6c427ce1f6f11f461984e04d40bf9ae3631f5f736b4c65d462`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 19 Nov 2021 03:08:35 GMT
ADD file:d27591ceabbe39902d88042ebe31aecc38844787fafa004cdeb0080da29c1623 in / 
# Fri, 19 Nov 2021 03:08:35 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 03:25:16 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 14 Dec 2021 01:41:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 14 Dec 2021 01:41:07 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:41:07 GMT
ENV LANG=C.UTF-8
# Tue, 14 Dec 2021 01:41:08 GMT
ENV JAVA_VERSION=19-ea+1
# Tue, 14 Dec 2021 01:41:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='652a141e1854a51df7991b003d6e9478021cb4a4ee67b320cb284e40dff46847'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='fe09452d49aad26e03df3d5b5ebfc22f8b2d8a1e16dcc03a2f00b31f586a770a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Dec 2021 01:41:20 GMT
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
	-	`sha256:f8e64c5ee8ba9033648401668d3a865278b207edf4bf23d357d3219fd07c0fb3`  
		Last Modified: Tue, 14 Dec 2021 01:49:29 GMT  
		Size: 189.5 MB (189475685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:fe1801c084bf723cc9eba0e66229539ae283b51f550b9c10c0ac88827c61a58c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.7 MB (244728395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e91c2feaf37abeade55efd33004cbe241195aaf43a67a1c02adef3fcced9294`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 19 Nov 2021 02:35:27 GMT
ADD file:31ec2bba02fab51f683553c78815a422089e6227bd4a65d33f35bc15588da3f7 in / 
# Fri, 19 Nov 2021 02:35:27 GMT
CMD ["/bin/bash"]
# Fri, 19 Nov 2021 02:52:30 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 14 Dec 2021 01:58:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 14 Dec 2021 01:58:38 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:58:39 GMT
ENV LANG=C.UTF-8
# Tue, 14 Dec 2021 01:58:40 GMT
ENV JAVA_VERSION=19-ea+1
# Tue, 14 Dec 2021 01:58:54 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='652a141e1854a51df7991b003d6e9478021cb4a4ee67b320cb284e40dff46847'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='fe09452d49aad26e03df3d5b5ebfc22f8b2d8a1e16dcc03a2f00b31f586a770a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Dec 2021 01:58:55 GMT
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
	-	`sha256:e754306742cb5ebb615fca16c20e81f8b85c4266a291613eb046115491b20281`  
		Last Modified: Tue, 14 Dec 2021 02:13:04 GMT  
		Size: 188.4 MB (188416069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
