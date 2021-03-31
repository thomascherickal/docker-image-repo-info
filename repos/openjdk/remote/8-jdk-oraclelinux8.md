## `openjdk:8-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:d375c272a73652802dba73ae95b3071f171cc676818b000d49bfaee507a3d5f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `openjdk:8-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:616755cc05d33a9c2dda85a0f019c5a95bb275a813dbc3be9cb2e6bbd5765192
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161133953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ddc3185d8e01c07a8afe43b0090c9e30983bc049b6453aa8c811d3cbbe45aca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:01:16 GMT
ADD file:6a8b1c26fdbf2beb390286575735d9efcd8cd6c3d135c9d7d25b3fe4c641a7ee in / 
# Tue, 30 Mar 2021 21:01:16 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:36:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:39:09 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Tue, 30 Mar 2021 21:39:09 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:39:10 GMT
ENV LANG=C.UTF-8
# Tue, 30 Mar 2021 21:39:10 GMT
ENV JAVA_VERSION=8u282
# Tue, 30 Mar 2021 21:39:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u282-b08/OpenJDK8U-jdk_x64_linux_8u282b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:50c2d151af498a24eabbdd1f14042e94106189e17f7858fa9c9e6537816bfa34`  
		Last Modified: Tue, 30 Mar 2021 21:02:23 GMT  
		Size: 42.1 MB (42065616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26bc0351d047f744512b1f8920863854334f02e11637445a710596e8d9aaa7d`  
		Last Modified: Tue, 30 Mar 2021 21:43:00 GMT  
		Size: 13.3 MB (13265630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0c60745e5e9e38c9236da6f1bece8ebfcd4fae148b6a156c82a513f9578b31`  
		Last Modified: Tue, 30 Mar 2021 21:47:27 GMT  
		Size: 105.8 MB (105802707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
