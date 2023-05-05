## `openjdk:21-oraclelinux8`

```console
$ docker pull openjdk@sha256:0797a15ae44fa2bebf576424643f1f8d6ffd4d6e0fe256304a853d1d1db82855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:2cda4bcf7b4e8b9e1bf176acbaaaf1b3158ea621c5780fb3c02af99074c9e598
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.4 MB (261425627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f6592b9e0999bd8866641e9f07c57e37d48d585d6519315237dd68421479ac7`
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
# Thu, 04 May 2023 23:36:32 GMT
ENV JAVA_VERSION=21-ea+21
# Thu, 04 May 2023 23:36:42 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='218aa2d9ef829851d8eafe470922cefd372aa31b68cdab3aa0691c0492e6adde'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='449a26a88e27c331c9565a95892533f33792094f23f28a71b880a60588ddf0c2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 04 May 2023 23:36:42 GMT
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
	-	`sha256:0cbcaf598be57fb62fd8091c936361772a1ef5864880b450391d097af939cc31`  
		Last Modified: Thu, 04 May 2023 23:38:42 GMT  
		Size: 201.9 MB (201858771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:728a7010f5cc48db66d282d81694e49e9735a1490e831b0bf7a25cfc1b6e964c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259549195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5026f830fab4079d1c2fbd8f679feedb57b64d92744327188913e579ca91765`
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
# Fri, 05 May 2023 00:02:15 GMT
ENV JAVA_VERSION=21-ea+21
# Fri, 05 May 2023 00:02:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='218aa2d9ef829851d8eafe470922cefd372aa31b68cdab3aa0691c0492e6adde'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/21/GPL/openjdk-21-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='449a26a88e27c331c9565a95892533f33792094f23f28a71b880a60588ddf0c2'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 05 May 2023 00:02:27 GMT
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
	-	`sha256:bea4c362c99a98e6dc7e8a66e16cc575d85041f2e2b7fee35758b557ad1d8a96`  
		Last Modified: Fri, 05 May 2023 00:04:25 GMT  
		Size: 200.2 MB (200227527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
