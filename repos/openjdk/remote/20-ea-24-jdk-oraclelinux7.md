## `openjdk:20-ea-24-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:aa7fe1d495a88fb1b2db2478ea1c8d99693943c8113b14157c50e609241c49cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-24-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:2f89a120f3e42da4d85b6ac217981ddbd4c7ff9d2d8d6a5457b76bade39c8b5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.3 MB (262322328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac92724b00f801dffa493a89eb86899cde27bf8e41f711802ff1493a71b0ea81`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:20:17 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 05 Nov 2022 02:20:17 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 02:20:17 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 02:20:17 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Nov 2022 01:41:53 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:42:04 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:42:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9a0b9cd2dfe62ff7a933afe41891425abf01b0aaed70cedb028f03392d60037f`  
		Last Modified: Fri, 04 Nov 2022 23:35:26 GMT  
		Size: 49.8 MB (49827924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd91916b9b5718027cc164239330e952a98aeb093ce9bd81860aa1729904850`  
		Last Modified: Sat, 05 Nov 2022 02:24:18 GMT  
		Size: 14.2 MB (14218114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ac7de56a1409bf37ecb0f979ac274b8682c77027f6c85635e463f5dcf8fc44`  
		Last Modified: Fri, 18 Nov 2022 01:46:31 GMT  
		Size: 198.3 MB (198276290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-24-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d0fc9f150b6d1e3c93da99a120bbca8343f9a76a4d3619f2f5f485f618beaadd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262506431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99f7e6e0b0bb031d256101ac04be083e2ca29b48670f1c8aa9d57ba4517a4269`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:27 GMT
ADD file:4d172a457b1d27e8913a5e05a18d79d4b651e2d8677c9391e5d838f8b88ecaf7 in / 
# Fri, 04 Nov 2022 22:50:28 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:50:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 05 Nov 2022 00:50:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Sat, 05 Nov 2022 00:50:12 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:50:12 GMT
ENV LANG=en_US.UTF-8
# Fri, 18 Nov 2022 01:57:51 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:58:03 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:58:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bb54b8cf6e14ad1a2ea509cf62cacf70a75fe1fc21dba31199165b9534e1b8c1`  
		Last Modified: Fri, 04 Nov 2022 22:52:11 GMT  
		Size: 50.4 MB (50401543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25e3b537f11ad791c5f6c0140d98f0ff4716add37dcc3762f87c091b8d79048`  
		Last Modified: Sat, 05 Nov 2022 00:54:35 GMT  
		Size: 15.3 MB (15262905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ba3204ed27173747ae8ef414f7c8f42bbbd7aaff53f866f14a686107115c5`  
		Last Modified: Fri, 18 Nov 2022 02:02:29 GMT  
		Size: 196.8 MB (196841983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
