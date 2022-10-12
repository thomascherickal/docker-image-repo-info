## `openjdk:20-ea-18-jdk-oracle`

```console
$ docker pull openjdk@sha256:ff944c337164ef87797146ecfaae19742a0754983ea2a401b87cbb6a214e5c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-18-jdk-oracle` - linux; amd64

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

### `openjdk:20-ea-18-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:78b4d4aabeeab067bf10d8796027a8e6c922211b33e8a43cb9b771014900a835
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.0 MB (247962082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3c9885d45efa5d21c2a3c47fe4e3f15f9cb71cc3eb85c91250738ceba29e556`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 12 Oct 2022 20:40:56 GMT
ADD file:049ff2e28998fde860d1a12f43ec245d10345a71953f67108180c23c237ce26e in / 
# Wed, 12 Oct 2022 20:40:56 GMT
CMD ["/bin/bash"]
# Wed, 12 Oct 2022 20:58:37 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 12 Oct 2022 20:58:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 12 Oct 2022 20:58:38 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 Oct 2022 20:58:39 GMT
ENV LANG=C.UTF-8
# Wed, 12 Oct 2022 20:58:40 GMT
ENV JAVA_VERSION=20-ea+18
# Wed, 12 Oct 2022 21:14:56 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1081d9b6e6439841c3665fe65caf47431f7a6208ff6da8ee66a617a5577754c1'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='92161bb7811ac65f8a1deddef23028d817634cab1605a7255aefb517c2a2f6f8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 12 Oct 2022 21:14:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:828689dcde4b0fe396ab27cf3a6d5f71ee01d48891421ec4381d74ed415be5d0`  
		Last Modified: Wed, 12 Oct 2022 20:42:33 GMT  
		Size: 39.4 MB (39409290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f742b2cfb7e7c72c98123d08c444932851dc28c95bdb7a2a6a4ebfbcd5456bd`  
		Last Modified: Wed, 12 Oct 2022 21:20:59 GMT  
		Size: 13.1 MB (13054769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e47c307f418f184a914c44a482f1e7a5e126a79a5b0e0374c7b6bc8c9d4a877`  
		Last Modified: Wed, 12 Oct 2022 21:21:14 GMT  
		Size: 195.5 MB (195498023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
