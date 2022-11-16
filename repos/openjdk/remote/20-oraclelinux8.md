## `openjdk:20-oraclelinux8`

```console
$ docker pull openjdk@sha256:8d711fb1c94c316fe2ed331b2f370985a7fcdfde67a32bb6b766053e62498bee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:fbc236537740f45cec0bd72ebf171405cb8d5f88b54017a3f3fe2f22be5e0367
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254342780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00d41df710b82323a3498f6e4590ae05cef0ed69c78638060a7b4697bf71c8de`
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
# Wed, 16 Nov 2022 08:45:49 GMT
ENV JAVA_VERSION=20-ea+23
# Wed, 16 Nov 2022 08:45:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Nov 2022 08:46:00 GMT
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
	-	`sha256:171c8dec6733021208709938172acfc73f9c7c581cbedd13710b619f74088fc3`  
		Last Modified: Wed, 16 Nov 2022 08:49:25 GMT  
		Size: 198.2 MB (198231526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:922e5b024cc01a3c124a36228f4de6ab5be1a26d6c406352410a2f89cd27482b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.6 MB (252633592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f024986d3bba7bec85884a5b1abbfecb38667452062cd2a81416cda18c08026`
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
# Wed, 16 Nov 2022 01:36:22 GMT
ENV JAVA_VERSION=20-ea+23
# Wed, 16 Nov 2022 01:36:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-x64_bin.tar.gz'; 			downloadSha256='0344aa24310a388514ddbc4a0279a9e28f222ae783ac918860ef8f13cfebabbe'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/23/GPL/openjdk-20-ea+23_linux-aarch64_bin.tar.gz'; 			downloadSha256='57ae94d8d6968fc4b6603eab15361e998664b7bb1707611dfa4ab9542c17fd24'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 16 Nov 2022 01:36:33 GMT
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
	-	`sha256:31f551cf49dc2015795aba7a1c73e7beba682f8e7ce6e979af580ecb2007ba89`  
		Last Modified: Wed, 16 Nov 2022 01:39:50 GMT  
		Size: 196.8 MB (196792527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
