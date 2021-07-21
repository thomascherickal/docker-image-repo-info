## `openjdk:8u302-oraclelinux7`

```console
$ docker pull openjdk@sha256:2fd4dd57079b2cae6354f5fc3b21e97202101ea69a4f2e91f9782fb34b0ab3e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:8u302-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:ea1134bf3af0682a1b2af774a2a2194766a18821d93f29ca9eeab1a09fd03dc7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169570268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:258a1ae5cdd5b07b7bebcaea9dcc307fc4339baf656c68072d1e1ee4aa73c113`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:20 GMT
ADD file:46efe0cb70a1c4f574c3b3e1fb9b9733930d246bb8077c4ec2160a840697e6c8 in / 
# Thu, 17 Jun 2021 16:51:21 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:18 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:10:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 17 Jun 2021 17:10:39 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:10:39 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Jul 2021 18:25:22 GMT
ENV JAVA_VERSION=8u302
# Wed, 21 Jul 2021 18:25:30 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:7627bfb99533146fcb8374f557bc24c36505fb2ee8578ec6072a821200247bbb`  
		Last Modified: Thu, 17 Jun 2021 16:52:21 GMT  
		Size: 48.3 MB (48260810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb70fb8946cabfaff2f43cee5915a69ad662b0294e9c91d8f545898e92ed32fd`  
		Last Modified: Thu, 17 Jun 2021 17:14:39 GMT  
		Size: 15.4 MB (15426613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bff95fcf1b492e8d97ef8a4a64a0271efed1f8895d99aada17e9ee9b0788ab0`  
		Last Modified: Wed, 21 Jul 2021 18:36:13 GMT  
		Size: 105.9 MB (105882845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:8u302-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:eaaacc1c1c9bd9e61423d68e67d2ee60f22a922b4d2b915135dfc0908ee76f81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170171629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8baf1df5246077eba706c0816a56a1e95312c33ca60f79cecf2bbf5c721664c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:08 GMT
ADD file:256f7e1c19fbbacd7c7650e1e9991f3617703ba349f259624d78e4393e945665 in / 
# Thu, 17 Jun 2021 16:51:08 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:14:40 GMT
ENV JAVA_HOME=/usr/java/openjdk-8
# Thu, 17 Jun 2021 17:14:40 GMT
ENV PATH=/usr/java/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:14:40 GMT
ENV LANG=en_US.UTF-8
# Wed, 21 Jul 2021 18:48:14 GMT
ENV JAVA_VERSION=8u302
# Wed, 21 Jul 2021 18:48:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_x64_linux_8u302b08.tar.gz'; 			;; 		'aarch64') 			downloadUrl='https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jdk_aarch64_linux_8u302b08.tar.gz'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	curl -fL -o openjdk.tgz.asc "$downloadUrl.sign"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys EAC843EBD3EFDB98CC772FADA5CD6035332FA671; 	gpg --batch --keyserver keyserver.ubuntu.com --keyserver-options no-self-sigs-only --recv-keys CA5F11C6CE22644D42C6AC4492EF8D39DC13168F; 	gpg --batch --list-sigs --keyid-format 0xLONG CA5F11C6CE22644D42C6AC4492EF8D39DC13168F 		| tee /dev/stderr 		| grep '0xA5CD6035332FA671' 		| grep 'Andrew Haley'; 	gpg --batch --verify openjdk.tgz.asc openjdk.tgz; 	rm -rf "$GNUPGHOME"; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/jre/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/jre/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		javac -version; 	java -version
```

-	Layers:
	-	`sha256:9a3d615f016c21e1c5fef521352cdd990a61abfd09a26d7124c61e33b2cab56a`  
		Last Modified: Thu, 17 Jun 2021 16:52:10 GMT  
		Size: 48.9 MB (48858581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a33d75d2c35cdf1c0dc42b99124399c0375b12141be4bddb4b819732453cb`  
		Last Modified: Thu, 17 Jun 2021 17:23:33 GMT  
		Size: 16.4 MB (16419706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bced07073d54db4d80007256975b77ec723733a6f8550a51ad84f284cf6597b`  
		Last Modified: Wed, 21 Jul 2021 19:04:17 GMT  
		Size: 104.9 MB (104893342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
