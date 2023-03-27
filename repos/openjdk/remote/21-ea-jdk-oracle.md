## `openjdk:21-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:d44ff9db9bea8146dafe0efe02f35440c0e49bc362b818a8c2eadbce547397d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:0aed5cb6f9710553f09c0fa293553a227fa6c6414a8f772ec245d658f3ac3ae0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261020740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e80072c1e464ffef2d890e2059d8b31c467369a14a69c11c17c60f9046cdfef`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 22 Mar 2023 23:55:20 GMT
ADD file:1a06059b1a097ecc61cb02965fc90e00183a8653d9ae009965823226559c5be9 in / 
# Wed, 22 Mar 2023 23:55:20 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:15:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:15:05 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Mar 2023 00:15:05 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 00:15:05 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 00:15:05 GMT
ENV JAVA_VERSION=21-ea+14
# Thu, 23 Mar 2023 00:15:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='5ff9e95f12627e7f9c4b2e61d4ddfa5eb224f6106eff7620a487244be71d9787'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/14/GPL/openjdk-21-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='32b9ef0cafec4114aac8917e9ad754c7a3bdcfbc47143e4e5182757a0311ae66'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Mar 2023 00:15:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ab8798141d463c224f18fa5dd1d249b554dda61be24da7aa516e4e2de324db76`  
		Last Modified: Wed, 22 Mar 2023 23:56:08 GMT  
		Size: 44.6 MB (44563376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363fdaa54a1583c24462f316031891a2beb8144c7ccd8851f6b6a8869b86ed3b`  
		Last Modified: Thu, 23 Mar 2023 00:15:51 GMT  
		Size: 15.0 MB (15018388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c294c9204234fd36b4cd3499a8fb039514cf71b3e33696bb1b5b4a10cd1b91`  
		Last Modified: Thu, 23 Mar 2023 00:16:04 GMT  
		Size: 201.4 MB (201438976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:8473039b7c2ba0e3e7ee6225b37a5062ba14bd949fa4e335688cfbccbd4f0245
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259328852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26b6f4eed7220907963e1cedef695e65aaec03af3f0eb813a2ca2406456aabd7`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 22 Mar 2023 23:59:36 GMT
ADD file:b4a46acde2a8ffdb8874f11aadcfc90177b15422278a1b8fa87e7ed9c97cf2a4 in / 
# Wed, 22 Mar 2023 23:59:36 GMT
CMD ["/bin/bash"]
# Thu, 23 Mar 2023 00:23:23 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Mar 2023 00:23:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Mar 2023 00:23:24 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 00:23:24 GMT
ENV LANG=C.UTF-8
# Mon, 27 Mar 2023 22:47:17 GMT
ENV JAVA_VERSION=21-ea+15
# Mon, 27 Mar 2023 22:47:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-x64_bin.tar.gz'; 			downloadSha256='0fec1002b8c8975b181bd6966a817028d6b373cbc759254231f9b96db1fe6edd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/15/GPL/openjdk-21-ea+15_linux-aarch64_bin.tar.gz'; 			downloadSha256='93cc1eb6202093a127f1f9ed2e866a51dff29321f878085c18f317cefb113ffc'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Mar 2023 22:47:31 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:40ffb7074955cd4f083dfcadee0a1ef1e12dbe031bdf2325c8bae38711b1f70f`  
		Last Modified: Thu, 23 Mar 2023 00:00:22 GMT  
		Size: 43.5 MB (43460037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafbc18f0b64482aa39e4830fa399092a7a9f9a39c37c154966aa80bef2ece45`  
		Last Modified: Thu, 23 Mar 2023 00:24:08 GMT  
		Size: 15.8 MB (15834377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040306b2243af2d0f0852fada111b45b46ddd4c4bc2f41be268923fb25cba07f`  
		Last Modified: Mon, 27 Mar 2023 22:49:26 GMT  
		Size: 200.0 MB (200034438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
