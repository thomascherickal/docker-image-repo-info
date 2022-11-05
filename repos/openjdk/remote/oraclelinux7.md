## `openjdk:oraclelinux7`

```console
$ docker pull openjdk@sha256:7c7d7df94b82c9360418d119d645838829264a65983419b3b1f21fc58decd003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:72581b4329ade3564fddb62452a0eadb6f38448279565c3402a68914ecbd5bff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.8 MB (252789856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a4125443b375762e543b45b6b2bbf369386f509d5b31db0da015807aff62a3`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 23:33:35 GMT
ADD file:aaaadfdf901c2df5f641e6c43b10817fcbd0caca73acb7672608f43ba71cefeb in / 
# Fri, 04 Nov 2022 23:33:36 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 02:20:17 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 05 Nov 2022 02:21:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Sat, 05 Nov 2022 02:21:06 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 02:21:06 GMT
ENV LANG=en_US.UTF-8
# Sat, 05 Nov 2022 02:21:06 GMT
ENV JAVA_VERSION=18.0.2.1
# Sat, 05 Nov 2022 02:21:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 02:21:17 GMT
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
	-	`sha256:a9ba674f49afd41534cf425e08df397f095758806fd995e61084e15a50b9ca12`  
		Last Modified: Sat, 05 Nov 2022 02:26:21 GMT  
		Size: 188.7 MB (188743818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:e3896cba76531481720edfbf4daebd0d36de96182f42db5b52ecf60bd4b49add
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.3 MB (253325849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9014f765ecad5ab5f96662470ba265f641179298b3a235ba706ef5f9b975762`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 04 Nov 2022 22:50:27 GMT
ADD file:4d172a457b1d27e8913a5e05a18d79d4b651e2d8677c9391e5d838f8b88ecaf7 in / 
# Fri, 04 Nov 2022 22:50:28 GMT
CMD ["/bin/bash"]
# Sat, 05 Nov 2022 00:50:12 GMT
RUN set -eux; 	yum install -y --setopt=skip_missing_names_on_install=False 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Sat, 05 Nov 2022 00:51:06 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Sat, 05 Nov 2022 00:51:06 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 00:51:06 GMT
ENV LANG=en_US.UTF-8
# Sat, 05 Nov 2022 00:51:06 GMT
ENV JAVA_VERSION=18.0.2.1
# Sat, 05 Nov 2022 00:51:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-x64_bin.tar.gz'; 			downloadSha256='3bfdb59fc38884672677cebca9a216902d87fe867563182ae8bc3373a65a2ebd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18.0.2.1/db379da656dc47308e138f21b33976fa/1/GPL/openjdk-18.0.2.1_linux-aarch64_bin.tar.gz'; 			downloadSha256='79900237a5912045f8c9f1065b5204a474803cbbb4d075ab9620650fb75dfc1b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 05 Nov 2022 00:51:23 GMT
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
	-	`sha256:fbfc2573fd920c62423e2b8e956e3514333cac65fa560fabf5de3b571f5ead66`  
		Last Modified: Sat, 05 Nov 2022 00:56:31 GMT  
		Size: 187.7 MB (187661401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
