## `openjdk:19-rc-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:167aaf0388ef3830d5bff8205322b80c7d1391ace2339216babda4c4af3030ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-rc-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:a4da2027ccdd1ab184cf862c26a75cd03b48cab351f2d7151d4311473d168550
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.9 MB (247945746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a8fc74414b9fca2dd9d4e777a6748b2c2a20646aba50a8a9540e367e9db7483`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Aug 2022 21:20:34 GMT
ADD file:94f0ad5f0805806df710f02659592b7a0ee14643d54d40f0dca144e16c2c69ec in / 
# Tue, 30 Aug 2022 21:20:34 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:47:35 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Aug 2022 21:48:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 30 Aug 2022 21:48:06 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Aug 2022 21:48:06 GMT
ENV LANG=C.UTF-8
# Tue, 30 Aug 2022 21:48:06 GMT
ENV JAVA_VERSION=19
# Tue, 30 Aug 2022 21:48:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-x64_bin.tar.gz'; 			downloadSha256='f47aba585cfc9ecff1ed8e023524e8309f4315ed8b80100b40c7dcc232c12f96'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-aarch64_bin.tar.gz'; 			downloadSha256='682bfb48158ca198393c4b7fd38f873e8d6316b0bc6511a07e917f7f0f3afb03'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Aug 2022 21:48:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:492d84e496ea03370b8fb5b989ff003b89c51a2f037216835b8b3f93dcc4d405`  
		Last Modified: Tue, 30 Aug 2022 21:21:33 GMT  
		Size: 39.5 MB (39521774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d74542bd1abb51e0ea04904a65559d263d7f85b016fcbd81a65768553957ae`  
		Last Modified: Tue, 30 Aug 2022 21:51:36 GMT  
		Size: 12.2 MB (12240649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f07f63d12fb82c7fa664f5ef670381808f049c2f59270b3acb60bc2bb5f8256`  
		Last Modified: Tue, 30 Aug 2022 21:52:53 GMT  
		Size: 196.2 MB (196183323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-rc-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e09f15b4390f6478842c12d716e7150e8f2be2d1b3d3e33e5bab27460e9a18f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246387945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd652571ab4acaaf929bb4f32072df8ce87e65984d979d69b0b337b141529f49`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Aug 2022 20:47:49 GMT
ADD file:4f53d93ae4bccd786d6beda6f0ec4a450fd23a8fff2786d9e5b024a64aad6bb1 in / 
# Tue, 30 Aug 2022 20:47:50 GMT
CMD ["/bin/bash"]
# Tue, 30 Aug 2022 21:08:02 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Aug 2022 21:09:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 30 Aug 2022 21:09:25 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Aug 2022 21:09:26 GMT
ENV LANG=C.UTF-8
# Tue, 30 Aug 2022 21:09:27 GMT
ENV JAVA_VERSION=19
# Tue, 30 Aug 2022 21:09:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-x64_bin.tar.gz'; 			downloadSha256='f47aba585cfc9ecff1ed8e023524e8309f4315ed8b80100b40c7dcc232c12f96'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk19/877d6127e982470ba2a7faa31cc93d04/36/GPL/openjdk-19_linux-aarch64_bin.tar.gz'; 			downloadSha256='682bfb48158ca198393c4b7fd38f873e8d6316b0bc6511a07e917f7f0f3afb03'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Aug 2022 21:09:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fe1dbcd3b09e2c1e850118728988d6907b2f43969fe81443f422984829c640ce`  
		Last Modified: Tue, 30 Aug 2022 20:48:58 GMT  
		Size: 38.3 MB (38321155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43dbff7ac899e8f3413a3849ac2dcb6c61d52e9763a3cf5bc4c38d1e823fa3a`  
		Last Modified: Tue, 30 Aug 2022 21:16:28 GMT  
		Size: 13.0 MB (13042009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42cb8fd6e4651be05854d7a82e90af4b01255236043068d17a40192602ae8e3a`  
		Last Modified: Tue, 30 Aug 2022 21:18:06 GMT  
		Size: 195.0 MB (195024781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
