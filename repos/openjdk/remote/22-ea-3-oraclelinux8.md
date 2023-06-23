## `openjdk:22-ea-3-oraclelinux8`

```console
$ docker pull openjdk@sha256:b9ba0122278c41155de4c85b8a22b5146f70a6a8c59cf59f94ae2c08648ef61f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-3-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:6e4c11886fe10de16ea1586c3ab13f7adfc82d173c3648958f8c7343eabc3d29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.5 MB (264512416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9ba18cc2d3a8bf85114e115d328973ad360d98552aab5100b6cf32ac8619b9`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 16 Jun 2023 00:20:42 GMT
ADD file:9f649031a04a4d0b24cc167d52bbd5ae3415fd808304c971291e35e75109822a in / 
# Fri, 16 Jun 2023 00:20:43 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:40:59 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 16 Jun 2023 00:40:59 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 16 Jun 2023 00:40:59 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 00:40:59 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jun 2023 00:25:46 GMT
ENV JAVA_VERSION=22-ea+3
# Fri, 23 Jun 2023 00:25:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='6541c5f5f08ec100af327c36768e302185851f548f6c33d1fe26250133998d5a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='e94529988d1c61d552981cc44896e13a1c49f3720567b2a92ad103f24291a167'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:25:58 GMT
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
	-	`sha256:56f32827efd0a6d03e1fcef00dd1a7d33cf09726994fd9cb2ab124c8c7efa16a`  
		Last Modified: Fri, 23 Jun 2023 00:30:06 GMT  
		Size: 204.6 MB (204634428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
