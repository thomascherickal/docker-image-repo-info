## `openjdk:21-rc-oraclelinux8`

```console
$ docker pull openjdk@sha256:8ecdacbf98495eb15b452e0b0cea66de86d6c042e416264fad571965599d7160
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-rc-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:f9774424407e984389bc655aef1bf5a7d6b7982959323061619aa8f43118e1c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.8 MB (263848505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:766d78857cbe4f2f0a4d2eb5fdacb2d425f6b56d90f2b786bf10dfb4315d926b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 01:20:36 GMT
ADD file:196115c6281a0a56854066be2766eb0dc9da452f60a060b90bbe681e6b8ffc11 in / 
# Fri, 11 Aug 2023 01:20:36 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:53:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:54:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 11 Aug 2023 01:54:38 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:54:38 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:04:02 GMT
ENV JAVA_VERSION=21
# Sat, 12 Aug 2023 00:04:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-x64_bin.tar.gz'; 			downloadSha256='a30c454a9bef8f46d5f1bf3122830014a8fbe7ac03b5f8729bc3add4b92a1d0a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk21/fd2272bbf8e04c3dbaee13770090416c/35/GPL/openjdk-21_linux-aarch64_bin.tar.gz'; 			downloadSha256='e8f4ed1a69815ddf56d7da365116eefc1e5a1159396dffee3dd21616a86d5d28'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:04:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b193354265ba898bb7548038f52378b3dbb6aac5afbaca49bb83ccfe51dfadeb`  
		Last Modified: Fri, 11 Aug 2023 01:21:58 GMT  
		Size: 44.9 MB (44910081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e75d2bbaed8a6321c319c610e5cd0923e1fc6a9ad6122e3b9573f10a5166f9e`  
		Last Modified: Fri, 11 Aug 2023 01:56:08 GMT  
		Size: 15.0 MB (15004378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ca4896ce47347bcdad08a003ac6c8caec2a623659f7559ad50b6cb172cc175`  
		Last Modified: Sat, 12 Aug 2023 00:10:32 GMT  
		Size: 203.9 MB (203934046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
