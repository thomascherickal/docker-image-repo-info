## `openjdk:22-ea-8-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:939a16bef946365e348d0da3af9eb42736191d3e15ead27b75163fbcd265ba43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `openjdk:22-ea-8-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:7737e14fb66f4e91ce6e04c0b7290125b7f10ee375b12f77cb2ed24d1693f5f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.7 MB (264700228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3b4cb37f2de1dc2b561722eebdf21cb328dd328201b8fa0965865ab84289a50`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 22 Jul 2023 01:20:32 GMT
ADD file:6d43f7bf7c8d8c056e6fcc566ccfa2c1e42be1ef095f94d6780d0ca7d9a02e6e in / 
# Sat, 22 Jul 2023 01:20:32 GMT
CMD ["/bin/bash"]
# Sat, 22 Jul 2023 01:40:55 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Sat, 22 Jul 2023 01:40:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Sat, 22 Jul 2023 01:40:55 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 22 Jul 2023 01:40:55 GMT
ENV LANG=C.UTF-8
# Thu, 03 Aug 2023 01:45:13 GMT
ENV JAVA_VERSION=22-ea+8
# Thu, 03 Aug 2023 01:45:36 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='f05e7933726ce10c3789634d099fdf1b3e61ae9d633aae85fa22ed92ed0a8bac'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/8/GPL/openjdk-22-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='ee073fed6cbf145e5e3a06384d3e8f99ee22179cbb4049e1af2dc01275290900'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 03 Aug 2023 01:45:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:49bb46380f8cb3491e82d000b27a6eb26b2490291da814ce3363bbf2c8baeb1a`  
		Last Modified: Sat, 22 Jul 2023 01:21:47 GMT  
		Size: 44.9 MB (44915006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938c78e257f8d32905a5685feaf98c164b8091b3f15fb7705c4181bd3998b783`  
		Last Modified: Sat, 22 Jul 2023 01:42:50 GMT  
		Size: 15.0 MB (15009045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b4a6d05a7ad77fac9ee4c6479513440bd6586faa4c877c3a730c509201fa3c`  
		Last Modified: Thu, 03 Aug 2023 01:52:14 GMT  
		Size: 204.8 MB (204776177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
