## `openjdk:20-ea-18-oraclelinux8`

```console
$ docker pull openjdk@sha256:925a08172a85abf3977844d3acba87ea34e30073faa2d696ecf919f6b86efb07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-18-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:d12adeb48b8935ea5ac5c3851627a72e0f71ba24646aa6ca13312858a5a1ad6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249736607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e246ce0ed67cd59e42cc1496756470a398d4682ac2caa50f826fea3cbb5747c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Oct 2022 20:31:40 GMT
ADD file:40e1b0533d9ae91c868834395cbd4b74cf2a47965791be201c03ae764f9da2b0 in / 
# Fri, 07 Oct 2022 20:31:41 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 20:50:12 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 07 Oct 2022 20:50:13 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 07 Oct 2022 20:50:13 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 20:50:13 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 23:45:37 GMT
ENV JAVA_VERSION=20-ea+18
# Fri, 07 Oct 2022 23:45:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1081d9b6e6439841c3665fe65caf47431f7a6208ff6da8ee66a617a5577754c1'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='92161bb7811ac65f8a1deddef23028d817634cab1605a7255aefb517c2a2f6f8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 07 Oct 2022 23:45:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:295ca23427284cb123fd4c132a1ecb521e7f787ac75dadec342f744a343efec4`  
		Last Modified: Fri, 07 Oct 2022 20:33:22 GMT  
		Size: 40.6 MB (40589568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f95ca5341d49c7c99a979d862484e30b44156db525868b136dd3cf8c0535aa`  
		Last Modified: Fri, 07 Oct 2022 20:54:09 GMT  
		Size: 12.2 MB (12231949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f399b336fab70942c891425cfe4feb51770e2620e58290b19d62a4f24d1893d1`  
		Last Modified: Fri, 07 Oct 2022 23:49:52 GMT  
		Size: 196.9 MB (196915090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-18-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:fc11664ec64fd01e6a1ad29fbaa76e829193ab8a4d58f5dca0420e1b4c310cc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.0 MB (247961724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dedc60218ae8d0a80a0091c33492fbadae256921050c5c83088c82f3f73cd2e`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Oct 2022 20:51:45 GMT
ADD file:6eb7b065ffe8855d82638de19bd23fba329883c96f01d093e7bc6bdb5da836a3 in / 
# Fri, 07 Oct 2022 20:51:46 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:13:40 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 07 Oct 2022 21:13:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 07 Oct 2022 21:13:42 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 21:13:43 GMT
ENV LANG=C.UTF-8
# Sat, 08 Oct 2022 00:20:43 GMT
ENV JAVA_VERSION=20-ea+18
# Sat, 08 Oct 2022 00:21:08 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1081d9b6e6439841c3665fe65caf47431f7a6208ff6da8ee66a617a5577754c1'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='92161bb7811ac65f8a1deddef23028d817634cab1605a7255aefb517c2a2f6f8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 08 Oct 2022 00:21:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5d45c82139e084eb338a0a2346c4ec4c6d2bfa4acda9194cf6602728b4a3e89f`  
		Last Modified: Fri, 07 Oct 2022 20:53:34 GMT  
		Size: 39.4 MB (39409020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e39aebf905a4bfcc927f63602bf79927ed6767d85862e1311b9e8f0e5924ad`  
		Last Modified: Fri, 07 Oct 2022 21:21:10 GMT  
		Size: 13.1 MB (13054492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e449a04693044e6400a53b93dd948516ef81824544e49d210c18b647d55d0`  
		Last Modified: Sat, 08 Oct 2022 00:28:25 GMT  
		Size: 195.5 MB (195498212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
