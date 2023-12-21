## `openjdk:23-jdk-oracle`

```console
$ docker pull openjdk@sha256:6640460e426f80ba0111afd79633e41d57b276423d50424f1ac84e24fe2f2758
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `openjdk:23-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:8a7f3e3844a8ba626b8dccf59523d473b20d74b73efa6f24f7470010f0815995
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.3 MB (269273420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6166d381a157fd324a7624df49ee8a25713b9a617d25dd2a650af235012f336b`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Dec 2023 19:53:43 GMT
ADD file:da89b67e484bc45f357250a868fd78e28086b13e4315635d19648e5d43812e89 in / 
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:53:43 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_VERSION=23-ea+2
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='c10168b0639ae5a316fb20444202e82fabe5908be7241f1cd42e34ed9d1eca76'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='84b416aba4f3578138dd0d27f570dbaee9123528c4d45d13a338278c3d7136c1'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bce031bc522d421fb188ef82a530f85c5477bb87cdeacdb911ea86f3f7cd3b66`  
		Last Modified: Wed, 20 Dec 2023 22:42:00 GMT  
		Size: 51.3 MB (51323468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d986f6e16b814d17738e29faaa870ea909cb21aef547eab206d33b92ad75acd7`  
		Last Modified: Thu, 21 Dec 2023 00:40:48 GMT  
		Size: 15.0 MB (14995426 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09263cab735c482e50f635c1f064f9ad065e933972c8062f592c04766e2dff65`  
		Last Modified: Thu, 21 Dec 2023 00:40:51 GMT  
		Size: 203.0 MB (202954526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-oracle` - unknown; unknown

```console
$ docker pull openjdk@sha256:18848b24256c23151237e501293d0a35bc85115e0fdf0cbc05fd2c8d83721ad8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1935697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9fa10100444cc58d1de0579d5c1944b39a90a546a851b10601819a75125040`

```dockerfile
```

-	Layers:
	-	`sha256:0dc8980fd21b51deecf08bd367871858eb93cb4d2401450acf5f50e947c6b560`  
		Last Modified: Thu, 21 Dec 2023 00:40:47 GMT  
		Size: 1.9 MB (1915833 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e0f917f7c25e0733d0704015e10e671ca541884e6d4d0ade5be72ef9e9231d6`  
		Last Modified: Thu, 21 Dec 2023 00:40:47 GMT  
		Size: 19.9 KB (19864 bytes)  
		MIME: application/vnd.in-toto+json

### `openjdk:23-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:56870dab24bc1a2ae161f891ee14cd878f2f707dcf1036c7fe2426bd84fbcedc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.6 MB (266631475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c0f90aa67e4f22f77c1d08608a173974732abbefdc82babd9f6057aa72cbd5`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 15 Dec 2023 19:53:43 GMT
ADD file:b736c1bb75174fcadec81f68a30d2db09432c3999d3df92c07c057a5cc8b07a6 in / 
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-23
# Fri, 15 Dec 2023 19:53:43 GMT
ENV PATH=/usr/java/openjdk-23/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 15 Dec 2023 19:53:43 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 19:53:43 GMT
ENV JAVA_VERSION=23-ea+2
# Fri, 15 Dec 2023 19:53:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-x64_bin.tar.gz'; 			downloadSha256='c10168b0639ae5a316fb20444202e82fabe5908be7241f1cd42e34ed9d1eca76'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk23/2/GPL/openjdk-23-ea+2_linux-aarch64_bin.tar.gz'; 			downloadSha256='84b416aba4f3578138dd0d27f570dbaee9123528c4d45d13a338278c3d7136c1'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version # buildkit
# Fri, 15 Dec 2023 19:53:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f065eb68ef2e8ae9b60daa693d770aedc4bf77fb5bacc4b006960acc8eb01f28`  
		Last Modified: Wed, 20 Dec 2023 22:54:12 GMT  
		Size: 50.1 MB (50079714 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e51f352f0f1de3c800e109fad5b2dae0cb9097249a14ca89d420642f858cc188`  
		Last Modified: Thu, 21 Dec 2023 07:07:40 GMT  
		Size: 15.7 MB (15690041 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f75820942c8cc7f26b1e815ebc5e01810117c60750d4a8fbf2b8bc2dae036b0b`  
		Last Modified: Thu, 21 Dec 2023 07:07:46 GMT  
		Size: 200.9 MB (200861720 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `openjdk:23-jdk-oracle` - unknown; unknown

```console
$ docker pull openjdk@sha256:5e95f95382da172efb79b361204a7eae4683a2c3fc6b549a72916b7b25fd56f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 MB (1934148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4ff261ec94c82691205a412c2b6d8cfb96c0b9bdb81f8a296b46a2eb25d906`

```dockerfile
```

-	Layers:
	-	`sha256:f0c650cec62b7467a20a2d4760e31d31842c58700d329b1f382d64da669cc6e5`  
		Last Modified: Thu, 21 Dec 2023 07:07:39 GMT  
		Size: 1.9 MB (1914413 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:27b015db920cfed59be976feadce4df6fe6be8332715a294da232a6df94cd21c`  
		Last Modified: Thu, 21 Dec 2023 07:07:39 GMT  
		Size: 19.7 KB (19735 bytes)  
		MIME: application/vnd.in-toto+json
