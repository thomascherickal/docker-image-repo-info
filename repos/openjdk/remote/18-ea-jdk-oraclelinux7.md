## `openjdk:18-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:c38242150ee33cecf993dc3967bf7ea0315ec7e53241bb3d9cf87a69d17847ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ce4c326af7ac5a60c8ca40f44ae6ebb71a43eb165afe0d18716114faa2ae9241
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.0 MB (251995533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95bb93f8d111d78b4b3aafe543ea16de5c32e350d9517726baf0852b2f6f63c3`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:23:11 GMT
ADD file:1ba19f36d1d89d348cc182f0c7feb2c27bcca7bd084032525deaba8822462091 in / 
# Thu, 28 Oct 2021 01:23:11 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 01:45:25 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 28 Oct 2021 01:45:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 28 Oct 2021 01:45:25 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 01:45:25 GMT
ENV LANG=en_US.UTF-8
# Thu, 11 Nov 2021 02:28:04 GMT
ENV JAVA_VERSION=18-ea+22
# Thu, 11 Nov 2021 02:28:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='71124796aac929f184d54cf5b2a3ba3a31c0cef1ba9b5b5e1535ec5a5d482a8b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='714a0b84e6ed39e5442ca0044dab9ebecddeceffc9b78aed8e4d7ba2fbefb8aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 11 Nov 2021 02:28:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a755c2d4aa362701b6bb477a4b1cb2594cb0dca6d0e6839e07b0636fb824c7f7`  
		Last Modified: Thu, 28 Oct 2021 01:24:42 GMT  
		Size: 48.3 MB (48328962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d0464e417ebb82551686797f3772337ca857388f6f2209630af5603196a562`  
		Last Modified: Thu, 28 Oct 2021 01:53:12 GMT  
		Size: 15.4 MB (15399150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60632eff72aeb95abb140b5e33b41e9e4d1f089f71271807f25b3f35c9257b0b`  
		Last Modified: Thu, 11 Nov 2021 02:35:25 GMT  
		Size: 188.3 MB (188267421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b461fb6d61e0024c1be00833b97537c2c3db57655ad5c8e717bf6a01df576c74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.5 MB (252548160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68d602f79c83d6ac58d86f3c5dabaf2d208aec518ca7e687f68d3644bc433cf4`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 28 Oct 2021 01:44:12 GMT
ADD file:f997c704e003e7bef1e40d457d005aa07a60cb4c37255cc2711119deb3e6df7d in / 
# Thu, 28 Oct 2021 01:44:13 GMT
CMD ["/bin/bash"]
# Thu, 28 Oct 2021 02:16:09 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 28 Oct 2021 02:16:10 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 28 Oct 2021 02:16:11 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 Oct 2021 02:16:12 GMT
ENV LANG=en_US.UTF-8
# Thu, 11 Nov 2021 03:03:12 GMT
ENV JAVA_VERSION=18-ea+22
# Thu, 11 Nov 2021 03:03:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-x64_bin.tar.gz'; 			downloadSha256='71124796aac929f184d54cf5b2a3ba3a31c0cef1ba9b5b5e1535ec5a5d482a8b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/22/GPL/openjdk-18-ea+22_linux-aarch64_bin.tar.gz'; 			downloadSha256='714a0b84e6ed39e5442ca0044dab9ebecddeceffc9b78aed8e4d7ba2fbefb8aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 11 Nov 2021 03:03:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9e1221f69ca9b4fd1daae21b9a20e7225f6ca7d0e34e9e998bc6600de1a3836a`  
		Last Modified: Thu, 28 Oct 2021 01:45:43 GMT  
		Size: 48.9 MB (48905370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b5770e043e6b3a738c83528c0b9c0c9be1c26e18eea50e4a5c270c853ccb2e`  
		Last Modified: Thu, 28 Oct 2021 02:29:48 GMT  
		Size: 16.5 MB (16454087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca6f204e54eb02d7c409bb1207527b66949905f7934c00b5aeee7533bb8e81`  
		Last Modified: Thu, 11 Nov 2021 03:16:03 GMT  
		Size: 187.2 MB (187188703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
