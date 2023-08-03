## `openjdk:21-ea-33-oraclelinux7`

```console
$ docker pull openjdk@sha256:bc0aa2488898f4556041e60f31ba91622f7f31dfe953197b2b295f3c6f926492
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:21-ea-33-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:77aba00e9493f9656b240eea7d32e2d3407c652087b7413de088392f83900823
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.7 MB (268656743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441873c7b8ecff7d7a31d33bf11c05924a4ba84377a373daf4364b36caf61ead`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 07:21:40 GMT
ADD file:733a37449d62d6e9f530185b9244e06cd8ff0ee896632576ae644437d0a1f852 in / 
# Wed, 14 Jun 2023 07:21:40 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 09:56:49 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 09:57:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 14 Jun 2023 09:57:19 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 09:57:19 GMT
ENV LANG=en_US.UTF-8
# Thu, 03 Aug 2023 01:48:41 GMT
ENV JAVA_VERSION=21-ea+33
# Thu, 03 Aug 2023 01:49:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/33/GPL/openjdk-21-ea+33_linux-x64_bin.tar.gz'; 			downloadSha256='c834bec462c77e18a4ba980cc761754649ad34ee40697597ec64306918dedb0b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/33/GPL/openjdk-21-ea+33_linux-aarch64_bin.tar.gz'; 			downloadSha256='41295b248c50ffe8bfa522c0fce7492eabfad5d0fad5c439e7918949066f225a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:49:04 GMT
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
	-	`sha256:9b5e2c00453229ac18071d4036bd1a4c3dc6c81e97a001ee85950cd83503e743`  
		Last Modified: Thu, 03 Aug 2023 01:56:29 GMT  
		Size: 203.9 MB (203929214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
