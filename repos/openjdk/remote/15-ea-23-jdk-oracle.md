## `openjdk:15-ea-23-jdk-oracle`

```console
$ docker pull openjdk@sha256:9d8e384641bab66671c4d0f840dc9a0457238e95d2d27960d1e96d4552d74b8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-ea-23-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:dcaff114f61368b32c4f067885fecc3fc3227fde485b192ba60edf43c62b150d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250273342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624da38a493435711378241fc0d6285d6c7b9b0b802ea9182e09e132295fd467`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 04 May 2020 20:20:53 GMT
ADD file:d23891d2372d6aae3d738388c74dacd92f9406083ee0c1ac0e2bfd140f92ec2b in / 
# Mon, 04 May 2020 20:20:53 GMT
CMD ["/bin/bash"]
# Mon, 04 May 2020 20:38:21 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Mon, 04 May 2020 20:38:21 GMT
ENV LANG=en_US.UTF-8
# Mon, 04 May 2020 20:38:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Mon, 04 May 2020 20:38:21 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 May 2020 20:58:26 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 22 May 2020 01:21:26 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-aarch64_bin.tar.gz; 			downloadSha256=c9817b2efa619dcde0d4a5fa9dd1d6bcbe5bdf05fee152e9a06387544c4e5c90; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz; 			downloadSha256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 22 May 2020 01:21:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:83755823a002357171a0b229ef5769a60db47a90b624adc45f8c6b7cd1d1394f`  
		Last Modified: Mon, 04 May 2020 20:22:07 GMT  
		Size: 43.5 MB (43455265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e105caaf23acf967db67aa1f683d428603dbb51e12295bfe8f5df6a4cce8bb`  
		Last Modified: Mon, 04 May 2020 20:40:58 GMT  
		Size: 14.8 MB (14758294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbbf40cf391760f79c8a138e8234829abedd40c54c6b8a19b093df3772bd66b`  
		Last Modified: Fri, 22 May 2020 01:26:10 GMT  
		Size: 192.1 MB (192059783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-ea-23-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:18c45ac3be3c05fecb60d21db75dc6ee4c26109c6cdaad6361a3e72aa1934790
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.2 MB (233217482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686360b5f07f25f56af65608260068bb82b3ee1233962f448d8080a9bc558775`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 04 May 2020 20:42:34 GMT
ADD file:b059ded860ba734fbe035c768d5c7e01a82decd7db5ca12f093672dab3b204c3 in / 
# Mon, 04 May 2020 20:42:37 GMT
CMD ["/bin/bash"]
# Fri, 22 May 2020 01:43:47 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 22 May 2020 01:43:48 GMT
ENV LANG=en_US.UTF-8
# Fri, 22 May 2020 01:43:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 22 May 2020 01:43:49 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 May 2020 01:43:50 GMT
ENV JAVA_VERSION=15-ea+23
# Fri, 22 May 2020 01:45:15 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-aarch64_bin.tar.gz; 			downloadSha256=c9817b2efa619dcde0d4a5fa9dd1d6bcbe5bdf05fee152e9a06387544c4e5c90; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/23/GPL/openjdk-15-ea+23_linux-x64_bin.tar.gz; 			downloadSha256=0a3a3f2bb3005d848f9a579c46c1cb581b46d6805faf673a7c1b5a2f158cd1b0; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 22 May 2020 01:45:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fa5299bfe4aa00db1c3f39321cc679889e30f51f690a75b8c75163698c4c7831`  
		Last Modified: Mon, 04 May 2020 20:43:38 GMT  
		Size: 44.1 MB (44074523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342df9bce1d80b8bdf565c6ceb8cbb008ee180f7fd52e3006d84ae4f81d0dc67`  
		Last Modified: Fri, 22 May 2020 01:48:19 GMT  
		Size: 15.0 MB (15028449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3fd8200fdfff9aca28885f3b5af2627050e0f3091bc7693d31f40d0457128b`  
		Last Modified: Fri, 22 May 2020 01:48:40 GMT  
		Size: 174.1 MB (174114510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
