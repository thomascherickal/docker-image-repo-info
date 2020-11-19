## `openjdk:16-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:3a3e5582dccda81a01d5f10fd959f7ed7ff0e21d30d03659540e21a41f3bfd3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:1c4c32291b1017a78ac938f3d46855a9b0db68222c126f818fdf4b8934132e24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.2 MB (247232909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985b224b9b644686822c97a17ceffd739e407782120b5e3df0be18e027e6d25f`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Wed, 18 Nov 2020 18:16:17 GMT
ADD file:fbc16b85088aeb16b00035f95c6e08678b18cb8a31a4034a171a84b878f95cae in / 
# Wed, 18 Nov 2020 18:16:17 GMT
CMD ["/bin/bash"]
# Thu, 19 Nov 2020 03:03:35 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 19 Nov 2020 03:03:35 GMT
ENV LANG=en_US.UTF-8
# Thu, 19 Nov 2020 03:03:35 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 19 Nov 2020 03:03:35 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 19 Nov 2020 03:03:35 GMT
ENV JAVA_VERSION=16-ea+24
# Thu, 19 Nov 2020 03:04:17 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/24/GPL/openjdk-16-ea+24_linux-aarch64_bin.tar.gz; 			downloadSha256=9085bbb4f9e4d70ac385f85fbd706ab1fa570417beb28d09ff71e4908684cd8c; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/24/GPL/openjdk-16-ea+24_linux-x64_bin.tar.gz; 			downloadSha256=ad1e33e43f923a8cde6e611e8ada1b76047f156d44b981d16daa440251f71823; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 19 Nov 2020 03:04:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:245e9951308ef864ce941f4383344a273da57264b763e6f5aba9347211cf7a40`  
		Last Modified: Wed, 18 Nov 2020 18:17:21 GMT  
		Size: 48.3 MB (48257477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad539b15199b16ffde2cf3133150c11af2d0a098c5344f38a10e4760a36cae02`  
		Last Modified: Thu, 19 Nov 2020 03:09:11 GMT  
		Size: 15.4 MB (15430776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0512c9b2a4728ed7a9b522c2c8d306ef1c86c09b55eaf325a60b6bb8fb7f29`  
		Last Modified: Thu, 19 Nov 2020 03:09:31 GMT  
		Size: 183.5 MB (183544656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c74bcd724be755be8ba9b8846f051a42c8276c802983d3e56a99f7664212d2f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.4 MB (243358335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fedb143a6d1e76ff5402081670b9c8f19d22fc908fa124561533e5cd8c2fd1`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Wed, 18 Nov 2020 21:39:27 GMT
ADD file:f4a327657a328a670e79dc5abbe14d34c0f6083bc105b04205bb7b6007009f5c in / 
# Wed, 18 Nov 2020 21:39:30 GMT
CMD ["/bin/bash"]
# Wed, 18 Nov 2020 22:29:47 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 18 Nov 2020 22:29:48 GMT
ENV LANG=en_US.UTF-8
# Wed, 18 Nov 2020 22:29:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 18 Nov 2020 22:29:50 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 22:29:51 GMT
ENV JAVA_VERSION=16-ea+24
# Wed, 18 Nov 2020 22:30:29 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/24/GPL/openjdk-16-ea+24_linux-aarch64_bin.tar.gz; 			downloadSha256=9085bbb4f9e4d70ac385f85fbd706ab1fa570417beb28d09ff71e4908684cd8c; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/24/GPL/openjdk-16-ea+24_linux-x64_bin.tar.gz; 			downloadSha256=ad1e33e43f923a8cde6e611e8ada1b76047f156d44b981d16daa440251f71823; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 Nov 2020 22:30:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:436adcdab5ec3071ba37753f4a768eb644a6d3b209b6c68878fbd4ff8f133edd`  
		Last Modified: Wed, 18 Nov 2020 21:40:29 GMT  
		Size: 48.9 MB (48865849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63ac2a3436373a229835a88787a306790127dbf63f5fe9ba4a0745aae062aeb`  
		Last Modified: Wed, 18 Nov 2020 22:34:42 GMT  
		Size: 16.5 MB (16482372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1d6b21b271682635451298d24aace971e8e6d9ac88dde40048c9dc0db12611`  
		Last Modified: Wed, 18 Nov 2020 22:35:03 GMT  
		Size: 178.0 MB (178010114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
