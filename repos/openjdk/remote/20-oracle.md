## `openjdk:20-oracle`

```console
$ docker pull openjdk@sha256:488f74c13fb7c1794e80a5bf7563102278140e958535040e8833d9486ae98e7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:ff53ffcca3483886356371c19e9751f4bee06dfade70d3de37815cf99c5a41e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.4 MB (254384967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:376d3747fcfe35115d22727f60059ac5412b9fc13f092d23450e8d272ddbb044`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 16 Nov 2022 07:52:28 GMT
ADD file:dc61a65eefcb58f8747074284cd3dd5a6f2885c21dd35370e6f184b9e8a51eee in / 
# Wed, 16 Nov 2022 07:52:29 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 08:45:49 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 16 Nov 2022 08:45:49 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 16 Nov 2022 08:45:49 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 08:45:49 GMT
ENV LANG=C.UTF-8
# Fri, 18 Nov 2022 01:41:32 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:41:47 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:41:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0bb5c0c24818c7d2abc9b51381985dfc00d9845e8a60062b26d28116af012db9`  
		Last Modified: Wed, 16 Nov 2022 07:53:24 GMT  
		Size: 43.9 MB (43869924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2939e28fefc8d8e79bec97d26786781edb063fe6bb9b814bcb9783044f279d`  
		Last Modified: Wed, 16 Nov 2022 08:49:12 GMT  
		Size: 12.2 MB (12241330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376a97324eda819a9a82c0298452e47329264278be44aea6041352e3fe9c8588`  
		Last Modified: Fri, 18 Nov 2022 01:45:47 GMT  
		Size: 198.3 MB (198273713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:54d60abf647fafca5512225645591f4aa9f45dc3ca582da3a95b9418638a45b6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252678735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e576f3e3d5f76b3522473422de9b659f439812189b7f4678962ad9462643f4b`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 15 Nov 2022 23:40:44 GMT
ADD file:44569001378d2d59b2d169aba48a6b2b88529ca46fd5d85598eff7ca37ded076 in / 
# Tue, 15 Nov 2022 23:40:45 GMT
CMD ["/bin/bash"]
# Wed, 16 Nov 2022 01:36:22 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 16 Nov 2022 01:36:22 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 16 Nov 2022 01:36:22 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 01:36:22 GMT
ENV LANG=C.UTF-8
# Fri, 18 Nov 2022 01:57:30 GMT
ENV JAVA_VERSION=20-ea+24
# Fri, 18 Nov 2022 01:57:44 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='f73656bed38d61eb8b7c771a59ad326adeb625e5f18e92b7fd11f657d1005d54'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/24/GPL/openjdk-20-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='58fb9a1ea196a73f54b3ab94189cb6eaece44105eb82d113db57b6ab51aca5e6'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 18 Nov 2022 01:57:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:01d65ebb4955ae24720eb5c24ff08081fed75975aea7b87c96ef7e58175901e0`  
		Last Modified: Tue, 15 Nov 2022 23:41:32 GMT  
		Size: 42.8 MB (42774711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eefa7d15fae88e599b20bbe34f347a8686634ade1cdb17b1d84e66775c495fa`  
		Last Modified: Wed, 16 Nov 2022 01:39:40 GMT  
		Size: 13.1 MB (13066354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60a42aaaf10657c490f065adb8bb713ab6942b6f1e215c3b1774695e59309e7`  
		Last Modified: Fri, 18 Nov 2022 02:01:49 GMT  
		Size: 196.8 MB (196837670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
