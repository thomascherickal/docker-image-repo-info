## `openjdk:18-oraclelinux8`

```console
$ docker pull openjdk@sha256:c412e4360bb12bf02a5832a41b86175323a5f095c6d52a7f3e95a634e464c849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:c3f692d7245baad99d96b213e6c5f24529d16132ba74fa19d62db2aaf9f85586
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.5 MB (241451286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c164acc56b8fbd812e2e9719b215580d9eb6d82677cff65a91a00ef75da0ff`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 05 Jul 2022 22:20:34 GMT
ADD file:69555d6633d88e50ab2ddecc8bc5002a8f79005d828a9093975d68ca05b023e9 in / 
# Tue, 05 Jul 2022 22:20:34 GMT
CMD ["/bin/bash"]
# Tue, 05 Jul 2022 22:49:44 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 05 Jul 2022 22:51:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Tue, 05 Jul 2022 22:51:26 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Jul 2022 22:51:26 GMT
ENV LANG=C.UTF-8
# Tue, 05 Jul 2022 22:51:27 GMT
ENV JAVA_VERSION=18.0.1.1
# Tue, 05 Jul 2022 22:51:36 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.1.1/65ae32619e2f40f3a9af3af1851d6e19/2/GPL/openjdk-18.0.1.1_linux-x64_bin.tar.gz'; 			downloadSha256='4f81af7203fa4c8a12c9c53c94304aab69ea1551bc6119189c9883f4266a2b24'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.1.1/65ae32619e2f40f3a9af3af1851d6e19/2/GPL/openjdk-18.0.1.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='e667166c47e90874af3641ad4a3952d3c835627e4301fa1f0d620d9b6e366519'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 05 Jul 2022 22:51:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e54b73e95ef388354463a761e4e93ce3dac29cb244b2dc0424f2f4afc6ddf5cd`  
		Last Modified: Tue, 05 Jul 2022 22:21:41 GMT  
		Size: 39.2 MB (39222121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e62647f09f0ab1a3ac2d84823777bead33aa8e201c13b86c063296e8268023`  
		Last Modified: Tue, 05 Jul 2022 22:58:01 GMT  
		Size: 13.5 MB (13505357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8e06a8884e166c2e6a94a6f4ada965ee29bfd0b3b68d5ff0a3512751443f5a`  
		Last Modified: Tue, 05 Jul 2022 23:01:31 GMT  
		Size: 188.7 MB (188723808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7029f31485d12e22dc21e18ccd5640c816c67eb15d09e325451d3c4c5a0025fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.0 MB (239972068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0de6f31b1faed71554b5db2511971b9d0f392230f4b404b244daefc34ac95b78`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:40:34 GMT
ADD file:deb746f3cc547a36a34f3bfe68510bbd6f8a3b2da72bcca3cce36dfe0e519e77 in / 
# Thu, 30 Jun 2022 17:40:35 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 18:00:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 18:03:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 30 Jun 2022 18:03:07 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 18:03:08 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 18:03:09 GMT
ENV JAVA_VERSION=18.0.1.1
# Thu, 30 Jun 2022 18:03:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.1.1/65ae32619e2f40f3a9af3af1851d6e19/2/GPL/openjdk-18.0.1.1_linux-x64_bin.tar.gz'; 			downloadSha256='4f81af7203fa4c8a12c9c53c94304aab69ea1551bc6119189c9883f4266a2b24'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.1.1/65ae32619e2f40f3a9af3af1851d6e19/2/GPL/openjdk-18.0.1.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='e667166c47e90874af3641ad4a3952d3c835627e4301fa1f0d620d9b6e366519'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 18:03:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c7107c973a1b04b1f048e43f460fd4f030df5f2e53fce3dfb8a13dc7fefdb4b0`  
		Last Modified: Thu, 30 Jun 2022 17:41:32 GMT  
		Size: 38.0 MB (38023864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a33b6e144a0eee25610c802e234489b8afda2108ce38e5f76ee4d79e5e45ff`  
		Last Modified: Thu, 30 Jun 2022 18:15:30 GMT  
		Size: 14.3 MB (14303308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0413a313e20f1bce92e3b6b65b63a5ee5ed33c9a5c9529eb3130424205a939b`  
		Last Modified: Thu, 30 Jun 2022 18:18:37 GMT  
		Size: 187.6 MB (187644896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
