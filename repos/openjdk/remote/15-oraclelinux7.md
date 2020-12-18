## `openjdk:15-oraclelinux7`

```console
$ docker pull openjdk@sha256:7cd2df3f1641c5af0dee8c751024b18a343093487c4d605a76f4fed59fe23bc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:0db08b708d3256cae3b9083e75dc9e9b14001782818a260751b14550e65e51c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.5 MB (259468206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb02bd4bf15fadfc32e249dd747a18ccb7b8afb9435bbcd129a8f676740cc4e`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 17 Dec 2020 17:36:01 GMT
ADD file:86d6ee7b986b86b9aa79210fd979dc5e350e434afc9b6897d52373bf8e99a3b1 in / 
# Thu, 17 Dec 2020 17:36:01 GMT
CMD ["/bin/bash"]
# Fri, 18 Dec 2020 04:48:41 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 18 Dec 2020 04:48:41 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Dec 2020 04:50:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 18 Dec 2020 04:50:31 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 04:50:31 GMT
ENV JAVA_VERSION=15.0.1
# Fri, 18 Dec 2020 04:50:43 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-aarch64_bin.tar.gz; 			downloadSha256=6a62b7ec065280bad978a3322733a089153dec5ebf5ba81fd2fa361382dbc7b0; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-x64_bin.tar.gz; 			downloadSha256=83ec3a7b1649a6b31e021cde1e58ab447b07fb8173489f27f427e731c89ed84a; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Dec 2020 04:50:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:aaf2c1f8a217b022b582b2fa29293a3e7bc90ade4849a2254c2a44eb2391396a`  
		Last Modified: Thu, 17 Dec 2020 17:37:11 GMT  
		Size: 48.3 MB (48257819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38912b320a7c43adfba3c23ef95458e4c4115aaab9fa9f6b4a89f4b6ce1125c6`  
		Last Modified: Fri, 18 Dec 2020 04:54:48 GMT  
		Size: 15.4 MB (15430916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d53084b0ad270c2755865ab0c7a9de274e4bfba6a9d3748fc02f9b49d9631a8a`  
		Last Modified: Fri, 18 Dec 2020 04:56:15 GMT  
		Size: 195.8 MB (195779471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:989f893f4a74c249b571085cacc6b7b0606aa835c5a43fb83bc73ce6d851c313
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240235134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408a82f164c8bb7038f1cda3d48f14d1512e33c83902bd54ce1d63c0945a7150`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Thu, 17 Dec 2020 10:54:39 GMT
ADD file:234e637b79d352a87884f78cc7eef7b15ada4bb4afd2ce527325eb690092902f in / 
# Thu, 17 Dec 2020 10:54:44 GMT
CMD ["/bin/bash"]
# Thu, 17 Dec 2020 13:37:35 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Dec 2020 13:37:36 GMT
ENV LANG=en_US.UTF-8
# Thu, 17 Dec 2020 13:39:40 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Thu, 17 Dec 2020 13:39:41 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Dec 2020 13:39:41 GMT
ENV JAVA_VERSION=15.0.1
# Thu, 17 Dec 2020 13:40:30 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-aarch64_bin.tar.gz; 			downloadSha256=6a62b7ec065280bad978a3322733a089153dec5ebf5ba81fd2fa361382dbc7b0; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15.0.1/51f4f36ad4ef43e39d0dfdbaf6549e32/9/GPL/openjdk-15.0.1_linux-x64_bin.tar.gz; 			downloadSha256=83ec3a7b1649a6b31e021cde1e58ab447b07fb8173489f27f427e731c89ed84a; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Dec 2020 13:40:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0c52f25eeb980aa519afffa967e1c689524d7fde7d50fc33420a3d54daed23da`  
		Last Modified: Thu, 17 Dec 2020 10:55:54 GMT  
		Size: 48.9 MB (48865698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e1a0b9099b484560144815390977bc89f52d6d5485e1ed1306403e8c868e55`  
		Last Modified: Thu, 17 Dec 2020 13:45:44 GMT  
		Size: 16.5 MB (16482477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf381d9de485765be5cf08a13987ec8050745c62da2f83cb47e0d6a7e337e776`  
		Last Modified: Thu, 17 Dec 2020 13:47:50 GMT  
		Size: 174.9 MB (174886959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
