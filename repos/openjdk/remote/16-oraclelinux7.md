## `openjdk:16-oraclelinux7`

```console
$ docker pull openjdk@sha256:60dd475d6920cb5ed8993aadd3a62ae39f56f10fb68e95e707e23467b7e72e64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:6d60084a941e286d5dcbbff19f0ba010700a0094c0a1e07fe21151ed78d08ae3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.5 MB (248529016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa0407097e64eec31a3213e40c57325090ce6d7de737a35a165ce6316689ced2`
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
# Fri, 18 Dec 2020 04:48:41 GMT
ENV JAVA_VERSION=16-ea+28
# Fri, 18 Dec 2020 04:49:33 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/28/GPL/openjdk-16-ea+28_linux-aarch64_bin.tar.gz; 			downloadSha256=ec5240a695751612960e7459476c6081e69a03aebe4ff3c7ae964b9235dfe9a4; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/28/GPL/openjdk-16-ea+28_linux-x64_bin.tar.gz; 			downloadSha256=2c2f2136a72e53deedef4e4e35d3d34315093a16732b9d112297e11e0661ea05; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Dec 2020 04:49:33 GMT
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
	-	`sha256:296e7dbd8b3b1d9596c0c43e8c2cfdfd05dab956d0eaecd83a9078a9c1f2e743`  
		Last Modified: Fri, 18 Dec 2020 04:55:04 GMT  
		Size: 184.8 MB (184840281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:7cd8b62b3000061453912a755c9e3b6a6c62efa02ef19508175dd8ab40262b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.5 MB (244547230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3285f921d5d9e0b6a5f5e14358e1a9186ba4023e0ab9ca3c6f539b2be6cbb06`
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
# Thu, 17 Dec 2020 13:37:38 GMT
ENV JAVA_VERSION=16-ea+28
# Thu, 17 Dec 2020 13:38:22 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/28/GPL/openjdk-16-ea+28_linux-aarch64_bin.tar.gz; 			downloadSha256=ec5240a695751612960e7459476c6081e69a03aebe4ff3c7ae964b9235dfe9a4; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/28/GPL/openjdk-16-ea+28_linux-x64_bin.tar.gz; 			downloadSha256=2c2f2136a72e53deedef4e4e35d3d34315093a16732b9d112297e11e0661ea05; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 17 Dec 2020 13:38:23 GMT
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
	-	`sha256:7e6dc467ac27faf5eb21edde7cb12fe90f554504d2a7bc8828cb62d4d379a14b`  
		Last Modified: Thu, 17 Dec 2020 13:46:12 GMT  
		Size: 179.2 MB (179199055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
