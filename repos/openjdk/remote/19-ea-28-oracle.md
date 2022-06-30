## `openjdk:19-ea-28-oracle`

```console
$ docker pull openjdk@sha256:4ad8353ec3fd10f1508f6d2fa33e1e56fcf24ccca1dbb0407d425eeb66c3fc85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-28-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:0ae33bd36d6f1afd61b1587a2acded4d6c76f406ea51b55d9b0689908b858129
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248879075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f70c64b7ace69e4e938bbf959996ddedecde9704ce644c1b3e7b959a3b191a`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:20:45 GMT
ADD file:03d0377f5864198b250372de990ebf0ef7597cfdcc2e18421e8e0025394a7572 in / 
# Thu, 30 Jun 2022 17:20:46 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 17:37:33 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 17:38:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 30 Jun 2022 17:38:04 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 17:38:04 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 17:38:04 GMT
ENV JAVA_VERSION=19-ea+28
# Thu, 30 Jun 2022 17:38:13 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/28/GPL/openjdk-19-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='4a6c13cb4b548d924142b11ae8fbff7f5a9c2813f7663023389866e8c15cd2ee'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/28/GPL/openjdk-19-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='f553cff91a88a315ad6af41f8c7a4a4b7b72a2bec9886e136841f2bedd87421d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 17:38:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:337897a5aaf7b54e691e2ed305fbf00e0e8933d5a8a3c07d6fbb95f10b15c644`  
		Last Modified: Thu, 30 Jun 2022 17:21:37 GMT  
		Size: 39.2 MB (39221672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1e7c755c4cccc19ca62372088ce86de7711ff0e0e2e7e18f65711eb2299602`  
		Last Modified: Thu, 30 Jun 2022 17:45:09 GMT  
		Size: 13.5 MB (13509384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fc0267e80642430491c61b4197d6aef14adfeb5748fd9401bc3ac97379d398`  
		Last Modified: Thu, 30 Jun 2022 17:46:43 GMT  
		Size: 196.1 MB (196148019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-28-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:76e284c5efb73e5236124f5ed8d7b7f65115c5ac37874e61ce208f8376d606ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.3 MB (247307424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e3d5d16bce0ea369b20dc3e10ea2365d46c3c1d0f0c5cb6285eafa5847d0ba`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:40:34 GMT
ADD file:deb746f3cc547a36a34f3bfe68510bbd6f8a3b2da72bcca3cce36dfe0e519e77 in / 
# Thu, 30 Jun 2022 17:40:35 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 18:00:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 18:02:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 30 Jun 2022 18:02:05 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 18:02:06 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 18:02:07 GMT
ENV JAVA_VERSION=19-ea+28
# Thu, 30 Jun 2022 18:02:22 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/28/GPL/openjdk-19-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='4a6c13cb4b548d924142b11ae8fbff7f5a9c2813f7663023389866e8c15cd2ee'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/28/GPL/openjdk-19-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='f553cff91a88a315ad6af41f8c7a4a4b7b72a2bec9886e136841f2bedd87421d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 18:02:22 GMT
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
	-	`sha256:ce446c7afd8ad46e9b4761055bf68720a8ba1f8be72fad6a00b468b3851fa3f0`  
		Last Modified: Thu, 30 Jun 2022 18:17:14 GMT  
		Size: 195.0 MB (194980252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
