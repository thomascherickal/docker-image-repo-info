## `openjdk:15-oraclelinux7`

```console
$ docker pull openjdk@sha256:25f7a0f58c1614079a3776823d5332301f21945c5e4ea765281b76e810d1ecf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:4a06c6d614a597840c709c6be5873fed3c991bddb3c5942f490d1e81371aadc4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.2 MB (260228091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a39fa0e9b620fa2397bd1e560b253e34f542ad463ae73ae2f402a7011a832055`
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
# Tue, 13 Oct 2020 00:42:41 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Tue, 13 Oct 2020 00:42:41 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 00:42:42 GMT
ENV JAVA_VERSION=15
# Tue, 13 Oct 2020 00:43:20 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 00:43:20 GMT
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
	-	`sha256:4ce6683a30bbdd92223d232befdd72e2be8fd017bce8bc6326885687216b052e`  
		Last Modified: Tue, 13 Oct 2020 00:47:18 GMT  
		Size: 195.8 MB (195752071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:8d1ac0794dd30815078b677381680a3fed7c68302bb12cefc1d4e32aa2706bc9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240153976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72d7bf7aea0ef2f05b2652eb1f2ee314d9bbaeeddf7c872b12e86b93b18e045b`
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
# Tue, 13 Oct 2020 00:20:50 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Tue, 13 Oct 2020 00:20:51 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 00:20:52 GMT
ENV JAVA_VERSION=15
# Tue, 13 Oct 2020 00:21:30 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Oct 2020 00:21:32 GMT
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
	-	`sha256:acea287cdb80add54e24fae4b23c8cbe5b5cb39535d7678fff57c6cded251b99`  
		Last Modified: Tue, 13 Oct 2020 00:24:38 GMT  
		Size: 174.9 MB (174856880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
