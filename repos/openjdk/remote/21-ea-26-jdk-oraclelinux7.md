## `openjdk:21-ea-26-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:ef4ef10f85e9a46cc93705e5558133e81a2d9029d6676185e0c5cc1d7ce42ce0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-26-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:33d6e538b48cd3cda87d5f3f20b3d9bdd0171163740eba8eacb0c8a82127c11f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268568609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ce39f3a4d384df71d818912902ba404785c3bd6cfe29b4028406f7c7409f3b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 Mar 2023 22:29:01 GMT
ADD file:a14b5a8b8b6993aeee5ac6052fdf283560d65365e5bcf133ab21c4756439384a in / 
# Fri, 31 Mar 2023 22:29:01 GMT
CMD ["/bin/bash"]
# Fri, 31 Mar 2023 23:12:41 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 31 Mar 2023 23:12:42 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Fri, 31 Mar 2023 23:12:42 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 31 Mar 2023 23:12:42 GMT
ENV LANG=en_US.UTF-8
# Sat, 10 Jun 2023 00:27:39 GMT
ENV JAVA_VERSION=21-ea+26
# Sat, 10 Jun 2023 00:27:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='16c6b09c742e73c9e092134517ecc36db2a5e44453c8b8b5374cfac1ee367a28'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='aa59bb222c548c18c21cb05a71854a46263a618a72ec6f2f408328689280380d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 10 Jun 2023 00:27:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e83e8f2e82cc31391cd0cb4f5ba574ba5eb9708fc0f5dcc34fef53b03ef28f31`  
		Last Modified: Fri, 31 Mar 2023 22:30:40 GMT  
		Size: 50.5 MB (50496029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7475b337670740c8f411f4efcbf2d4308101210ec581e69836860ffcd789ca`  
		Last Modified: Fri, 31 Mar 2023 23:14:05 GMT  
		Size: 14.2 MB (14240731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083c3747eb4b59dbc67d0f1d31d3d73ed49add38eab97a46785327c23bb0e9f5`  
		Last Modified: Sat, 10 Jun 2023 00:30:18 GMT  
		Size: 203.8 MB (203831849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-26-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d8ff57be8f616d53ebef37669892189610d9e1d0ac8e84bb46e99a216e8436f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268463980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8472a034246f5c812bfdfbe2f3c2d91e2f0a4e7cdfeaba1fd40318488ed7d906`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Jun 2023 03:45:43 GMT
ADD file:a9ba9c7acb256e802c7248b56f377a6f0ea08b1b61e11e482516633a13f4d686 in / 
# Wed, 14 Jun 2023 03:45:44 GMT
CMD ["/bin/bash"]
# Wed, 14 Jun 2023 04:08:20 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 14 Jun 2023 04:08:50 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 14 Jun 2023 04:08:50 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Jun 2023 04:08:50 GMT
ENV LANG=en_US.UTF-8
# Wed, 14 Jun 2023 04:08:50 GMT
ENV JAVA_VERSION=21-ea+26
# Wed, 14 Jun 2023 04:09:01 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-x64_bin.tar.gz'; 			downloadSha256='16c6b09c742e73c9e092134517ecc36db2a5e44453c8b8b5374cfac1ee367a28'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/26/GPL/openjdk-21-ea+26_linux-aarch64_bin.tar.gz'; 			downloadSha256='aa59bb222c548c18c21cb05a71854a46263a618a72ec6f2f408328689280380d'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 14 Jun 2023 04:09:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:52fd87ed40fcddc3fe63b876d1f94f6edae688637a5cc56983dced68a50c953e`  
		Last Modified: Wed, 14 Jun 2023 03:46:28 GMT  
		Size: 51.1 MB (51052081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aeb39f5d39e6fb51e698f8f5e6416d0689047f9392a9bd3f97f28c4d5d5596`  
		Last Modified: Wed, 14 Jun 2023 04:10:01 GMT  
		Size: 15.2 MB (15238146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1274d4f7aed0eba559a5727387cc9ae61bc854257911d561e0cad1d7472a5a`  
		Last Modified: Wed, 14 Jun 2023 04:10:53 GMT  
		Size: 202.2 MB (202173753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
