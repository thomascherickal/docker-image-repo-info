## `openjdk:21-jdk-oracle`

```console
$ docker pull openjdk@sha256:1f52cd81333f547e5ed2f521f15c316ad451e712599a67645dce96dafe01caed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:867eba7f5a50e3adda1399515db83340a2c34f24b05bcd2bf63fe5ae1380f217
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263739792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99cef28ee3a69fca278fa189ec2db617772e39564aeb74ef54cfd40281f2c80`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:40:59 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:41:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 16 Jun 2023 00:41:31 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 00:41:31 GMT
ENV LANG=C.UTF-8
# Tue, 04 Jul 2023 01:53:39 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 01:53:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='414ca270602b11d0b674c105d1d5577793c9db79e2947187e663dba4750cbf9b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='ddfa7ea3dd22c846676b4def3aef78a5411c208987ace8f47bbcfafd33f26f46'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 04 Jul 2023 01:53:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:46ef68baacb785b3cf2f2826bfce791acb5264bed0fdf301623ac0c3c57f4daf`  
		Last Modified: Fri, 16 Jun 2023 00:22:14 GMT  
		Size: 44.9 MB (44871780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df40f423a19e7cc991828aa15e47b0b84747ce895ae0ee55b8298f3bc44f03a3`  
		Last Modified: Fri, 16 Jun 2023 00:42:40 GMT  
		Size: 15.0 MB (15006208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82ff7a0ba0bdb954074e74397fd972893cd677977216fe1256fc67362e38911`  
		Last Modified: Tue, 04 Jul 2023 01:59:46 GMT  
		Size: 203.9 MB (203861804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:77c3e36ab0766ab3e652661f47f068a82b9cb9aa7dadeaa30d4bec83e7693192
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.5 MB (261482394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8680ccffd8d8802d1686900f160836f0c0f0cd4d734e0c0dc31bbb3f120de33`
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
# Tue, 04 Jul 2023 01:18:57 GMT
ENV JAVA_VERSION=21-ea+29
# Tue, 04 Jul 2023 01:19:06 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-x64_bin.tar.gz'; 			downloadSha256='414ca270602b11d0b674c105d1d5577793c9db79e2947187e663dba4750cbf9b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/29/GPL/openjdk-21-ea+29_linux-aarch64_bin.tar.gz'; 			downloadSha256='ddfa7ea3dd22c846676b4def3aef78a5411c208987ace8f47bbcfafd33f26f46'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 04 Jul 2023 01:19:08 GMT
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
	-	`sha256:1372d1f23e10b416844666f2ef75e8d30cda06791458ed603914ab857e61d9de`  
		Last Modified: Tue, 04 Jul 2023 01:24:49 GMT  
		Size: 202.2 MB (202210152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
