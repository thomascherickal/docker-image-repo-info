## `openjdk:20-ea-31-oracle`

```console
$ docker pull openjdk@sha256:5274a6412ced46c2afda5294504599605b16cf608e8a61de702406c2ed9a8300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-31-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:603755484a90243c7043527e8f21583a8a05c59dacc20606f3423b6ac55ab0c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254273291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1de0c86502709adae23f5584cb83fe67bc6d280ca07a68d82554d50187627483`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 Jan 2023 21:49:30 GMT
ADD file:599abbad96e264361b1bc5a7643f88354e406a2a1f55256af8a67e5a71ac3044 in / 
# Tue, 17 Jan 2023 21:49:31 GMT
CMD ["/bin/bash"]
# Wed, 18 Jan 2023 04:26:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 18 Jan 2023 04:27:24 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 18 Jan 2023 04:27:24 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 04:27:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Jan 2023 04:27:24 GMT
ENV JAVA_VERSION=20-ea+31
# Wed, 18 Jan 2023 04:27:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/31/GPL/openjdk-20-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='3269ddcaa2745f47e0610531a0c6f06671f7b85fd4c02ae4a29a6f14089748a6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/31/GPL/openjdk-20-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ee53148820a0f603ef492aa7c62154c043cf38cea3259581a79010d8297c2f5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 Jan 2023 04:27:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c57acc5afca507dabd7a22ed8ab1a978dad73d90dacad7b0b4668750f8fca64`  
		Last Modified: Tue, 17 Jan 2023 21:50:21 GMT  
		Size: 43.9 MB (43885845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8fb8780af51fbf2479bc74be4aef9eef6a67db84a17a1eadc0d9bb6464a16c`  
		Last Modified: Wed, 18 Jan 2023 04:31:02 GMT  
		Size: 12.3 MB (12251739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842595628e6911f1873740e04083094e281655fbc905ac65623d158821f1ca1`  
		Last Modified: Wed, 18 Jan 2023 04:32:13 GMT  
		Size: 198.1 MB (198135707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-31-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:97fe9ccc3fea73c3b9682d9617c0f0eeac8c329ea88f486ab8dc9e7e5f4c7eca
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.5 MB (252471727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b83712f0fab0f2915b0eb842aa888870be361b182fd5db3246ace2429d2579`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 17 Jan 2023 22:11:15 GMT
ADD file:dc09c8b8bd2fd3e0439792a21b95984ec8104b2a384f5ea2ef173918c105da9c in / 
# Tue, 17 Jan 2023 22:11:15 GMT
CMD ["/bin/bash"]
# Wed, 18 Jan 2023 04:00:40 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 18 Jan 2023 04:01:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 18 Jan 2023 04:01:04 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Jan 2023 04:01:05 GMT
ENV LANG=C.UTF-8
# Wed, 18 Jan 2023 04:01:05 GMT
ENV JAVA_VERSION=20-ea+31
# Wed, 18 Jan 2023 04:01:13 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/31/GPL/openjdk-20-ea+31_linux-x64_bin.tar.gz'; 			downloadSha256='3269ddcaa2745f47e0610531a0c6f06671f7b85fd4c02ae4a29a6f14089748a6'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/31/GPL/openjdk-20-ea+31_linux-aarch64_bin.tar.gz'; 			downloadSha256='6ee53148820a0f603ef492aa7c62154c043cf38cea3259581a79010d8297c2f5'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 18 Jan 2023 04:01:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:002eb071499b5ede36f617906154b8933e643acc41d2993585876528939fb80f`  
		Last Modified: Tue, 17 Jan 2023 22:11:59 GMT  
		Size: 42.8 MB (42775871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceecd3085b25f549de68213105de48a98b0db45a66e38d315c34ae860197f1a`  
		Last Modified: Wed, 18 Jan 2023 04:04:31 GMT  
		Size: 13.1 MB (13068620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc961efda62f327353594b3eda4efd920713f0c905e5314d89010afb48d05bb`  
		Last Modified: Wed, 18 Jan 2023 04:05:38 GMT  
		Size: 196.6 MB (196627236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
