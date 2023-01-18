## `openjdk:21-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:7cef2cc05cdb9651e29c363f3d8b9077ce1b78c46336ce04ad863e392059570d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:2402cb765373293b2fdc23199df9c0ef019293fa034bb7a9e5c742dad5df1938
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.3 MB (255252754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10a69f3d0ce3157377272a9bfb9f231df750b7e91152e4a9150f9c03332c42bb`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 Jan 2023 21:49:30 GMT
ADD file:599abbad96e264361b1bc5a7643f88354e406a2a1f55256af8a67e5a71ac3044 in / 
# Tue, 17 Jan 2023 21:49:31 GMT
CMD ["/bin/bash"]
# Wed, 18 Jan 2023 04:26:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 18 Jan 2023 04:26:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 18 Jan 2023 04:26:54 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 04:26:54 GMT
ENV LANG=C.UTF-8
# Wed, 18 Jan 2023 04:26:54 GMT
ENV JAVA_VERSION=21-ea+5
# Wed, 18 Jan 2023 04:27:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/5/GPL/openjdk-21-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='2dba614859e77c261a7a30b3019b05dc1e7b5651d065de741426ea540a4ba264'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/5/GPL/openjdk-21-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='621f8196ad96481076d3730496db77ff154976c81798fc7ff3064cd1deeacdb8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 Jan 2023 04:27:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c57acc5afca507dabd7a22ed8ab1a978dad73d90dacad7b0b4668750f8fca64`  
		Last Modified: Tue, 17 Jan 2023 21:50:21 GMT  
		Size: 43.9 MB (43885845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8fb8780af51fbf2479bc74be4aef9eef6a67db84a17a1eadc0d9bb6464a16c`  
		Last Modified: Wed, 18 Jan 2023 04:31:02 GMT  
		Size: 12.3 MB (12251739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2b469e60d3705d1aa403d50c123f33fac5944924f143fc59197b38547e326f`  
		Last Modified: Wed, 18 Jan 2023 04:31:15 GMT  
		Size: 199.1 MB (199115170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e59fc1c8d73779956df8a6156861b44e4a5cd9aae5af03fbad70ef9620723533
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.4 MB (253416866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca4916db6edf900ba1404b926d75aae43dc17194aeefd49d822bf2f60e741e3`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 Jan 2023 22:11:15 GMT
ADD file:dc09c8b8bd2fd3e0439792a21b95984ec8104b2a384f5ea2ef173918c105da9c in / 
# Tue, 17 Jan 2023 22:11:15 GMT
CMD ["/bin/bash"]
# Wed, 18 Jan 2023 04:00:40 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 18 Jan 2023 04:00:40 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 18 Jan 2023 04:00:40 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 04:00:40 GMT
ENV LANG=C.UTF-8
# Wed, 18 Jan 2023 04:00:40 GMT
ENV JAVA_VERSION=21-ea+5
# Wed, 18 Jan 2023 04:00:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/5/GPL/openjdk-21-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='2dba614859e77c261a7a30b3019b05dc1e7b5651d065de741426ea540a4ba264'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/5/GPL/openjdk-21-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='621f8196ad96481076d3730496db77ff154976c81798fc7ff3064cd1deeacdb8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 Jan 2023 04:00:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:002eb071499b5ede36f617906154b8933e643acc41d2993585876528939fb80f`  
		Last Modified: Tue, 17 Jan 2023 22:11:59 GMT  
		Size: 42.8 MB (42775871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceecd3085b25f549de68213105de48a98b0db45a66e38d315c34ae860197f1a`  
		Last Modified: Wed, 18 Jan 2023 04:04:31 GMT  
		Size: 13.1 MB (13068620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09356457eeed50c1f04c45658eeee52eee158eeb86dd7135ff8c2db83eca57cb`  
		Last Modified: Wed, 18 Jan 2023 04:04:42 GMT  
		Size: 197.6 MB (197572375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
