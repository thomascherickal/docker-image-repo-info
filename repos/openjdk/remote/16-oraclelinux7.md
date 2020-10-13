## `openjdk:16-oraclelinux7`

```console
$ docker pull openjdk@sha256:0077171a9993c3d9152460065d82db2607848951b5eb513b1399718fca434798
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:772248d3b9cdb1133e135862b9c9d8bd384de0196141e7e3249a9598cc12f251
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.0 MB (261023437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e2d7496225a4f7b8e877348c11f5485b8507e0ff6542c247504dd7d23616ec0`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 13 Oct 2020 00:23:46 GMT
ADD file:793c5c6e19fd582be4d448e8112d88c35da538f04ccdae7f6c452d84c8340aad in / 
# Tue, 13 Oct 2020 00:23:46 GMT
CMD ["/bin/bash"]
# Tue, 13 Oct 2020 00:41:15 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 13 Oct 2020 00:41:16 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Oct 2020 00:41:16 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 13 Oct 2020 00:41:16 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 00:41:16 GMT
ENV JAVA_VERSION=16-ea+19
# Tue, 13 Oct 2020 00:42:07 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-aarch64_bin.tar.gz; 			downloadSha256=9e7094e0dcba61b6b8111f48934cb7395e6dafb1d1ddea7d2296cb0872d67d66; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-x64_bin.tar.gz; 			downloadSha256=487e44f1ec92106437a96f8af07a83ac314dee51dfd46838c23657e550bc616f; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 00:42:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:41152c08460e17bb4938ae7b3513375500def33918c0c58e738ba74f2e1f4eed`  
		Last Modified: Tue, 13 Oct 2020 00:25:19 GMT  
		Size: 48.2 MB (48244505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8adb1e46ec2e9c9ae083596afff6a1fd30fdb8c1878d8a25641a4aa79f5dd0`  
		Last Modified: Tue, 13 Oct 2020 00:46:35 GMT  
		Size: 16.2 MB (16231515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822e4a30fffefd51514b67e3c733f9906dfda4a91753675acf945865f80c28bf`  
		Last Modified: Tue, 13 Oct 2020 00:46:49 GMT  
		Size: 196.5 MB (196547417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:5c9583e1e2277530e377ec8fc4f46b235a20e145e9b4d67482eff4eaa85d39cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.6 MB (240564628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09242e2deedd6c9d5ec6e93fd0d516950cd9dcb3769d928982c4ab943f2ae954`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 13 Oct 2020 00:01:23 GMT
ADD file:3901ded436783e2bee5efa520251623b82144ffef13ece54748f9d262eff841f in / 
# Tue, 13 Oct 2020 00:01:29 GMT
CMD ["/bin/bash"]
# Tue, 13 Oct 2020 00:19:37 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 13 Oct 2020 00:19:38 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Oct 2020 00:19:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 13 Oct 2020 00:19:39 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 00:19:40 GMT
ENV JAVA_VERSION=16-ea+19
# Tue, 13 Oct 2020 00:20:24 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-aarch64_bin.tar.gz; 			downloadSha256=9e7094e0dcba61b6b8111f48934cb7395e6dafb1d1ddea7d2296cb0872d67d66; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/19/GPL/openjdk-16-ea+19_linux-x64_bin.tar.gz; 			downloadSha256=487e44f1ec92106437a96f8af07a83ac314dee51dfd46838c23657e550bc616f; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 00:20:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:976db0add784ec3dc16e6f09c92eec05cef273da83204e7ea624a14d6db66547`  
		Last Modified: Tue, 13 Oct 2020 00:03:00 GMT  
		Size: 48.8 MB (48848065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0f875096760c96a1d20b41bf35d8ae70cd277fd4947e158d30829af7203218`  
		Last Modified: Tue, 13 Oct 2020 00:23:20 GMT  
		Size: 16.4 MB (16449031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f3f4b29ca80b857a19951257361344ab5ae91732c727261062215a7020f0`  
		Last Modified: Tue, 13 Oct 2020 00:23:43 GMT  
		Size: 175.3 MB (175267532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
