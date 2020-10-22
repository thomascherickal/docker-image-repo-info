## `openjdk:16-ea-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:b3bdb86dc5fbefab226684a6af3a4f13b99c871982c7b054d614ac24c2699eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:5a694c0e085f06ec915f841ebc9d52ecf3fb9665b9be83ae3c35bbeac0dfc7c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.3 MB (264319025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829f2807d9cc9829e53775a5c75c6cc923f5642a7d95a4fb216eaae1bad31c59`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:22:07 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:16:12 GMT
ADD file:dab686af43f04bdaabbdbe7703e0c2dc85868a5dbb38942747055a44e038f37f in / 
# Thu, 22 Oct 2020 02:16:12 GMT
CMD ["/bin/bash"]
# Thu, 22 Oct 2020 02:34:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 22 Oct 2020 02:34:47 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 02:34:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 22 Oct 2020 02:34:48 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 02:34:48 GMT
ENV JAVA_VERSION=16-ea+20
# Thu, 22 Oct 2020 02:35:32 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-aarch64_bin.tar.gz; 			downloadSha256=5226280cbdaec7e5327d77282717f6a5f716f9437194dd3d464059fbdcfbd8be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-x64_bin.tar.gz; 			downloadSha256=98b09726ff551251f988fdd812123a0e33effc5ec3ca45d58ab200f911397fff; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 02:35:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fd3d5e431db632e40b1f1d5ed9a34a906447d43146906e56da1f14f07998bc28`  
		Last Modified: Thu, 22 Oct 2020 02:18:09 GMT  
		Size: 54.2 MB (54161024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004722dc5e0b01dbfaadfde989754299882cd0cd89e7da3f08996ffde63d55e`  
		Last Modified: Thu, 22 Oct 2020 02:44:53 GMT  
		Size: 13.5 MB (13493854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1f643e88ad25e2aae7856fcb9ed525ece7d6e7ffde6f832f17d4f3d176d683`  
		Last Modified: Thu, 22 Oct 2020 02:45:12 GMT  
		Size: 196.7 MB (196664147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7cddd6cb45d29469389ee967c54366507e9f8d23bf997c4d984a2e55e0a6a3d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246201830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1437530785f1eec92d657a5f4d454b082af0fc9c3c3b2582136cf77effa96e9a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:40:54 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/8-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 8 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 22 Oct 2020 02:02:57 GMT
ADD file:91f94052d144e7fac61501c6d72e663eda67c40303d29f0b62fda4abe0e5a284 in / 
# Thu, 22 Oct 2020 02:03:00 GMT
CMD ["/bin/bash"]
# Thu, 22 Oct 2020 09:16:39 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 22 Oct 2020 09:16:41 GMT
ENV LANG=C.UTF-8
# Thu, 22 Oct 2020 09:16:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 22 Oct 2020 09:16:42 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Oct 2020 22:45:37 GMT
ENV JAVA_VERSION=16-ea+21
# Thu, 22 Oct 2020 22:46:34 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-aarch64_bin.tar.gz; 			downloadSha256=bee09458526a8c10a40f3d4e5bf6c384b1bbc6f9002997d2f4c0d8c090cca1f8; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/21/GPL/openjdk-16-ea+21_linux-x64_bin.tar.gz; 			downloadSha256=3294d805c6125a6dd55a387f82f74df0c9fc0bce06934061fb3ff2dd42075b33; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 22 Oct 2020 22:46:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:428aa11a26cf7698a25c3ec8f290dd1667191a70a5797b7232fa597f1e52ec1b`  
		Last Modified: Thu, 22 Oct 2020 02:04:59 GMT  
		Size: 54.3 MB (54285957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e761c4ae4b3b9dbb16537c08ceb4e5ad0d91323e105a8b241ae8c7538fa70b1f`  
		Last Modified: Thu, 22 Oct 2020 09:24:38 GMT  
		Size: 14.4 MB (14381453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179bc4e532061314a92eae26ee461a1638f9c817713e3e649451d0028402ea6f`  
		Last Modified: Thu, 22 Oct 2020 22:55:31 GMT  
		Size: 177.5 MB (177534420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
