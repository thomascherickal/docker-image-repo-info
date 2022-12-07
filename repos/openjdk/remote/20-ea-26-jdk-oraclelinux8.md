## `openjdk:20-ea-26-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:9f6d30a1685a6cf2599eeab7534bc767dd2b19d18944f2031d86d61d8031a100
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-26-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:4cebacadf67cdaa780281a7bc2ae31cc27f00a82f19e5f11920e1c340ed07c60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254064274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a414286d4c552c92c5feb55aed3fe62346de77136541f6662f9aa121bb93d10d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 07 Dec 2022 01:51:27 GMT
ADD file:04d9ae26c2acac414b69a784563f765d531aeaf941ea0341025b4544f9ade244 in / 
# Wed, 07 Dec 2022 01:51:27 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:27:04 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:27:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 07 Dec 2022 02:27:04 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:27:04 GMT
ENV LANG=C.UTF-8
# Wed, 07 Dec 2022 02:27:04 GMT
ENV JAVA_VERSION=20-ea+26
# Wed, 07 Dec 2022 02:27:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 07 Dec 2022 02:27:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0ed027b72ddc5d1a749fc58b7c26610167393b08ae71ef6625496508903f70a2`  
		Last Modified: Wed, 07 Dec 2022 01:53:11 GMT  
		Size: 43.9 MB (43868738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3502f40d35be69b4df858d92b5ac60d6b792eec7beabb7cbd78c816329f47b7f`  
		Last Modified: Wed, 07 Dec 2022 02:30:44 GMT  
		Size: 12.2 MB (12248357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ead438c9eea2b871e5d1f7ea675c220c920d68f93386ffb098844c6a06b885`  
		Last Modified: Wed, 07 Dec 2022 02:30:57 GMT  
		Size: 197.9 MB (197947179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-26-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:baa606bee40c57f2ec25c7f680af8a1eee3b260891ac8f09a4c0ce4ab5abbe92
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252327868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce155a3eab376d805ea308764bbc3f0a135ca66b14f3222ecc3f57b3379fced`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 07 Dec 2022 02:10:44 GMT
ADD file:6fdd782c2779edf7149126e79dcb46ebde32975107cdd5d129cce0860e797cde in / 
# Wed, 07 Dec 2022 02:10:44 GMT
CMD ["/bin/bash"]
# Wed, 07 Dec 2022 02:53:05 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 07 Dec 2022 02:53:05 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 07 Dec 2022 02:53:06 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 07 Dec 2022 02:53:06 GMT
ENV LANG=C.UTF-8
# Wed, 07 Dec 2022 02:53:06 GMT
ENV JAVA_VERSION=20-ea+26
# Wed, 07 Dec 2022 02:53:14 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='70075a76ed683898d8d71852394c88ab73d8665b15accfafa85dac3be5fbf87e'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/26/GPL/openjdk-20-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='041c2b0e7b68e58376d8b03db365434ceecd65671de20af28e6c32f47ccde94a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 07 Dec 2022 02:53:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:12a06ca91af857ea3cb02aedc5c643c5f06865868ae5c386c8ea664be60ead7e`  
		Last Modified: Wed, 07 Dec 2022 02:12:09 GMT  
		Size: 42.8 MB (42772059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122e459b46a4edc515fedc5c9be076b28ba6b0606f3cc90d412ea3d88b15576e`  
		Last Modified: Wed, 07 Dec 2022 02:57:10 GMT  
		Size: 13.1 MB (13058882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338d0c2e681c3a611efedd9c0fb2c532c3945690316d8f8ab5d8c904582b3584`  
		Last Modified: Wed, 07 Dec 2022 02:57:20 GMT  
		Size: 196.5 MB (196496927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
