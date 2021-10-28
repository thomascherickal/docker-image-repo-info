## `openjdk:17-oraclelinux8`

```console
$ docker pull openjdk@sha256:329525790f32a130fb5b25785cb5d8d1d695d61c2c5a4f73814e4e5ec6cfc0da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:ba0fc847b43cb8756be4497758863d7b51003efcb9b861211a8d5d3afe6c9fa2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.6 MB (242632892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b002702b7d015a0cfe17b6d7679c903fc5fecb65c906a7ad1a19aa98d51c2d1b`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:22:47 GMT
ADD file:45a1eba89256c6e3801f14738faca9e260b17b306f0fc8769ba0b0f94f0fdf68 in / 
# Thu, 28 Oct 2021 01:22:47 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 01:44:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 28 Oct 2021 01:45:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 28 Oct 2021 01:45:58 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:45:58 GMT
ENV LANG=C.UTF-8
# Thu, 28 Oct 2021 01:45:59 GMT
ENV JAVA_VERSION=17.0.1
# Thu, 28 Oct 2021 01:46:10 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Oct 2021 01:46:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f420596490555ff89c8ec7d6b74b4e46c2b3b98dc775c9d19494d8afeb475852`  
		Last Modified: Thu, 28 Oct 2021 01:24:04 GMT  
		Size: 42.0 MB (41970837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9c63ed3ba0226d765a092dd6fcc06fe5ece8a2dd0fd11e1add9c0ddee488e`  
		Last Modified: Thu, 28 Oct 2021 01:52:24 GMT  
		Size: 13.5 MB (13491622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf092705b191dbeb36cf56fddcc2e45ab0778a28ddc4c4a29c2acf3077c43f10`  
		Last Modified: Thu, 28 Oct 2021 01:54:15 GMT  
		Size: 187.2 MB (187170433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9039a1576e4bc610cdafe37b16154063b179ec1d150b03a0d765cd1d5c6749b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.1 MB (242130274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61937d6b1fc1e8cf99260a17d811b13e45ecf33a392db240ac0edc918caa62d6`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:43:49 GMT
ADD file:accebe81069e9a5a2fa2b5311f1fd53f84fc7cc12b93d70f150e3ee0c4d1853c in / 
# Thu, 28 Oct 2021 01:43:50 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 02:15:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 28 Oct 2021 02:17:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 28 Oct 2021 02:17:07 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 02:17:08 GMT
ENV LANG=C.UTF-8
# Thu, 28 Oct 2021 02:17:09 GMT
ENV JAVA_VERSION=17.0.1
# Thu, 28 Oct 2021 02:17:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-x64_bin.tar.gz'; 			downloadSha256='1c0a73cbb863aad579b967316bf17673b8f98a9bb938602a140ba2e5c38f880a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk17.0.1/2a2082e5a09d4267845be086888add4f/12/GPL/openjdk-17.0.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='86653d48787e5a1c029df10da7808194fe8bd931ddd72ff3d42850bf1afb317e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Oct 2021 02:17:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:42445708416d90c524044613ca219573cb3b87e3c236ae8642b0e17b341389fb`  
		Last Modified: Thu, 28 Oct 2021 01:45:02 GMT  
		Size: 41.9 MB (41879582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4f9f60b42882cee2f44d430dab6e4bd76aacf43d9e203013dc45e48cfc38eb`  
		Last Modified: Thu, 28 Oct 2021 02:28:51 GMT  
		Size: 14.3 MB (14273910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1ce40e61e1f8464f2fe3066e4712fe7d0e54db14c35a96c036ed408acb907e`  
		Last Modified: Thu, 28 Oct 2021 02:31:04 GMT  
		Size: 186.0 MB (185976782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
