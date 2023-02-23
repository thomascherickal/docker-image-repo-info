## `openjdk:20-rc-oracle`

```console
$ docker pull openjdk@sha256:7b062d50c623345db402b3b947ba320ab52785bdb712e6152d9698e96a13760e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-rc-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:ec062f28f88f8455cde6746071d8aea311f1aa8370154569af5670e54b725738
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.9 MB (254925241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b610e334aeb074516e6b92e734e7b1c97742058e48b15d17256aeac0fbc00a3`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Feb 2023 19:37:08 GMT
ADD file:7c92981e2fed9bedfca663209480ce9006dce0edc6c44c25640255683952b929 in / 
# Thu, 23 Feb 2023 19:37:08 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 19:56:18 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Feb 2023 19:56:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 23 Feb 2023 19:56:42 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Feb 2023 19:56:42 GMT
ENV LANG=C.UTF-8
# Thu, 23 Feb 2023 19:56:42 GMT
ENV JAVA_VERSION=20
# Thu, 23 Feb 2023 19:56:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Feb 2023 19:56:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1319f85bbd2aad3767d41a6c767c94c23f7432642c7bda3df878c147ba384902`  
		Last Modified: Thu, 23 Feb 2023 19:38:02 GMT  
		Size: 44.6 MB (44552452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fe2a72fd544bf059ba3dab17c20dd57232b65e41885f9004b841d0106f73b`  
		Last Modified: Thu, 23 Feb 2023 19:58:20 GMT  
		Size: 12.2 MB (12246468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677222843d4d6aaf2c835d46702235d78f22d46a5ea33993c035be791245f5ca`  
		Last Modified: Thu, 23 Feb 2023 19:59:32 GMT  
		Size: 198.1 MB (198126321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-rc-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c9e6e02355c50b606229e6fee8be195d1b3294062ddb25be5e4bcc9ff8377313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253160907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a08879983bbf5d3bedd73eb29eceeb9d48ce569642255a52b9b990f548054149`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Feb 2023 19:52:36 GMT
ADD file:650f46a4a6a15a9b2d6f048bb51976942936d0c5daba7b0337bceacbc4efcf85 in / 
# Thu, 23 Feb 2023 19:52:37 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 20:13:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Feb 2023 20:14:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 23 Feb 2023 20:14:21 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Feb 2023 20:14:21 GMT
ENV LANG=C.UTF-8
# Thu, 23 Feb 2023 20:14:21 GMT
ENV JAVA_VERSION=20
# Thu, 23 Feb 2023 20:14:34 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Feb 2023 20:14:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7166504978b203e953381fdfe4d9e7656565d62a75183fcc5bf460e6135e033d`  
		Last Modified: Thu, 23 Feb 2023 19:53:23 GMT  
		Size: 43.5 MB (43459902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766ec681792700cac3beb59912bb93402833e5171c8ae979918ee6806da3d433`  
		Last Modified: Thu, 23 Feb 2023 20:16:05 GMT  
		Size: 13.1 MB (13073314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7730f6d8361e1609b98a47d0f57035b11f5cf489bce4e960b828f7a6f3e6e0`  
		Last Modified: Thu, 23 Feb 2023 20:17:11 GMT  
		Size: 196.6 MB (196627691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
