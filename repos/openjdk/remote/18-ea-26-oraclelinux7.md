## `openjdk:18-ea-26-oraclelinux7`

```console
$ docker pull openjdk@sha256:7c020c956714c4766941abaaca24ba2adc745d0c1ea575eac68c9d201c1c85d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-26-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:e824573fbbb59ad5d38f857a79c5956a7aa0f035d7e7c29a11d40df16f6aaa2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252288626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0566a23aa87edf680acf046f9fe84722d21a35a8ab4e860ae2a55ffaf35d8844`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 03:36:07 GMT
ADD file:f1e23cb77895c4f36fa773b22bdbd74dfd2a144a4da854f13fd100d73f5517d8 in / 
# Thu, 02 Dec 2021 03:36:07 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:28:23 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 02 Dec 2021 11:28:23 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 02 Dec 2021 11:28:24 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:28:24 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Dec 2021 23:46:41 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:46:52 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='fdf145c2819ef28edee67b7a6605bee89aefc505a1abea1686bec03fcba87c70'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='14e35be6e99a093bd4d5666bd4d557ebb94ab9e03eab9e9ae0eb69fc7b3e662b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Dec 2021 23:46:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f09c1d3b7e7b9dae0fc06393c0a6ae2becfdaf108965c4634fb5aa08ef682b39`  
		Last Modified: Thu, 02 Dec 2021 03:37:01 GMT  
		Size: 48.3 MB (48330617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0bdeb652c6947210f8fca8bc5216da702dcb944e14fb6272fde14a87c1834`  
		Last Modified: Thu, 02 Dec 2021 11:46:03 GMT  
		Size: 15.4 MB (15388709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd360b527d9693075864c40919e387ff628ee7519430fee0d776256439c7cab`  
		Last Modified: Fri, 03 Dec 2021 23:54:10 GMT  
		Size: 188.6 MB (188569300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-26-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d081db1c30fff7128390b0d4b1f2c2cae2857925355896c0c40f82d5d70d7a12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252875448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c89945050c4682f07a895ae52b3abbcdb1cc2860e34966ce943dcc35e155e2`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 08:51:25 GMT
ADD file:9e54130641553fdfd5c6fccb94502b8821e5f6a3a312a5b58537b439bf8b2670 in / 
# Thu, 02 Dec 2021 08:51:26 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:01:07 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 02 Dec 2021 11:01:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 02 Dec 2021 11:01:09 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:01:10 GMT
ENV LANG=en_US.UTF-8
# Fri, 03 Dec 2021 23:08:28 GMT
ENV JAVA_VERSION=18-ea+26
# Fri, 03 Dec 2021 23:08:45 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='fdf145c2819ef28edee67b7a6605bee89aefc505a1abea1686bec03fcba87c70'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/26/GPL/openjdk-18-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='14e35be6e99a093bd4d5666bd4d557ebb94ab9e03eab9e9ae0eb69fc7b3e662b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 03 Dec 2021 23:08:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:badc99e3da86862c7fae71e717cef8fd1a5a34023f0932c8c979275fb8de6a32`  
		Last Modified: Thu, 02 Dec 2021 08:52:20 GMT  
		Size: 48.9 MB (48905570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56494d755d6c4fa6e0ed158c6946591b3ec2ad7e02e9c86d1434bcf5b27c263`  
		Last Modified: Thu, 02 Dec 2021 11:21:55 GMT  
		Size: 16.5 MB (16464679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f64a595f0912e790552d51354eb7731cacdd7bd9f8ca743695afdc914184604`  
		Last Modified: Fri, 03 Dec 2021 23:20:45 GMT  
		Size: 187.5 MB (187505199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
