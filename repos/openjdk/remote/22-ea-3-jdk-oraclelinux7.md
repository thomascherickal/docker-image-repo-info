## `openjdk:22-ea-3-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:722d5be5fa2df9f9c54616cb07cdf08e40d281617c7e418545f9a56401100e72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-3-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:8dd176b68a97fa97e8338e156e23705846395703f83b421709ac73875cce5a21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.4 MB (269364080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3764014f6fee848fde611ceace0f907327036f274b8876d575854bc9671153`
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
# Fri, 23 Jun 2023 00:26:01 GMT
ENV JAVA_VERSION=22-ea+3
# Fri, 23 Jun 2023 00:26:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='6541c5f5f08ec100af327c36768e302185851f548f6c33d1fe26250133998d5a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/3/GPL/openjdk-22-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='e94529988d1c61d552981cc44896e13a1c49f3720567b2a92ad103f24291a167'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 23 Jun 2023 00:26:12 GMT
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
	-	`sha256:9b8118d1461016b21ac204ab62413ee4fd414ba84f05e01461ada98dd26f34f7`  
		Last Modified: Fri, 23 Jun 2023 00:30:48 GMT  
		Size: 204.6 MB (204636551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
