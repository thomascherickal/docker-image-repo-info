## `openjdk:21-ea-19-oracle`

```console
$ docker pull openjdk@sha256:9b9499f2e046bd29d7f9f029f4ea3277bee95759a5bc95c9d66a911424322273
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-19-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:8775a716b7c04a81fea3b1175093bbb15a552afd811df32170fc551d18358f9e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261149539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9773d723c7caf27bc340d3a9e2864208bc2262ec09ce3885ce23922e6e9ce534`
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
# Fri, 21 Apr 2023 20:07:06 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:07:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:07:17 GMT
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
	-	`sha256:151eac6a77aaab1f773ddb55f22d2cf691acf5fb956f87ec4edf2717d593ab43`  
		Last Modified: Fri, 21 Apr 2023 20:09:17 GMT  
		Size: 201.6 MB (201582683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-19-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:073653029c0d9bc107a0291190e4bf0147ecf894a0f72e5ff268a5cd26d0a694
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259264721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8675c655a59963347c00523add61401e12e40986f8939b1a505c919c4504dda7`
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
# Fri, 21 Apr 2023 20:22:25 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 20:22:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5af95497753fbc33981f5ab1267fbd3be57e4095ceca9806490a25b56f819007'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/19/GPL/openjdk-21-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='d08fe17feea7fa18c4e9ee9918496974d0194d1fac9a485d47cc2d30601c3682'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 21 Apr 2023 20:22:37 GMT
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
	-	`sha256:4a3807b8c3f2ff2a75ff784add21e8d11bf2668038951a28ca165b0523a41b01`  
		Last Modified: Fri, 21 Apr 2023 20:24:33 GMT  
		Size: 199.9 MB (199943053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
