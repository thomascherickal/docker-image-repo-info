## `openjdk:18-ea-5-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:92b0574e7aae14917e65c6603fe8a7d671f7fcf0998cdd42f3029c401e3f397b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-5-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:963d7f0e1293509695f581468c9986b02e3aadb46d75dbf67ec08dc095f93878
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243441704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64953b78f7ae1af8467a5339a490fa71b0de999e393b2aff7442261e136b4ee8`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jul 2021 20:20:57 GMT
ADD file:c830de449b9ecd90e02f56d99e8326701da17970fa314bd7b060fd9a7cf7ac77 in / 
# Mon, 12 Jul 2021 20:20:58 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 23:33:03 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 23:33:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Mon, 12 Jul 2021 23:33:04 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 23:33:04 GMT
ENV LANG=C.UTF-8
# Mon, 12 Jul 2021 23:33:04 GMT
ENV JAVA_VERSION=18-ea+5
# Mon, 12 Jul 2021 23:33:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='a50d2f7309f987ee33cfdfdfbd22c18ea8e6dc8a3bb21b582cd67fb97c906a82'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='28e3b50e98e75ae64d200ddcf87ba0664229e0659ccba3cd8ee2e25cbe6de24f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 12 Jul 2021 23:33:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c828c776e142cb23ad61c84403bb42deaa97efeda5e2b600df46f7dbd38ec681`  
		Last Modified: Mon, 12 Jul 2021 20:22:25 GMT  
		Size: 42.2 MB (42179737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8846dac42cae4499c0917b5bd5e81c0e6d6fcc5326d50972b3faed7ccdf688b8`  
		Last Modified: Mon, 12 Jul 2021 23:41:34 GMT  
		Size: 13.4 MB (13392657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed24551ac1f98ce693d69f36de301abef2a05e6a4de258600e7571fbc4b5333`  
		Last Modified: Mon, 12 Jul 2021 23:41:47 GMT  
		Size: 187.9 MB (187869310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-5-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:2e865629f600db863f175c195e7f362d527dd3c57454e9fc101b05e413ecbf65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.8 MB (242812685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d885ac4971fa923d41c1c1bdd87e12a157991f1ef1de15a8c7e3f1fa0bf099`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 12 Jul 2021 20:40:32 GMT
ADD file:a184ed870dc7a85028f7ba3bd0cf3820d6f1b94ac4cea1ac94ca48c786901041 in / 
# Mon, 12 Jul 2021 20:40:33 GMT
CMD ["/bin/bash"]
# Mon, 12 Jul 2021 21:03:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 12 Jul 2021 21:03:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Mon, 12 Jul 2021 21:03:06 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 12 Jul 2021 21:03:06 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jul 2021 00:11:35 GMT
ENV JAVA_VERSION=18-ea+5
# Tue, 13 Jul 2021 00:12:54 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='a50d2f7309f987ee33cfdfdfbd22c18ea8e6dc8a3bb21b582cd67fb97c906a82'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='28e3b50e98e75ae64d200ddcf87ba0664229e0659ccba3cd8ee2e25cbe6de24f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jul 2021 00:12:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6186b25cabd91cbdd2c6bf65b0c5ef261f52719e7c6c4d6252e7082b7a51b42e`  
		Last Modified: Mon, 12 Jul 2021 20:41:48 GMT  
		Size: 42.1 MB (42072715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8304774b066b61c2ae3dc6de204cb3d384a726b9376d301afc654577b50a9c0`  
		Last Modified: Mon, 12 Jul 2021 21:15:51 GMT  
		Size: 14.2 MB (14170180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dcb467d0ad7d1968a4c14db0d83056664f87a23fd6f9a0c012c51b4898e358`  
		Last Modified: Tue, 13 Jul 2021 00:26:50 GMT  
		Size: 186.6 MB (186569790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
