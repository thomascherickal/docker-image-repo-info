## `openjdk:15-jdk-oracle`

```console
$ docker pull openjdk@sha256:1e9055f25a90b237414dfab5d0223e74f399c31065aea2599cd43dc932c9d420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:15-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:4711f82bd00dd50079ae252615f272e817c5a78797d6fb65f974aa44c10b30c1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.4 MB (263406883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fff2ebb59bb6517c3e24831823794da2732ecb14df8a7563e2c2f4ab863d846`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 14 Sep 2020 18:33:21 GMT
ADD file:8011e31575cbf4b8ebb243821b300ba24330e02cab925024aa98f4ce27997846 in / 
# Mon, 14 Sep 2020 18:33:21 GMT
CMD ["/bin/bash"]
# Mon, 14 Sep 2020 18:50:46 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 14 Sep 2020 18:50:46 GMT
ENV LANG=C.UTF-8
# Mon, 14 Sep 2020 18:51:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Mon, 14 Sep 2020 18:51:54 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Sep 2020 18:51:54 GMT
ENV JAVA_VERSION=15
# Mon, 14 Sep 2020 18:52:40 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 14 Sep 2020 18:52:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:79701ada7495177c292979fd69d41eee91dc93ef0feea5ff95bb453f4ab7a1c5`  
		Last Modified: Mon, 14 Sep 2020 18:35:00 GMT  
		Size: 54.2 MB (54164063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffa6cd00cf525ae203ffe0f93764b5d175c46f27a7e15bb0da88efb308e5292`  
		Last Modified: Mon, 14 Sep 2020 18:55:41 GMT  
		Size: 13.5 MB (13491747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b8613aa641f3057f2233da22f2218260f14fb12cc2e644f6e3c12f59f0555`  
		Last Modified: Mon, 14 Sep 2020 18:56:50 GMT  
		Size: 195.8 MB (195751073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:27ea1013c7428cbb01d9611729a0acd88cf6acc65d4fcbf7be3d5efdf3e9c999
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.5 MB (243492507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:665156d548e1413141463ea53d3fb47c936673eca2879d06fe6e9cd426ca103c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 31 May 2019 21:40:52 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Mon, 14 Sep 2020 17:42:14 GMT
ADD file:b3bd5c2ec8ff0efe8a0b1384563b42f02d6bcf7531132d9ec4748ecfe264d476 in / 
# Mon, 14 Sep 2020 17:42:18 GMT
CMD ["/bin/bash"]
# Mon, 14 Sep 2020 17:59:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Mon, 14 Sep 2020 18:00:04 GMT
ENV LANG=C.UTF-8
# Mon, 14 Sep 2020 18:01:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Mon, 14 Sep 2020 18:01:47 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Sep 2020 18:01:49 GMT
ENV JAVA_VERSION=15
# Mon, 14 Sep 2020 18:02:39 GMT
RUN set -eux; 		objdump="$(command -v objdump)"; 	arch="$(objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		arm64 | aarch64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-aarch64_bin.tar.gz; 			downloadSha256=01e7e07dd8a67a65b32fdcaff75ba3f21cd9cfc749287e7c9b1c6037f96a3537; 			;; 		amd64 | i386:x86-64) 			downloadUrl=https://download.java.net/java/GA/jdk15/779bf45e88a44cbd9ea6621d33e33db1/36/GPL/openjdk-15_linux-x64_bin.tar.gz; 			downloadSha256=bb67cadee687d7b486583d03c9850342afea4593be4f436044d785fba9508fb7; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 14 Sep 2020 18:02:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a805b9845b615e5963d09def3e5e9919b39e76b5122c2abecc98d4a4bb358394`  
		Last Modified: Mon, 14 Sep 2020 17:43:27 GMT  
		Size: 54.3 MB (54266593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dee2ba14d3dd42ac318a14c434bced8bd3cc7a2c58339deb209699b1d167b21`  
		Last Modified: Mon, 14 Sep 2020 20:56:35 GMT  
		Size: 14.4 MB (14366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c962550dadc0ccae13f43c26067641e639dd560cd6f0f96e1826189b592551db`  
		Last Modified: Mon, 14 Sep 2020 20:59:35 GMT  
		Size: 174.9 MB (174859078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
