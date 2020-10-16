## `openjdk:16-ea-20-oraclelinux7`

```console
$ docker pull openjdk@sha256:ed1d6a275f011c315f8b03fefd789e3e4f88e109287e8ed6243623de77008a7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-20-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:f279c52ee1ed291aa5d7d23da461fc9acca419f1ff9c32d1ed7fe07292ea7d13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261139897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bede66c6abc3da9ab34c1e69ee524509103ad2cdcf6b473568dee9e583232ce`
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
# Fri, 16 Oct 2020 20:32:04 GMT
ENV JAVA_VERSION=16-ea+20
# Fri, 16 Oct 2020 20:32:18 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-aarch64_bin.tar.gz; 			downloadSha256=5226280cbdaec7e5327d77282717f6a5f716f9437194dd3d464059fbdcfbd8be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-x64_bin.tar.gz; 			downloadSha256=98b09726ff551251f988fdd812123a0e33effc5ec3ca45d58ab200f911397fff; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Oct 2020 20:32:18 GMT
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
	-	`sha256:fa9ee49503fe3607e728d7fcb1cdb26b02b9eb819fcdf2e1eb31e0fba66cefaf`  
		Last Modified: Fri, 16 Oct 2020 20:37:07 GMT  
		Size: 196.7 MB (196663877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-20-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:29f156563f2d1d15aa55b1eff87ad4fa03ddd7a6d478e025ce3315e69250b9ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.6 MB (240649990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e4c229cb1094762bb55c2bb699e390726bd7df26e29b3ee82095f1aa6894f91`
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
# Fri, 16 Oct 2020 21:23:01 GMT
ENV JAVA_VERSION=16-ea+20
# Fri, 16 Oct 2020 21:23:30 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-aarch64_bin.tar.gz; 			downloadSha256=5226280cbdaec7e5327d77282717f6a5f716f9437194dd3d464059fbdcfbd8be; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/20/GPL/openjdk-16-ea+20_linux-x64_bin.tar.gz; 			downloadSha256=98b09726ff551251f988fdd812123a0e33effc5ec3ca45d58ab200f911397fff; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Oct 2020 21:23:32 GMT
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
	-	`sha256:d4f311f587ce105fb4fa819024895dd474e32e9ba3b1ba37ed19350f0c26f206`  
		Last Modified: Fri, 16 Oct 2020 21:28:10 GMT  
		Size: 175.4 MB (175352894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
