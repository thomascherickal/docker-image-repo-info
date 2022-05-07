## `openjdk:19-ea-21-jdk`

```console
$ docker pull openjdk@sha256:9268f80cbc6ec1b4bc6f3381374e77e7121708736b410a9fd045123dfce8509d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:19-ea-21-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:10bf85d8c48b27df5b6b5cdf42541693ab3c1d3afc7fbd0a9d18f6b22ed17166
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249920400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c1e038eb13274946dea3106c1453830917d1157911280cbbdebdf4cf2c805c5`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 02 May 2022 21:46:34 GMT
ADD file:e59d0ab85f777209561c628874489b9544223a23fed0755bedd408a55452b4af in / 
# Mon, 02 May 2022 21:46:35 GMT
CMD ["/bin/bash"]
# Mon, 02 May 2022 22:06:20 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 02 May 2022 22:06:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Mon, 02 May 2022 22:06:22 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 02 May 2022 22:06:23 GMT
ENV LANG=C.UTF-8
# Sat, 07 May 2022 00:46:27 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 00:46:41 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 07 May 2022 00:46:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2d35f3f87cf615a8684aa1b866b03a7078bce1beea91489effc1e6c03c83124c`  
		Last Modified: Mon, 02 May 2022 21:47:34 GMT  
		Size: 42.0 MB (42016620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e242efb2259690773e11adafa3652b3b5f5ac58742dfba66216c5527ec988`  
		Last Modified: Mon, 02 May 2022 22:17:46 GMT  
		Size: 14.3 MB (14292260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a247b11036a9396dc02dcc5e53df822012cccd7835b9037ca82061c052ecab4c`  
		Last Modified: Sat, 07 May 2022 00:58:52 GMT  
		Size: 193.6 MB (193611520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
