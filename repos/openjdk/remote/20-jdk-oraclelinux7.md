## `openjdk:20-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:47ff60d722cd34ebb529d8d9cc2ca251fde3cf8057ebe53b84cc5f39a0ee05c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:1ed0510af461abf125e10373b04fb3d7d1201b616ea01ab944f2180379932759
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261165341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21484727a4026a1c1196bc9d04973c23d0125011d052e79ba819869ab7b1854c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Oct 2022 20:32:03 GMT
ADD file:d7b7ed3315719e2a7f19233b68dbf42298d9d6e1a882de7154751ad29710eeac in / 
# Fri, 07 Oct 2022 20:32:03 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 20:50:44 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 07 Oct 2022 20:50:45 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 07 Oct 2022 20:50:45 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 20:50:45 GMT
ENV LANG=en_US.UTF-8
# Fri, 14 Oct 2022 01:48:01 GMT
ENV JAVA_VERSION=20-ea+19
# Fri, 14 Oct 2022 01:48:11 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/19/GPL/openjdk-20-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='872bf878e925d040e586f05723275d769f00f5718745e0758e6345ab2ffa0b66'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/19/GPL/openjdk-20-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='3ea4c7aa0de5ed4d0e5e0d55d2ef9cfa261087e65af3fdf849ecb2186a414c0d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 14 Oct 2022 01:48:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0056409b8e897373ba0cef19c5e1f387c06dafd5e11f3f2f0f22d34c8acb6717`  
		Last Modified: Fri, 07 Oct 2022 20:34:25 GMT  
		Size: 49.9 MB (49869229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f738e86ce06f94dc5d19ca70ae49d8b2442605a4c05912a8a401f2a0d6da130a`  
		Last Modified: Fri, 07 Oct 2022 20:54:58 GMT  
		Size: 14.2 MB (14241449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc723e8b233210986a7b6950c622a631163680047c13d9aed5f0f097c7e9427`  
		Last Modified: Fri, 14 Oct 2022 01:52:45 GMT  
		Size: 197.1 MB (197054663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:197cce286fdf6dbe05a0270a6c26d9f797032699798e14f3f638c4fdce897a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261199288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5653aa17fad798e928a29b6045a9208b3af2985f8ace5830257edf11dee8d53`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Oct 2022 20:52:08 GMT
ADD file:bd392af27b158db82c5b1c7acfd7aa49ada7d4eda11ea878a109b9c92f64b349 in / 
# Fri, 07 Oct 2022 20:52:09 GMT
CMD ["/bin/bash"]
# Fri, 07 Oct 2022 21:14:39 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 07 Oct 2022 21:14:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Fri, 07 Oct 2022 21:14:40 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 21:14:41 GMT
ENV LANG=en_US.UTF-8
# Sat, 08 Oct 2022 00:21:21 GMT
ENV JAVA_VERSION=20-ea+18
# Sat, 08 Oct 2022 00:21:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1081d9b6e6439841c3665fe65caf47431f7a6208ff6da8ee66a617a5577754c1'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/18/GPL/openjdk-20-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='92161bb7811ac65f8a1deddef23028d817634cab1605a7255aefb517c2a2f6f8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 08 Oct 2022 00:21:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0e5c63cf456b69584a9fa30dc0b1a5bca10abe38570de2326383f28a61ba1733`  
		Last Modified: Fri, 07 Oct 2022 20:54:19 GMT  
		Size: 50.4 MB (50440495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ebea763a2ab54a09b2c1fb8539a9b9f04dd09c1dbfc8c2ac2cf27892200da8`  
		Last Modified: Fri, 07 Oct 2022 21:22:10 GMT  
		Size: 15.3 MB (15260688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bd322d3378b8cd149cf392f708c268559d22246fdcb6542c9a691acaeb8647`  
		Last Modified: Sat, 08 Oct 2022 00:29:22 GMT  
		Size: 195.5 MB (195498105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
