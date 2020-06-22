## `openjdk:16-ea-2-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:3c1841393f6e9638e88c7e41e4541bfaec501d431664b540ff978d23805a4550
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-ea-2-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:54064b99eb28ac9bac30953f5096e88f2507400546026a06bd477b131a51736b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.0 MB (253983148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f9ad3f17bcfdb986fc3263715df302ff89915801cc11aad8e31cd27412b6a2`
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
# Mon, 22 Jun 2020 19:30:29 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 20:21:07 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-aarch64_bin.tar.gz; 			downloadSha256=c166b3aeb4901a4b082b99e73234b4a7603ae123505a20aca7d7ab907a25903d; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-x64_bin.tar.gz; 			downloadSha256=5a29aad9b578aaa3427522f4e777e273b3c92f8b7befa8e5c8819741e168ec1c; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Mon, 22 Jun 2020 20:21:08 GMT
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
	-	`sha256:1b00c1f65453dd4941f4f47ce5080b36da25a6415624ec55b0ba4f5734081dcb`  
		Last Modified: Mon, 22 Jun 2020 20:25:46 GMT  
		Size: 195.8 MB (195765421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-ea-2-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:062cd27bb5b177f4ee7bdf62ee1d6392ec1867e02fb5b2ef9f602c109dfbbab5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233948430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a5842fb008bf6e3d70fa480e8838818bfcddeeaabe3de68950f3df522d4d3d7`
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
# Mon, 22 Jun 2020 20:03:04 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 20:03:49 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-aarch64_bin.tar.gz; 			downloadSha256=c166b3aeb4901a4b082b99e73234b4a7603ae123505a20aca7d7ab907a25903d; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk16/2/GPL/openjdk-16-ea+2_linux-x64_bin.tar.gz; 			downloadSha256=5a29aad9b578aaa3427522f4e777e273b3c92f8b7befa8e5c8819741e168ec1c; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Mon, 22 Jun 2020 20:03:50 GMT
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
	-	`sha256:a1f5f8ef50d700a4386e6db3f58fe7ab488740817ee601d0466e71050a24314f`  
		Last Modified: Mon, 22 Jun 2020 20:08:51 GMT  
		Size: 174.9 MB (174863226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
