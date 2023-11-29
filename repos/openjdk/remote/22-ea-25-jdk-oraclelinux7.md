## `openjdk:22-ea-25-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:96aa146916389da59988dbf1f00f26d1b1c46f7ec5287d2cd08d670917c43140
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-25-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:9c5b353526e1c07d67433ab744f02f48a9fc32f37b80c9571ea9048715ef7feb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.1 MB (269069483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18244b5d684bae58a32e3538fdd34849df3a073f13fed6129a0de8dac9b6125b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 14 Nov 2023 18:20:58 GMT
ADD file:3e0277519395faaec643f0d6752812c14478974d1a914a763327a3cf30bbd28c in / 
# Tue, 14 Nov 2023 18:20:58 GMT
CMD ["/bin/bash"]
# Tue, 14 Nov 2023 18:46:40 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 14 Nov 2023 18:46:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Tue, 14 Nov 2023 18:46:41 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:46:41 GMT
ENV LANG=en_US.UTF-8
# Wed, 29 Nov 2023 01:45:13 GMT
ENV JAVA_VERSION=22-ea+25
# Wed, 29 Nov 2023 01:45:37 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/25/GPL/openjdk-22-ea+25_linux-x64_bin.tar.gz'; 			downloadSha256='0f98721a88a1dd380773adbf29dd79df25be9b69045c3266f913ecacc5e74d3e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/25/GPL/openjdk-22-ea+25_linux-aarch64_bin.tar.gz'; 			downloadSha256='ea5fc28e7b6ed0a5da04b4740a35d8dd26bb68a48a516da2d002359d817ba35c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Nov 2023 01:45:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:11a38aebcb7ae84df8b4fdcc1c7540389829a1f599b7a9986df89df733b69cea`  
		Last Modified: Tue, 14 Nov 2023 18:22:00 GMT  
		Size: 50.5 MB (50499111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d855689795ad008f2a59d12fd4c1661d113041ec2efd3339b326986f9ee7f96f`  
		Last Modified: Tue, 14 Nov 2023 18:47:56 GMT  
		Size: 14.3 MB (14252430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200e00a5cc9af02a5deca8fbd98b0f35f8a4fe8453c52715ebbd6a19eac02b68`  
		Last Modified: Wed, 29 Nov 2023 01:49:12 GMT  
		Size: 204.3 MB (204317942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-25-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b0b71585c69fb840f6b7062ed924f64cfd28ab9f15e11a61ce8a189315c034e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.7 MB (268738114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65a7432f1bc58e4d1a851d646cc76b1cc66fd647e970df6e8e4a78cbb9073853`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 14 Nov 2023 18:47:13 GMT
ADD file:0429c6e46360abe0bf4baedbcca5a063b60eb02c2b38c8642fd5e6d6431f2216 in / 
# Tue, 14 Nov 2023 18:47:14 GMT
CMD ["/bin/bash"]
# Tue, 14 Nov 2023 19:11:54 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 14 Nov 2023 19:11:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Tue, 14 Nov 2023 19:11:54 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 19:11:54 GMT
ENV LANG=en_US.UTF-8
# Wed, 29 Nov 2023 06:31:14 GMT
ENV JAVA_VERSION=22-ea+25
# Wed, 29 Nov 2023 06:31:26 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/25/GPL/openjdk-22-ea+25_linux-x64_bin.tar.gz'; 			downloadSha256='0f98721a88a1dd380773adbf29dd79df25be9b69045c3266f913ecacc5e74d3e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/25/GPL/openjdk-22-ea+25_linux-aarch64_bin.tar.gz'; 			downloadSha256='ea5fc28e7b6ed0a5da04b4740a35d8dd26bb68a48a516da2d002359d817ba35c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 29 Nov 2023 06:31:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:234b67cef5b9c7021cf94a462ae8c27e19f05d8ab6020a2c08b47a355a51757e`  
		Last Modified: Tue, 14 Nov 2023 18:48:16 GMT  
		Size: 51.1 MB (51110162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3db892ec75a05fe3c6e1f29c7ee60b17e26e42c96c7901605d8be961e62e5a`  
		Last Modified: Tue, 14 Nov 2023 19:12:57 GMT  
		Size: 15.2 MB (15245362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73003877e6f9f632e9fa1ced45f2f24af2a83928cefca202ce7afcb3f2914428`  
		Last Modified: Wed, 29 Nov 2023 06:33:59 GMT  
		Size: 202.4 MB (202382590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
