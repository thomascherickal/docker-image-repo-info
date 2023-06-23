## `openjdk:21-ea-28-jdk-oracle`

```console
$ docker pull openjdk@sha256:f91e54d98fb9a56d0ed52e6ccf5670a7efdce7e5d8f26b750460e4304c268255
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-ea-28-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:1683b1496606b99953c1deb33ed9c3f645c34e9cd9ca6d4125fae9af78c71783
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.7 MB (263728465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e61056c26f5887bf79067e44998e475ee55bec8e38aa9e143ab668c193038499`
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
# Fri, 23 Jun 2023 00:27:25 GMT
ENV JAVA_VERSION=21-ea+28
# Fri, 23 Jun 2023 00:27:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-x64_bin.tar.gz'; 			downloadSha256='c5ff4dc462286ead4a7f1480719f695a976a130005df30d33ba210aadc094ff9'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/28/GPL/openjdk-21-ea+28_linux-aarch64_bin.tar.gz'; 			downloadSha256='4f98a729913be1d28fda8491420394e394fbbf84c4d1f41f05b83ba4c8b989aa'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:27:36 GMT
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
	-	`sha256:6768b713dca2216b7cdcaeade9f1d6091ac43c34a8fac151cb38a6d5dde530f1`  
		Last Modified: Fri, 23 Jun 2023 00:33:32 GMT  
		Size: 203.9 MB (203850477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
