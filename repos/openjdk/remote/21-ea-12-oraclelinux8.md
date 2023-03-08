## `openjdk:21-ea-12-oraclelinux8`

```console
$ docker pull openjdk@sha256:d5512dd90a9f3ee4b4a730c9368c66256404fc6a63151b12759a2860e55d97e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-12-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:7412f8aa9aa5832a6e0e78650ba0ca2bbf656de6d619544eb9d222197466e878
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.0 MB (258984767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cea25d9c29a15ff72dff7aa83e0ebdf32084363a1be21745c47cf9a72a89f77`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:53:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:53:15 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 08 Mar 2023 20:53:15 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 20:53:15 GMT
ENV LANG=C.UTF-8
# Wed, 08 Mar 2023 20:53:16 GMT
ENV JAVA_VERSION=21-ea+12
# Wed, 08 Mar 2023 20:53:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='da247094c9b9e7b4ab18b5e36adc89e3b7f6ee77192816ce059b933e23e09fca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='ea0bf5244a8b27f1c111cb40cb161186c9217f0bbc31e3a019b81c21505c8f18'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 20:53:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754d31dea44245a0029d262dade1fe4e14228c7182d3efde4994c6a76398bc7`  
		Last Modified: Wed, 08 Mar 2023 20:56:42 GMT  
		Size: 15.0 MB (15014167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b7bbe3560c7fa5849ccc8ef87b09dfc87077c5e3d2c04df9325bf13d4fdf82`  
		Last Modified: Wed, 08 Mar 2023 20:56:54 GMT  
		Size: 199.4 MB (199412786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-12-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ecfe3402b24f21026ce9a57affac59f4da79df1f84a5969ec2e1f2dc23f6bb54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257187654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ea0efb3c8d3019bfb1ca8d35faf69cfdbbd1a390949b233d984e460e112cef`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:19:53 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:19:53 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 08 Mar 2023 21:19:53 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 21:19:53 GMT
ENV LANG=C.UTF-8
# Wed, 08 Mar 2023 21:19:53 GMT
ENV JAVA_VERSION=21-ea+12
# Wed, 08 Mar 2023 21:20:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-x64_bin.tar.gz'; 			downloadSha256='da247094c9b9e7b4ab18b5e36adc89e3b7f6ee77192816ce059b933e23e09fca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/12/GPL/openjdk-21-ea+12_linux-aarch64_bin.tar.gz'; 			downloadSha256='ea0bf5244a8b27f1c111cb40cb161186c9217f0bbc31e3a019b81c21505c8f18'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 21:20:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec39ece690c19b75d657ca26bf156e883914c8bea4948e081819aff289dc43c5`  
		Last Modified: Wed, 08 Mar 2023 21:22:51 GMT  
		Size: 15.8 MB (15834481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5fb69d20d4574f551d397e697d69f9fad2c396c580aeac1897f8eafe8be0b5`  
		Last Modified: Wed, 08 Mar 2023 21:23:03 GMT  
		Size: 197.9 MB (197897034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
