## `openjdk:18-oracle`

```console
$ docker pull openjdk@sha256:1f1370ff5836b46abf93f20aca0ecaf1a60d9c8a839e20acea09037e033922ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:0476bc0054cbed9b7fc6d8ddd6589ec43508bf63d6df5154910fd003128ec974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243541716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16afa2f591dba9fd7cd9625d99b28a5528c39d16b6b1781846760e5e8f97d7c0`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:22:47 GMT
ADD file:45a1eba89256c6e3801f14738faca9e260b17b306f0fc8769ba0b0f94f0fdf68 in / 
# Thu, 28 Oct 2021 01:22:47 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 01:44:41 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 28 Oct 2021 01:44:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 28 Oct 2021 01:44:41 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:44:41 GMT
ENV LANG=C.UTF-8
# Thu, 28 Oct 2021 01:44:41 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 28 Oct 2021 01:44:53 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='aa609b9f3a4a31b3cb3649a39dabf11476d9c5f1f3b8b9583b2be48e14e3c321'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a1bfee1fed3794347cfce38d0f4a163b7e90702ceb5fe9256d06664c0daa5726'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 28 Oct 2021 01:44:54 GMT
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
	-	`sha256:3719e81f67b1fc4a84131e65e6dc15d0549c6487b26afa7ceb5fa0d238e10ca2`  
		Last Modified: Thu, 28 Oct 2021 01:52:35 GMT  
		Size: 188.1 MB (188079257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:f3d087bc9e1efd9cde6d2ebfaf186876da63e2a44f20dbae196dd10216c5ca82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.1 MB (243142550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41ed085c49362c09f7bdb7b4576740de2267e16472b2a3fb36c0b65e1e085c49`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 14 Oct 2021 03:43:23 GMT
ADD file:f161e88dde917cf9d761056277b85a1880719b445048fc52649306cec001db66 in / 
# Thu, 14 Oct 2021 03:43:24 GMT
CMD ["/bin/bash"]
# Thu, 14 Oct 2021 05:42:19 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 14 Oct 2021 05:42:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 14 Oct 2021 05:42:21 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Oct 2021 05:42:22 GMT
ENV LANG=C.UTF-8
# Fri, 22 Oct 2021 02:16:38 GMT
ENV JAVA_VERSION=18-ea+20
# Fri, 22 Oct 2021 02:17:00 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='aa609b9f3a4a31b3cb3649a39dabf11476d9c5f1f3b8b9583b2be48e14e3c321'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/20/GPL/openjdk-18-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='a1bfee1fed3794347cfce38d0f4a163b7e90702ceb5fe9256d06664c0daa5726'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 22 Oct 2021 02:17:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a1eec3e47437e3334dd709f3a36be617982ec7579fa52be305301bb95c0d4be1`  
		Last Modified: Thu, 14 Oct 2021 03:44:37 GMT  
		Size: 41.9 MB (41877085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ec5552a84ea6485845e8e0a4d9b09b5e8f78d742440c18650d1ec9b1aacd89`  
		Last Modified: Thu, 14 Oct 2021 05:57:59 GMT  
		Size: 14.3 MB (14270572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606e2cfa96bfc5d10c9d12cc2503481dd3bd880d49c6089c1d5b01dc90159290`  
		Last Modified: Fri, 22 Oct 2021 02:33:10 GMT  
		Size: 187.0 MB (186994893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
