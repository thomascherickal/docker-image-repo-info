## `openjdk:22-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:562049f716a556c9b3971b4a6d9d6777ceece94c99c849d9f8debd80ed480e09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:c5e3470712a349f81dc50ae4fe41df839aa6a871560ee731cfca0a10b490eba5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.7 MB (264707346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981906d9c6016d55f5624f4acf5cba3b9bbe924f4c4254d24d5cb570bf490427`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 01:20:36 GMT
ADD file:196115c6281a0a56854066be2766eb0dc9da452f60a060b90bbe681e6b8ffc11 in / 
# Fri, 11 Aug 2023 01:20:36 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:53:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:53:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 11 Aug 2023 01:53:51 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:53:51 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:02:26 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:02:37 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:02:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b193354265ba898bb7548038f52378b3dbb6aac5afbaca49bb83ccfe51dfadeb`  
		Last Modified: Fri, 11 Aug 2023 01:21:58 GMT  
		Size: 44.9 MB (44910081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e75d2bbaed8a6321c319c610e5cd0923e1fc6a9ad6122e3b9573f10a5166f9e`  
		Last Modified: Fri, 11 Aug 2023 01:56:08 GMT  
		Size: 15.0 MB (15004378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee71eb3023bf943feee66a6e22df8fddf16ce8649e0ac1234bf449819c22485`  
		Last Modified: Sat, 12 Aug 2023 00:06:47 GMT  
		Size: 204.8 MB (204792887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:bc67655a58b15e4d333ee63195384d931f2d6effec37c9392553235e60a3b525
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262474238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edfac54a7d20104cad2f28fa1abcdf8d2a849062567ba2f76d8da70fff424a7`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 00:40:33 GMT
ADD file:24663feb951dcfae36948e6cbc8697e8bef563d86c15af3daa54a1b830965593 in / 
# Fri, 11 Aug 2023 00:40:34 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:11:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:11:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 11 Aug 2023 01:11:14 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:11:15 GMT
ENV LANG=C.UTF-8
# Fri, 11 Aug 2023 01:11:15 GMT
ENV JAVA_VERSION=22-ea+9
# Fri, 11 Aug 2023 01:11:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/9/GPL/openjdk-22-ea+9_linux-x64_bin.tar.gz'; 			downloadSha256='dd11f0f96ed6992b56452eee0683b50f1b550f74c31fb39e1eb1ff8a232caf68'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/9/GPL/openjdk-22-ea+9_linux-aarch64_bin.tar.gz'; 			downloadSha256='47ab1fb3cbe8174c21e10880e5de0c60d754cf5ba6d5cdfbe1a1d91b53b193bc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Aug 2023 01:11:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd2ec1b01835c3bcf117123886f982435cd8e445790b761779f35779d61faad3`  
		Last Modified: Fri, 11 Aug 2023 00:41:41 GMT  
		Size: 43.6 MB (43625591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7023146e285ffba3adcf0df2d0ef98b1f28c00ef46b2ffc20a5c3d01540eba`  
		Last Modified: Fri, 11 Aug 2023 01:13:09 GMT  
		Size: 15.7 MB (15666637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d23f2b2ca690299eb463a98645be8dfdb2f83636b8c3f8fc0149a8858c5ab04`  
		Last Modified: Fri, 11 Aug 2023 01:13:20 GMT  
		Size: 203.2 MB (203182010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
