## `openjdk:21-ea-oracle`

```console
$ docker pull openjdk@sha256:594903d68ce98eb81bceb83ac79a805578003ff082bc78cfb53556b90076f47a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:9a2f62fad44f09dcded2dee83fa59707f6b328a84af4bec6cd8fe4d7be2f4e7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263735828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8498aaffead77df48156fb51318fa5584f516b10b379e6a588d7771d4d954b5c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 02:04:16 GMT
ADD file:7a7c6d19e1a4f691c6bd96ea6b7568f6cc041fce11298e57d51913b978e9e7e3 in / 
# Tue, 04 Jul 2023 02:04:17 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 17:47:24 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 04 Jul 2023 17:48:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Tue, 04 Jul 2023 17:48:37 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 17:48:37 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 20:48:16 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 20:48:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 20:48:27 GMT
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
	-	`sha256:9f6f6013b8fc9447fe67d684b41c62470902a1d88c94e2d0eea528f73e52dd0a`  
		Last Modified: Mon, 10 Jul 2023 20:54:35 GMT  
		Size: 203.9 MB (203860975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:0d2d97e1c1a4e54c53698d7a6241ab02f12eaaa1089ee2e02644a3dca277bc39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.5 MB (261484442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c537c18fab97caa283eeedb8bd6081320e0ecd3bd579a1582824c98093123295`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Jul 2023 00:52:20 GMT
ADD file:1313260ee8b32fa94bcf06c44034cd7e4f9baf44c7df9e74facfe21323b37292 in / 
# Tue, 04 Jul 2023 00:52:21 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 01:17:20 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 04 Jul 2023 01:18:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Tue, 04 Jul 2023 01:18:57 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 01:18:57 GMT
ENV LANG=C.UTF-8
# Mon, 10 Jul 2023 21:34:37 GMT
ENV JAVA_VERSION=21-ea+30
# Mon, 10 Jul 2023 21:34:47 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='c35a1f2906d502e9f75a975165f4c86e29167ca8cc2d9d25b5351b46d90d4ab7'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/30/GPL/openjdk-21-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='ae690af5ffa639feba3bc04fc804480cdbc40b4099890c9d28dceac8f58f0426'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 10 Jul 2023 21:34:49 GMT
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
	-	`sha256:b0650ecd544fbbbba1e9a109f0db9d9134246711f7bc18fa9d232dd76f685cb8`  
		Last Modified: Mon, 10 Jul 2023 21:40:26 GMT  
		Size: 202.2 MB (202212200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
