## `openjdk:22-ea-8-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:5e17875c057fd2d50000712265ac3583a9b020e37ddc6f82da61ea763faecae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-8-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:fd90dfab12efcfcec28b7d4388a99eeee766cd168f6b19411a590d9b06b661bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269506190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e30cb0d59cea77c38f85ba1c0f03e4cce9d0eaf6e4000e7098472d90204027`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:56:49 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 09:56:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Wed, 14 Jun 2023 09:56:49 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 09:56:49 GMT
ENV LANG=en_US.UTF-8
# Thu, 03 Aug 2023 01:45:42 GMT
ENV JAVA_VERSION=22-ea+8
# Thu, 03 Aug 2023 01:46:04 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='f05e7933726ce10c3789634d099fdf1b3e61ae9d633aae85fa22ed92ed0a8bac'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='ee073fed6cbf145e5e3a06384d3e8f99ee22179cbb4049e1af2dc01275290900'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:46:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:70e9ff4420fbc58483e68c13199a06c24b14013b2548998a7e367f59ca5157bc`  
		Last Modified: Wed, 14 Jun 2023 07:22:30 GMT  
		Size: 50.5 MB (50484765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4714d29e017353e367cfbeb707bad46a96692fceb51533b3749c668baf3b5b8f`  
		Last Modified: Wed, 14 Jun 2023 09:58:27 GMT  
		Size: 14.2 MB (14242764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdbccd1bf3e73428f6eb676e3d0ebdfd447d1df0e456c8d65ccbb0897c7be1f`  
		Last Modified: Thu, 03 Aug 2023 01:52:55 GMT  
		Size: 204.8 MB (204778661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
