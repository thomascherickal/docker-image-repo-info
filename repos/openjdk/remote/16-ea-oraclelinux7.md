## `openjdk:16-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:5527bec12a4d536726d42a59dba05d6813d1e36465c7878e1d6d01b6d0879df7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:f3407a33ac63a824fefe1380b9ed2f713dfaf319a39fe72f921190ec664822ac
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248525066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4ce6d543c9848dfd24e6862d2977f6138c135d4f46f485b73ab7255d94a4205`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 21:23:41 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-amd64/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 22 Dec 2020 17:21:03 GMT
ADD file:427e3de4e281b54b6b3ecbe5e05d7fc4433263f8261c48987f7ded117fc1be97 in / 
# Tue, 22 Dec 2020 17:21:04 GMT
CMD ["/bin/bash"]
# Tue, 22 Dec 2020 17:38:18 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 22 Dec 2020 17:38:18 GMT
ENV LANG=en_US.UTF-8
# Tue, 22 Dec 2020 17:38:18 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 22 Dec 2020 17:38:18 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Dec 2020 17:38:19 GMT
ENV JAVA_VERSION=16-ea+29
# Tue, 22 Dec 2020 17:38:33 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-aarch64_bin.tar.gz; 			downloadSha256=2a273d305f8c5ed1eec0cec322ed37660eddd7bcf1b381583e6c6b66fe020eda; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-x64_bin.tar.gz; 			downloadSha256=484b901cea7c2b6fafea3a4215028f12f225c17807d5413a2d52edcd604ef6ec; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Dec 2020 17:38:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1184447a0a941bd8539b65a1b6a5af90677e55e49e45cc7eee6cac4f123bff94`  
		Last Modified: Tue, 22 Dec 2020 17:22:22 GMT  
		Size: 48.3 MB (48256777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0e5ad4c6cf695a5cf68ff112562da71423d525c8f7f0075a634bea8ea4ac47`  
		Last Modified: Tue, 22 Dec 2020 17:42:38 GMT  
		Size: 15.4 MB (15429206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8ece1354473dba708790ecebaccf68c323ca941befd14b213d28739cc84ebf`  
		Last Modified: Tue, 22 Dec 2020 17:42:51 GMT  
		Size: 184.8 MB (184839083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b199b621e072e47828408055b27664c2f13b935abe5a1ea2c2c8a4dd08013273
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244554309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fcfc368c5a290fc5ecf3016659676c84eb574dc129f735c18accde9544e3463`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Sep 2020 20:41:36 GMT
LABEL org.opencontainers.image.authors=Oracle Linux Product Team <ol-ovm-info_ww@oracle.com> org.opencontainers.image.url=https://github.com/oracle/container-images org.opencontainers.image.source=https://github.com/oracle/container-images/tree/dist-arm64v8/7-slim org.opencontainers.image.vendor=Oracle America, Inc org.opencontainers.image.title=Oracle Linux 7 (slim) org.opencontainers.image.description=Oracle Linux is an open-source       operating system available under the GNU General Public License (GPLv2) and       is suitable for both general purpose or Oracle workloads.
# Tue, 22 Dec 2020 17:40:57 GMT
ADD file:ec95b4619b5e5fc03a6ad9b5ae466fc891abf449e7dbde03283ce3a9885f238e in / 
# Tue, 22 Dec 2020 17:41:01 GMT
CMD ["/bin/bash"]
# Tue, 22 Dec 2020 17:58:47 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 22 Dec 2020 17:58:48 GMT
ENV LANG=en_US.UTF-8
# Tue, 22 Dec 2020 17:58:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Tue, 22 Dec 2020 17:58:49 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Dec 2020 17:58:50 GMT
ENV JAVA_VERSION=16-ea+29
# Tue, 22 Dec 2020 17:59:40 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-aarch64_bin.tar.gz; 			downloadSha256=2a273d305f8c5ed1eec0cec322ed37660eddd7bcf1b381583e6c6b66fe020eda; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/29/GPL/openjdk-16-ea+29_linux-x64_bin.tar.gz; 			downloadSha256=484b901cea7c2b6fafea3a4215028f12f225c17807d5413a2d52edcd604ef6ec; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 22 Dec 2020 17:59:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2fa5b4561d489d4ba037541bc1400de45a1aad2d6e7197b8bfa0999af4c62266`  
		Last Modified: Tue, 22 Dec 2020 17:42:05 GMT  
		Size: 48.9 MB (48867329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f4fbf760ea337587e3374187a1443f6bf6d20437e76dcacf8de2747a34e1a2`  
		Last Modified: Tue, 22 Dec 2020 18:04:33 GMT  
		Size: 16.5 MB (16482482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e1d4de842a360b5174b39bf87b36921e1caa64dcaa5570373707290124c8ed`  
		Last Modified: Tue, 22 Dec 2020 18:04:55 GMT  
		Size: 179.2 MB (179204498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
