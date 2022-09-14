## `openjdk:20-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:8f398943135aa1d3edd5da3026886d205481b3581c8629e773d1210932ee318c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:29f74b38b2519b953f73c473e832e7476214d2a1625b95ed38e57d242282d2e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249668259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b1086ade108aa9631878b63e516cbafc5b9745a0398fd5ca66a870db64c953`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Sep 2022 21:20:28 GMT
ADD file:e00d9d8d8f616feec8c064f2250e4836ea3b533ead0611d1af2245974abb4e88 in / 
# Wed, 14 Sep 2022 21:20:28 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 21:37:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 14 Sep 2022 21:37:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 14 Sep 2022 21:37:14 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Sep 2022 21:37:14 GMT
ENV LANG=C.UTF-8
# Wed, 14 Sep 2022 21:37:15 GMT
ENV JAVA_VERSION=20-ea+14
# Wed, 14 Sep 2022 21:37:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/14/GPL/openjdk-20-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='ce9c99a0d70bf7c6548b68a33770a50d1273d5d5ea72522a1fe91ae6d3f22c1d'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/14/GPL/openjdk-20-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='4935236eb4e51be13ddfcc1ce717191128feb8ff9329676971ea54775261d9ff'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 14 Sep 2022 21:37:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:051f419db9dd9462e8995886d24f592c26cef792cc915dfbc7548e0b19aa55fe`  
		Last Modified: Wed, 14 Sep 2022 21:21:25 GMT  
		Size: 40.6 MB (40590248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa51c6010a14c1984cbdea1332a5d2f77bf6e0141bc497b44dca611e21f9b391`  
		Last Modified: Wed, 14 Sep 2022 21:41:16 GMT  
		Size: 12.2 MB (12232427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1de9fd0d70d3695809ab481e64677aef3930c6970bdffbc2058f56cbb51c46`  
		Last Modified: Wed, 14 Sep 2022 21:41:30 GMT  
		Size: 196.8 MB (196845584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:61a92e9e5b817140720cb5085e3bddf48ecbc948c0220737f2cf04b62cb66258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.8 MB (247824889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:327fc2d7dfc1589b0bf7cf0f26426f1b504482683be19374868b0ae596a19b4b`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 14 Sep 2022 21:41:16 GMT
ADD file:30401488699aa4b911abaeec83f0938e0fede937c09940369ec58cc56eae4624 in / 
# Wed, 14 Sep 2022 21:41:17 GMT
CMD ["/bin/bash"]
# Wed, 14 Sep 2022 22:01:28 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 14 Sep 2022 22:01:28 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 14 Sep 2022 22:01:29 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 14 Sep 2022 22:01:30 GMT
ENV LANG=C.UTF-8
# Wed, 14 Sep 2022 22:01:31 GMT
ENV JAVA_VERSION=20-ea+14
# Wed, 14 Sep 2022 22:01:44 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/14/GPL/openjdk-20-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='ce9c99a0d70bf7c6548b68a33770a50d1273d5d5ea72522a1fe91ae6d3f22c1d'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/14/GPL/openjdk-20-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='4935236eb4e51be13ddfcc1ce717191128feb8ff9329676971ea54775261d9ff'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 14 Sep 2022 22:01:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9a8b791677e1fdf76ff862b55362355b48c8636d0eabf606d1af65888ab73ec8`  
		Last Modified: Wed, 14 Sep 2022 21:42:22 GMT  
		Size: 39.4 MB (39409909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1458b25adde8441e97a5f07c35975478bc0d77410ada29b87b31f52fbbaf994`  
		Last Modified: Wed, 14 Sep 2022 22:09:27 GMT  
		Size: 13.1 MB (13055052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb649ad427168cb643ed70b488042132140d468c756370675e7618aefef860e1`  
		Last Modified: Wed, 14 Sep 2022 22:09:47 GMT  
		Size: 195.4 MB (195359928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
