## `openjdk:21-oraclelinux8`

```console
$ docker pull openjdk@sha256:11f572172ded05aa7e3b7cc45e0d302643163087d82fc8d733f89d84b9527fa0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:05e6b8b134f07526bf7ebd595f04c8efb3121988bde553ae4c95e5c5737bd6a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (260981415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913d280a1b28669439bd4aa49762aaa5435dacb828bc4befc0fd3430f88df30a`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 06 Apr 2023 18:20:31 GMT
ADD file:61a2085af5116916e7b117c2e7ad7116bdc0282d8fa9ce76191c4101f5e866ff in / 
# Thu, 06 Apr 2023 18:20:32 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:37:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:37:15 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 06 Apr 2023 18:37:15 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Apr 2023 18:37:16 GMT
ENV LANG=C.UTF-8
# Sat, 15 Apr 2023 00:30:03 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:30:14 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:30:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:328ba678bf27575937f8b9dfbf5b5f39b21941af068f8e5960de8131e289da85`  
		Last Modified: Thu, 06 Apr 2023 18:21:19 GMT  
		Size: 44.6 MB (44563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55560f49b1cd4515e5c12b0a190ca11492533ca3757e761c254daf809031bdc5`  
		Last Modified: Thu, 06 Apr 2023 18:38:00 GMT  
		Size: 15.0 MB (15002954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3543229fa802e7798f2e2c8826071fcb13f5657c2f9a6d7a0e245a3ba6238ffd`  
		Last Modified: Sat, 15 Apr 2023 00:32:23 GMT  
		Size: 201.4 MB (201414559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:0f799e2213739b05d1fb3282226131232310243f89d36fe3deee90614f44873c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.1 MB (259091148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e885078103e0421707d2cf2fea515a22b96657bff0196cd52391a3ec4b2ae5`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 06 Apr 2023 18:40:07 GMT
ADD file:c798bcae4b9271a204dc37f132bce1f0042c02cb1ad5a2237f56dec227d44438 in / 
# Thu, 06 Apr 2023 18:40:07 GMT
CMD ["/bin/bash"]
# Thu, 06 Apr 2023 18:59:01 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 06 Apr 2023 18:59:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 06 Apr 2023 18:59:01 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Apr 2023 18:59:01 GMT
ENV LANG=C.UTF-8
# Sat, 15 Apr 2023 00:55:31 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:55:41 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='1c6d7b740ced597243d8c05f823f81728a618c73ffa4cbe28a6d3e2eba02ce00'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/18/GPL/openjdk-21-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='b0009295c1ef02c743fc272b654b11bd506714e8efedc881295a1de74e87d8a8'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 15 Apr 2023 00:55:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6425367b44c9c3f59fd1e81f8fa2e9170ca2ef552d63f35a08ef3969ee4ff557`  
		Last Modified: Thu, 06 Apr 2023 18:40:43 GMT  
		Size: 43.5 MB (43477048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57603b9946d65e0ac1577d90598fe906f0885a24be64058c4412b3d03b03a59a`  
		Last Modified: Thu, 06 Apr 2023 18:59:42 GMT  
		Size: 15.8 MB (15844620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694cbfe2e30e106b747b3633e474d2a3db4b26f2af40848029dc982b4bcf5ded`  
		Last Modified: Sat, 15 Apr 2023 00:57:35 GMT  
		Size: 199.8 MB (199769480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
