## `openjdk:20-oracle`

```console
$ docker pull openjdk@sha256:e2bc7178d86c3f6b4b0c3605d99e406c61ffaeba477e673c538659c492cb8748
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:4e68e1de8cab24c44b57a0bcce0887be45773d97f6f539265a884d84e9f1dd94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254065749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2969fc5399f6d007ac77fdb7a7c12afe3c71972664c0f500a0d30441f70449aa`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Nov 2022 19:20:57 GMT
ADD file:6767deed84cff167f77f7d9f835925cd8a5d3093d0b99f0180245cfd6312ae06 in / 
# Tue, 29 Nov 2022 19:20:58 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 19:43:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 29 Nov 2022 19:43:57 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 29 Nov 2022 19:43:57 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Nov 2022 19:43:57 GMT
ENV LANG=C.UTF-8
# Fri, 02 Dec 2022 00:21:20 GMT
ENV JAVA_VERSION=20-ea+26
# Fri, 02 Dec 2022 00:21:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 02 Dec 2022 00:21:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:996f1bba14d621751efdd3a7ff3a65db06e0edb9b3e211ef1c3e68223e053af7`  
		Last Modified: Tue, 29 Nov 2022 19:22:40 GMT  
		Size: 43.9 MB (43871608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1233d0894f0a77c915206fb2429d895953c3cef4150186d415a3c1c256a7f1`  
		Last Modified: Tue, 29 Nov 2022 19:48:00 GMT  
		Size: 12.2 MB (12246997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64167a12cc7912cb267670b192fbfc3d7c0196220e3cedf64b946227203b4ddf`  
		Last Modified: Fri, 02 Dec 2022 00:25:29 GMT  
		Size: 197.9 MB (197947144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3c2954de26adadf768236e44ece5d75e76bff855b07ec57651f0a81451f348d4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252338490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11497544e7715782afbe80706c24497acb84b901df3d0d4ba9e34d6c074d071c`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Nov 2022 19:48:22 GMT
ADD file:8919add412c121e3fffd8882c8379cfef3889b0d6b18afc150e1bd4a4bae08d4 in / 
# Tue, 29 Nov 2022 19:48:23 GMT
CMD ["/bin/bash"]
# Tue, 29 Nov 2022 20:06:02 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 29 Nov 2022 20:06:03 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Tue, 29 Nov 2022 20:06:03 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Nov 2022 20:06:03 GMT
ENV LANG=C.UTF-8
# Thu, 01 Dec 2022 23:43:14 GMT
ENV JAVA_VERSION=20-ea+26
# Thu, 01 Dec 2022 23:43:26 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 01 Dec 2022 23:43:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e16f89d504be05b35448ef4e921fc7ea5f090b53960d0bc6764f6d31a0ea2f4a`  
		Last Modified: Tue, 29 Nov 2022 19:49:52 GMT  
		Size: 42.8 MB (42775103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa7949e83b2b403f5e3a79f19d33aaa5ea4a1adb33854be91352471fec3fb34`  
		Last Modified: Tue, 29 Nov 2022 20:10:17 GMT  
		Size: 13.1 MB (13066550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18be7763bfbdfbd09a882cd9e195f9d94eed6950df2a624042a0defd91d3e4d3`  
		Last Modified: Thu, 01 Dec 2022 23:47:37 GMT  
		Size: 196.5 MB (196496837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
