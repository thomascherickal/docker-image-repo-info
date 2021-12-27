## `openjdk:19-ea-3-jdk-oracle`

```console
$ docker pull openjdk@sha256:80c6f0b34bcef02cbaaa6d6b8605f42b841e790f02a483502d92fbf5a14aa67b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-3-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:c43c0594dec8e784983b3fc89c55c27a9ea00d4004e6a998e688e2fa7147336f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.1 MB (245130247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3caa55b7e93745097d317867be2529822b0f9b02914738e04aefc82065e91783`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Dec 2021 02:20:57 GMT
ADD file:15b307e0b1aafead42c103e34d3e51a271acea1ab0b68961e239f11af3b0d179 in / 
# Thu, 23 Dec 2021 02:20:57 GMT
CMD ["/bin/bash"]
# Thu, 23 Dec 2021 02:37:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Dec 2021 02:37:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 23 Dec 2021 02:37:55 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Dec 2021 02:37:55 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 18:51:34 GMT
ENV JAVA_VERSION=19-ea+3
# Mon, 27 Dec 2021 18:51:46 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='30e778f7957c2a472df602c7daf108b4cc7994815c5d57bb33a90b55c70e85ca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='b984d67b32bfc13899f25f728f8c8184aac8f9e15f35d6db1f285a714eeb0234'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Dec 2021 18:51:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:155aced2666332ddff5a741b0236f360820e7aa3fc3dde2224fc17a91fc48db6`  
		Last Modified: Thu, 23 Dec 2021 02:21:56 GMT  
		Size: 42.1 MB (42105152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5901c58ecb29b61159b5e3a63dfbb0fb520b2de1d33c9fb038d9b697e3fcd4`  
		Last Modified: Thu, 23 Dec 2021 02:45:32 GMT  
		Size: 13.5 MB (13520734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa379cddc5a283ec05e4430a1895d435f882bb4c949d245d3bb0728f4835301f`  
		Last Modified: Mon, 27 Dec 2021 19:00:33 GMT  
		Size: 189.5 MB (189504361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-3-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7ee3575a8db06c80370f58ef4f873b33a482e20e7a8f405d1b5d469cf96a8460
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.8 MB (244752356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30529ddb97b20c011fbe1a4518ea00c984c0be5f6d34c9f0187d7996073a155`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Dec 2021 02:40:45 GMT
ADD file:140d632303428d802f77f473aef33fa52daacdfc76b23edde4344be661c1d4b0 in / 
# Thu, 23 Dec 2021 02:40:46 GMT
CMD ["/bin/bash"]
# Thu, 23 Dec 2021 02:58:38 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 27 Dec 2021 17:43:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Mon, 27 Dec 2021 17:43:39 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Dec 2021 17:43:40 GMT
ENV LANG=C.UTF-8
# Mon, 27 Dec 2021 17:43:41 GMT
ENV JAVA_VERSION=19-ea+3
# Mon, 27 Dec 2021 17:43:54 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='30e778f7957c2a472df602c7daf108b4cc7994815c5d57bb33a90b55c70e85ca'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/3/GPL/openjdk-19-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='b984d67b32bfc13899f25f728f8c8184aac8f9e15f35d6db1f285a714eeb0234'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 27 Dec 2021 17:43:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:53f096d4aa0757c30613f325df1e03a90db9d9879ea251b394e3ab0a068b5610`  
		Last Modified: Thu, 23 Dec 2021 02:41:44 GMT  
		Size: 42.0 MB (42018351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921862a08fd8bc652539d62804daf06ab6464bd5b42061f5bedbdfa73bd62136`  
		Last Modified: Thu, 23 Dec 2021 03:11:46 GMT  
		Size: 14.3 MB (14303905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a545a8621767b845e56cc4728ce687d4b37020f940fd8db5b1c12ab9e1f63046`  
		Last Modified: Mon, 27 Dec 2021 17:59:33 GMT  
		Size: 188.4 MB (188430100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
