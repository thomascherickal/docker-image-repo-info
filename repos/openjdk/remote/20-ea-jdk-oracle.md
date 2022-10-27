## `openjdk:20-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:15078c64274beb575dee4db1655042e34861dbb26224f8dc99ee81adff2f8e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:8ce314169dfd252b7f3e742e25cb478925cdbf7b39a60fd8c50f10ed5588e973
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249923148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:839ca5c9c54312f436cee15bec79f0a337309afee4d41a44d22acac52b328c87`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Oct 2022 17:21:44 GMT
ADD file:bb73a6f29d54ad7e2f7ec0aeeb404b06eee41432910aa60dd8f9ec5cdb904455 in / 
# Thu, 27 Oct 2022 17:21:44 GMT
CMD ["/bin/bash"]
# Thu, 27 Oct 2022 17:39:38 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 27 Oct 2022 17:39:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 27 Oct 2022 17:39:38 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Oct 2022 17:39:38 GMT
ENV LANG=C.UTF-8
# Thu, 27 Oct 2022 17:39:38 GMT
ENV JAVA_VERSION=20-ea+20
# Thu, 27 Oct 2022 17:39:49 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 Oct 2022 17:39:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d67a603b911ada80815df642621203365c074f4903f50aed87dcf6df07e6e4c6`  
		Last Modified: Thu, 27 Oct 2022 17:23:23 GMT  
		Size: 40.6 MB (40581871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80422febbaefdcc8ba66af30635f777afc7bef13f71ad47f90af2a5da4e8099`  
		Last Modified: Thu, 27 Oct 2022 17:42:41 GMT  
		Size: 12.2 MB (12223871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa359fe060464a6cf16a750f8c4d3b6f81ca3cc70951b9f03af532d3ef2fbf55`  
		Last Modified: Thu, 27 Oct 2022 17:42:55 GMT  
		Size: 197.1 MB (197117406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:cf24f53b3637160d6f152301079de029044ad4bba97d2c8999ab7b0fdb56caab
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.1 MB (248134068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca59314726d3fa7db69bc0ae17a4ab2abe48b1c90fcb9f40a4b138b1948da5e3`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 27 Oct 2022 17:48:04 GMT
ADD file:9972b7a185a3ff13a8ec0490c58d6e2b47d402e40b486eb32e78f2fd0919c27e in / 
# Thu, 27 Oct 2022 17:48:04 GMT
CMD ["/bin/bash"]
# Thu, 27 Oct 2022 18:08:03 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 27 Oct 2022 18:08:03 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 27 Oct 2022 18:08:04 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Oct 2022 18:08:04 GMT
ENV LANG=C.UTF-8
# Thu, 27 Oct 2022 18:08:04 GMT
ENV JAVA_VERSION=20-ea+20
# Thu, 27 Oct 2022 18:08:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-x64_bin.tar.gz'; 			downloadSha256='0cb0f79bee2e61134a86049952a1e572bb3e2dad49aa200a20f18c697715a402'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/20/GPL/openjdk-20-ea+20_linux-aarch64_bin.tar.gz'; 			downloadSha256='4db7319dfbfb4a3561e9707c0178d0ba8d6413bc94f13d8c9ce406fd7445e000'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 27 Oct 2022 18:08:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:67fb6ea658c323fd156e1a1606d34b6fb59066aa9985abaa0f6c60ad6e91fab1`  
		Last Modified: Thu, 27 Oct 2022 17:49:29 GMT  
		Size: 39.4 MB (39409912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f0bec0421380148673bf482c1454b86ac9d0915765c91eb8f6262fbf649809`  
		Last Modified: Thu, 27 Oct 2022 18:13:59 GMT  
		Size: 13.1 MB (13050232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bb60113a481a4cfae8838846f1d78995dc8c7a7bd9de5acd8f3404ddce8905`  
		Last Modified: Thu, 27 Oct 2022 18:14:09 GMT  
		Size: 195.7 MB (195673924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
