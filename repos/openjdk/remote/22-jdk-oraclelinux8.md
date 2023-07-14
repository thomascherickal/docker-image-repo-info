## `openjdk:22-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:82a15678738a2cd1bf0fa38c40e89fee1ece7d124bbce9d6b0aaefc172239923
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:234f44d66b312a59c5496fc113cfc029421d8c88a3583e37b34617ae65ac75d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.6 MB (264565813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a7ae89e6e601d86e878dca1eca230f222dcfd1ea299ba03553bf8c0c9e9c126`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 17:47:24 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 04 Jul 2023 17:47:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Tue, 04 Jul 2023 17:47:25 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:47:25 GMT
ENV LANG=C.UTF-8
# Fri, 14 Jul 2023 00:33:00 GMT
ENV JAVA_VERSION=22-ea+6
# Fri, 14 Jul 2023 00:33:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-x64_bin.tar.gz'; 			downloadSha256='c0f9b77f4e63ceed956850811dd605aab708ed3251fdcb20bc4b34e46e98142d'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-aarch64_bin.tar.gz'; 			downloadSha256='d42979ec7c71a40dcadb323c40a19068416045a32b0b8d950d7bfc96ae75197e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Jul 2023 00:33:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e2c03c89dcad02e83fe01768b82c438fcf60b831104614ca96ed5d8df01db295`  
		Last Modified: Tue, 04 Jul 2023 02:05:27 GMT  
		Size: 44.9 MB (44876686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1589371ef7dbf0bbba39e839420d2a593e729690f3c9a3a1cc86d3cd6b47912`  
		Last Modified: Tue, 04 Jul 2023 17:50:16 GMT  
		Size: 15.0 MB (14998167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b064a35e1ad0a6ff947dcb3d78c0b6be4c3f9e3d319682fc37f5a8d5c1e043d`  
		Last Modified: Fri, 14 Jul 2023 00:37:30 GMT  
		Size: 204.7 MB (204690960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b876a9f1a6df89ef490f3bcdf671f8c99adb58f12969af3c1aa473d75beaf0e7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.3 MB (262290451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c4d6da8639c0ad2249987184d16bbd5a44d047a2696116363810663a84759c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:17:20 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:17:20 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Tue, 04 Jul 2023 01:17:21 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 01:17:21 GMT
ENV LANG=C.UTF-8
# Fri, 14 Jul 2023 00:44:21 GMT
ENV JAVA_VERSION=22-ea+6
# Fri, 14 Jul 2023 00:44:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-x64_bin.tar.gz'; 			downloadSha256='c0f9b77f4e63ceed956850811dd605aab708ed3251fdcb20bc4b34e46e98142d'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/6/GPL/openjdk-22-ea+6_linux-aarch64_bin.tar.gz'; 			downloadSha256='d42979ec7c71a40dcadb323c40a19068416045a32b0b8d950d7bfc96ae75197e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Jul 2023 00:44:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:29e800056b7e3d5007df41c0ad55416bb45d5863affcf39316c5755e71b20a30`  
		Last Modified: Tue, 04 Jul 2023 00:53:16 GMT  
		Size: 43.6 MB (43595268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4e6eec249ed9ec194f18c4c5eda620b32132cc41a2083ec5505ff863774f15`  
		Last Modified: Tue, 04 Jul 2023 01:21:26 GMT  
		Size: 15.7 MB (15676974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc867d2331b14b0e42d4e60a951bc2c2de000afa72053211d21358f3dbb2e3d6`  
		Last Modified: Fri, 14 Jul 2023 00:48:47 GMT  
		Size: 203.0 MB (203018209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
