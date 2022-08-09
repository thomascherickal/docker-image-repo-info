## `openjdk:19-ea-34-jdk-oracle`

```console
$ docker pull openjdk@sha256:7e34ac795a955c9b52eaba20511d1ff758fe1830839321e913d4456e3e42c6dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-34-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:177859802a9de531de78542029f8a759843db086edba9fee4e6467f03a8220a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248901718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9379295221fe6205e1be76e1212423aef85b4a4e90846c253d0a11d7dd8a709c`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:36:37 GMT
ADD file:0a05a213ae66f556b2b320291ac58ec9f2f67554e29338a072f1347f22864a49 in / 
# Thu, 04 Aug 2022 00:36:37 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:35:27 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:35:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 04 Aug 2022 01:35:57 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:35:57 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 22:52:59 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:53:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 22:53:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:32c1bf40aba1f372a057d3280b0b7cdacde9d8500a069004e6f243bc09cde806`  
		Last Modified: Thu, 04 Aug 2022 00:37:33 GMT  
		Size: 39.2 MB (39223952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d72ac1fb23a36f89addf60367990f28d5c0882e4b8f569c77b51c51eb271261`  
		Last Modified: Thu, 04 Aug 2022 01:42:41 GMT  
		Size: 13.5 MB (13506500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759b12086838c0cadc93bbe08dd3f35cd6565cb1307dbc34b28e7c6fe6bb9b46`  
		Last Modified: Mon, 08 Aug 2022 23:04:09 GMT  
		Size: 196.2 MB (196171266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-34-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:87b8ff3d086260cf3ed9ddcd0b549a351056553e2a84187d734a7476089fef53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.3 MB (247334316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b288690c01e858cdbcfe18357258664c8fa1803ed1d90f9e444111d7154800`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 04 Aug 2022 00:40:43 GMT
ADD file:a68d82fa032efe6adc2926f7e745508f0541bba3f906e2702d34252353100747 in / 
# Thu, 04 Aug 2022 00:40:44 GMT
CMD ["/bin/bash"]
# Thu, 04 Aug 2022 01:01:11 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 04 Aug 2022 01:02:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 04 Aug 2022 01:02:12 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 01:02:13 GMT
ENV LANG=C.UTF-8
# Mon, 08 Aug 2022 23:32:16 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 23:32:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-x64_bin.tar.gz'; 			downloadSha256='719889f7aaf988e7ec5c6edd0c3bd03342294f329a36dd6591af2e64f6aefae7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/34/GPL/openjdk-19-ea+34_linux-aarch64_bin.tar.gz'; 			downloadSha256='8d5d5327b1a7d35ae2c16ba69701cb58cb5b5df58f5ace295c08fe77d96a688b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 08 Aug 2022 23:32:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf56004177eb6ca162c88de29e84bc4ba3d2e7efd3703df9ecae51b89003d52`  
		Last Modified: Thu, 04 Aug 2022 00:41:51 GMT  
		Size: 38.0 MB (38023046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225b6ab834ff85ee0d347a2859ecb14fc169f362360408133589ab8a37d8333`  
		Last Modified: Thu, 04 Aug 2022 01:14:59 GMT  
		Size: 14.3 MB (14278746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6108e1a6eeb1984a19a306b3f37c0b9676fcfadb5ec712c6b45726cba6a851`  
		Last Modified: Mon, 08 Aug 2022 23:50:26 GMT  
		Size: 195.0 MB (195032524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
