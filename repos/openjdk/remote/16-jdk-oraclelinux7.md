## `openjdk:16-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:b78791adead641604d8debdc8ce1643e6831238752dd2c0084a51b99146a516d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:8005ea10f714c83a813fba02edcf69cf60b068d23400e383e2c3afda4570ecf2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248527748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209b97bc25cd123ae43329f896fc910a62f360f0ed50e0bc494691ad68c4c953`
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
# Fri, 18 Dec 2020 04:48:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Fri, 18 Dec 2020 04:48:41 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 20:53:40 GMT
ENV JAVA_VERSION=16-ea+29
# Fri, 18 Dec 2020 20:54:00 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-aarch64_bin.tar.gz; 			downloadSha256=2a273d305f8c5ed1eec0cec322ed37660eddd7bcf1b381583e6c6b66fe020eda; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-x64_bin.tar.gz; 			downloadSha256=484b901cea7c2b6fafea3a4215028f12f225c17807d5413a2d52edcd604ef6ec; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Dec 2020 20:54:00 GMT
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
	-	`sha256:848a569cd713aa30a7d3f64e8780fc496411928316af11cb3754772b05f63fa7`  
		Last Modified: Fri, 18 Dec 2020 20:58:37 GMT  
		Size: 184.8 MB (184839013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:4a23dbc04f49cdbf3543545a68528ea6b47ee4a68e381a50a49f475dc9956fa5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244552876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89ef3570e033a7a195f8b3edd0c2c2759505ecbcbad8a73acecc64cb656c2735`
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
# Thu, 17 Dec 2020 13:37:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 17 Dec 2020 13:37:37 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Dec 2020 19:45:05 GMT
ENV JAVA_VERSION=16-ea+29
# Fri, 18 Dec 2020 19:45:46 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-aarch64_bin.tar.gz; 			downloadSha256=2a273d305f8c5ed1eec0cec322ed37660eddd7bcf1b381583e6c6b66fe020eda; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-x64_bin.tar.gz; 			downloadSha256=484b901cea7c2b6fafea3a4215028f12f225c17807d5413a2d52edcd604ef6ec; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Dec 2020 19:45:48 GMT
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
	-	`sha256:39452dbe210b97742706bff6d8156ef9a9e1e4d63c22d2ae569674b11a7231b1`  
		Last Modified: Fri, 18 Dec 2020 19:52:32 GMT  
		Size: 179.2 MB (179204701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
