## `openjdk:15-ea-31-jdk-oracle`

```console
$ docker pull openjdk@sha256:43f8f2d1ff190215460440dd5d24185dbe32bdf6432658abd5bdcc3aa0bd079d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm64 variant v8

### `openjdk:15-ea-31-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:6bb9df077c8fe4b15c0b959817347c4760c3601911e4b84d5008a408d5ea3fce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.9 MB (233919196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58a6784aa59da252a67e82c3b895a8770e46e7c1a0fd91e503f4ec4c1421c13d`
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
# Wed, 10 Jun 2020 19:12:07 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Wed, 10 Jun 2020 19:12:07 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Jul 2020 02:33:50 GMT
ENV JAVA_VERSION=15-ea+31
# Fri, 10 Jul 2020 02:34:35 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/31/GPL/openjdk-15-ea+31_linux-aarch64_bin.tar.gz; 			downloadSha256=27ef4fe5b302ff8804a86a7b455ebd16a5adbfb0f83cf8453026957a46088455; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/early_access/jdk15/31/GPL/openjdk-15-ea+31_linux-x64_bin.tar.gz; 			downloadSha256=87a9314b733f711973093455f055a9f461a01a7c52dfe77d29da67d47795141b; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o /openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 */openjdk.tgz" | sha256sum -c -; 		mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		java --version; 	javac --version
# Fri, 10 Jul 2020 02:34:38 GMT
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
	-	`sha256:0c3548e570ad2173fe1cd8b65c0bd4e7c45af3b00928fa908ab5a930509342e7`  
		Last Modified: Fri, 10 Jul 2020 02:39:38 GMT  
		Size: 174.8 MB (174833992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
