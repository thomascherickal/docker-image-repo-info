## `openjdk:17-ea-3-oraclelinux8`

```console
$ docker pull openjdk@sha256:58c40381f1e68d1a719d4a9a8a65e7567d9f0c344d8a3e7de9731b5bcea89e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-3-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:c67fb826fa06e3bd063a975550a73fc1e1fc144a9bdac58df166fd1ce41d15aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241226286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9200c75722c732c5bba89e73e725eae9a17565fad6134fe0b43161b587f71950`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 18 Dec 2020 18:20:53 GMT
ADD file:ae640751036e8faf191ef80903201a939fb88b6280ec402d34f100cf54e41b5d in / 
# Fri, 18 Dec 2020 18:20:53 GMT
CMD ["/bin/bash"]
# Fri, 18 Dec 2020 18:38:18 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 18 Dec 2020 18:38:18 GMT
ENV LANG=C.UTF-8
# Mon, 28 Dec 2020 20:20:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Mon, 28 Dec 2020 20:20:56 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 28 Dec 2020 20:20:56 GMT
ENV JAVA_VERSION=17-ea+3
# Mon, 28 Dec 2020 20:21:30 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/3/GPL/openjdk-17-ea+3_linux-aarch64_bin.tar.gz; 			downloadSha256=eacf61fc385681aa56993d5a326acbdb2d40658fb741a7c5b45b002f335262ad; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/3/GPL/openjdk-17-ea+3_linux-x64_bin.tar.gz; 			downloadSha256=fa2562dcc7bf374fc91c01dc722032147ea7553f961a250f8ae7348e6091dabc; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 28 Dec 2020 20:21:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:edcbc9047efe2641ebc4f2393b0e5717733c062c211b0db349abc2ea82364e57`  
		Last Modified: Fri, 18 Dec 2020 18:22:18 GMT  
		Size: 42.1 MB (42059283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096c31e209d76bfb493c22693ffe401d20bd3b9b8bc2256934fda17f29780bb3`  
		Last Modified: Fri, 18 Dec 2020 18:42:59 GMT  
		Size: 13.3 MB (13261719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6226dedf9b1c94569ae99b55c20b92a9e186f79346d3fa823ec9c93875315d7`  
		Last Modified: Mon, 28 Dec 2020 20:26:11 GMT  
		Size: 185.9 MB (185905284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-3-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:14d238a6e8007cfeb491b46d6740694f199d7e0d48e60e5847c5e191b47600b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.3 MB (236312252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a8a02f3be46072741b6bb05a1274b808b8abe07c2993202ade190313ff19bb`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Fri, 18 Dec 2020 18:43:40 GMT
ADD file:be2d17640c58ed7d6ce818b679805972eedbbacd4ab5ae5e15f5c8542d1ff8ea in / 
# Fri, 18 Dec 2020 18:43:43 GMT
CMD ["/bin/bash"]
# Fri, 18 Dec 2020 19:43:59 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 18 Dec 2020 19:43:59 GMT
ENV LANG=C.UTF-8
# Mon, 28 Dec 2020 20:41:35 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Mon, 28 Dec 2020 20:41:36 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 28 Dec 2020 20:41:37 GMT
ENV JAVA_VERSION=17-ea+3
# Mon, 28 Dec 2020 20:42:27 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/3/GPL/openjdk-17-ea+3_linux-aarch64_bin.tar.gz; 			downloadSha256=eacf61fc385681aa56993d5a326acbdb2d40658fb741a7c5b45b002f335262ad; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk17/3/GPL/openjdk-17-ea+3_linux-x64_bin.tar.gz; 			downloadSha256=fa2562dcc7bf374fc91c01dc722032147ea7553f961a250f8ae7348e6091dabc; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 28 Dec 2020 20:42:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:68012513ce8f557e79d400caae7326eb282a43c35afa4fd0a04e0c6470a0c6da`  
		Last Modified: Fri, 18 Dec 2020 18:45:16 GMT  
		Size: 42.0 MB (41984474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19435fd29840d5adb1fcf43416b769187aa10d3f70e390e22cd1edadb7415d63`  
		Last Modified: Fri, 18 Dec 2020 19:51:11 GMT  
		Size: 14.1 MB (14059908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7f133287d0a90db102e197249b7507fc8b68ad4be1c878701867a44031deb2`  
		Last Modified: Mon, 28 Dec 2020 20:48:33 GMT  
		Size: 180.3 MB (180267870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
