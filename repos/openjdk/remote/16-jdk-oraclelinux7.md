## `openjdk:16-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:c3e368f22362799312b1e6c1223455303819d952a8ac6dde7429b93fd51a9121
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:92384ba69bba3132d9257f1b5861cf385aab58d082a521b2f66b34ed9f95189d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.1 MB (254097383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8306b5b9627c2abbbfe14eb0737eafd436e3406e5d9806a66051c48a3cf908f5`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Wed, 10 Jun 2020 18:22:32 GMT
ADD file:79bb5b8b89fe54ba99fd9d42d4f8774bfb9c1319ac3ead17a2005a3bde852451 in / 
# Wed, 10 Jun 2020 18:22:32 GMT
CMD ["/bin/bash"]
# Wed, 10 Jun 2020 18:39:27 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 10 Jun 2020 18:39:28 GMT
ENV LANG=en_US.UTF-8
# Thu, 18 Jun 2020 20:37:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 18 Jun 2020 20:37:39 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Jun 2020 20:37:39 GMT
ENV JAVA_VERSION=16-ea+1
# Thu, 18 Jun 2020 20:38:21 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/1/GPL/openjdk-16-ea+1_linux-aarch64_bin.tar.gz; 			downloadSha256=ee2dcc864f03cbf35d5e87c039de02dd133b593a0e69865ec6a6a5128e74e9f7; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/1/GPL/openjdk-16-ea+1_linux-x64_bin.tar.gz; 			downloadSha256=ff4188d2c3ae82c9103e79ebe417eedf943ba67823ef9d4ff89a5e385449d520; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Thu, 18 Jun 2020 20:38:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fa926a7d213a8145d6a906d68a085b21909a4b26871f142804e68b322bf8881f`  
		Last Modified: Wed, 10 Jun 2020 18:23:43 GMT  
		Size: 43.5 MB (43457466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22aed8993d2fb0bb3a658c631a1dfbd05c0e5d42218f419d18238996bd06ea08`  
		Last Modified: Wed, 10 Jun 2020 18:42:25 GMT  
		Size: 14.8 MB (14760261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a725c558c44afad8008e1ac86b6199256aaa8d0491f6c8ba317e26a8fe880257`  
		Last Modified: Thu, 18 Jun 2020 20:42:05 GMT  
		Size: 195.9 MB (195879656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d6a6bcd3bb8e9b9da66b790953aeeb6aad77798ea4770ee20025c3cbbe20ad7c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (234048331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3ce082b91ed08f825b626fd710f1672cfb700818700f5e7f0bd9310042c3a25`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Wed, 10 Jun 2020 18:54:47 GMT
ADD file:64c488ae0df14676929e149538eb50b12e9a99518a126c88ee9704e8a88424e5 in / 
# Wed, 10 Jun 2020 18:54:49 GMT
CMD ["/bin/bash"]
# Wed, 10 Jun 2020 19:12:05 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 10 Jun 2020 19:12:06 GMT
ENV LANG=en_US.UTF-8
# Thu, 18 Jun 2020 23:55:12 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Thu, 18 Jun 2020 23:55:13 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Jun 2020 23:55:14 GMT
ENV JAVA_VERSION=16-ea+1
# Thu, 18 Jun 2020 23:56:03 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/1/GPL/openjdk-16-ea+1_linux-aarch64_bin.tar.gz; 			downloadSha256=ee2dcc864f03cbf35d5e87c039de02dd133b593a0e69865ec6a6a5128e74e9f7; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/1/GPL/openjdk-16-ea+1_linux-x64_bin.tar.gz; 			downloadSha256=ff4188d2c3ae82c9103e79ebe417eedf943ba67823ef9d4ff89a5e385449d520; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Thu, 18 Jun 2020 23:56:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9b791ce794f1b8ac779f7e2bb939c8f822209f7507dbc7f70d072d98b700e55a`  
		Last Modified: Wed, 10 Jun 2020 18:55:52 GMT  
		Size: 44.1 MB (44072411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7857b3d293f1062b1c04189b86491b9bbfd2e793fec6975e1bdcabf4ef9ed3`  
		Last Modified: Wed, 10 Jun 2020 19:14:19 GMT  
		Size: 15.0 MB (15012793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199cb58622c8f2a577c7776e49e602f0a71757b1c8be66b70015841d16b666d6`  
		Last Modified: Thu, 18 Jun 2020 23:59:52 GMT  
		Size: 175.0 MB (174963127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
