## `openjdk:18-ea-25-oraclelinux7`

```console
$ docker pull openjdk@sha256:1318a44eef5bd312daaae3030ad195fb4d98fd5a9d75392df88723e7ee77a4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `openjdk:18-ea-25-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b7bf32aa085096c5c57a18f4fbb1e48deb214b857ae6582b55c50fe477ffcc58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252868001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6209f8280056eac3097899b56e2f57bde857ff41f0a4640ed406010ab12d258`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Nov 2021 22:01:36 GMT
ADD file:718e42489681d6e9446ec4bb10ba8e24c85d645eb9a303e587f767bedcf668d1 in / 
# Wed, 24 Nov 2021 22:01:37 GMT
CMD ["/bin/bash"]
# Wed, 24 Nov 2021 23:34:39 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Nov 2021 23:34:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 24 Nov 2021 23:34:40 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 23:34:41 GMT
ENV LANG=en_US.UTF-8
# Tue, 30 Nov 2021 04:08:05 GMT
ENV JAVA_VERSION=18-ea+25
# Tue, 30 Nov 2021 04:08:22 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/25/GPL/openjdk-18-ea+25_linux-x64_bin.tar.gz'; 			downloadSha256='74a01fc91a33136b6a5d387ecdfc2790ef5e351e3bef869706b288bc9a1df6a2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/25/GPL/openjdk-18-ea+25_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6f03a12f2c2228a46544ba43b73cd40e4bbb7b5ef857445641d64391d04798c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Nov 2021 04:08:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:53ff3b63a7657067cd7642c8106127a05a5ea45e3b68cbf830d4120a127e9c82`  
		Last Modified: Wed, 24 Nov 2021 22:02:31 GMT  
		Size: 48.9 MB (48907823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef6b8fb533810fdc95b689d95dd39d5a3f59cb3d3147fddf5bbdf7df183774b`  
		Last Modified: Wed, 24 Nov 2021 23:46:39 GMT  
		Size: 16.5 MB (16464628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3c88ae867632b7ef754897dc08d6b78eacaee4b24059fcc1ac1f4d69d868b4`  
		Last Modified: Tue, 30 Nov 2021 04:20:25 GMT  
		Size: 187.5 MB (187495550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
