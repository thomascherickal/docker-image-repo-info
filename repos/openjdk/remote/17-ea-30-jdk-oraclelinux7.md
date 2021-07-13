## `openjdk:17-ea-30-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:f1bdc0cf20096e38bf9b782eff9af70e7d40330550a4c05fd2c2dc20456f6093
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-30-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:997e86ea9b7109612dbf0f0cde31b9edfe772713105875b2477a0fc6b4d1ec88
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.8 MB (250823714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbd7ae8eec6d4204becd7a1c92bb53b166ab919e65534c67c31b2e3708faf068`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:20 GMT
ADD file:46efe0cb70a1c4f574c3b3e1fb9b9733930d246bb8077c4ec2160a840697e6c8 in / 
# Thu, 17 Jun 2021 16:51:21 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:18 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:08:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 17 Jun 2021 17:08:51 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:08:52 GMT
ENV LANG=en_US.UTF-8
# Mon, 12 Jul 2021 23:35:12 GMT
ENV JAVA_VERSION=17-ea+30
# Mon, 12 Jul 2021 23:35:21 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='527ba5657fb7d9814cdc22d860ab078bfa838e0d821a23a969e4cfd1ec616024'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='a346c3043a0e636d0cfe0cc722e6e974871f96d777b96f9ec64960bd4dbd0fbd'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 12 Jul 2021 23:35:22 GMT
CMD ["jshell"]
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
	-	`sha256:2f893cfce94b3eecc2980efbc6a2e307796ac3e1d2760368448bd10eaf57e6ea`  
		Last Modified: Mon, 12 Jul 2021 23:45:31 GMT  
		Size: 187.1 MB (187136291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-30-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:766bb6dc1d7e00f8827edcaf6341050a3319e51a3b78e2e08fc3903039c0cf39
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251226898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c67ef858a07d07eb4c90e7f3255b5ed70f37dc788a11b8fec57896a7241fad`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:08 GMT
ADD file:256f7e1c19fbbacd7c7650e1e9991f3617703ba349f259624d78e4393e945665 in / 
# Thu, 17 Jun 2021 16:51:08 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:10:00 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Thu, 17 Jun 2021 17:10:00 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:10:00 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Jul 2021 00:14:44 GMT
ENV JAVA_VERSION=17-ea+30
# Tue, 13 Jul 2021 00:15:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-x64_bin.tar.gz'; 			downloadSha256='527ba5657fb7d9814cdc22d860ab078bfa838e0d821a23a969e4cfd1ec616024'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/30/GPL/openjdk-17-ea+30_linux-aarch64_bin.tar.gz'; 			downloadSha256='a346c3043a0e636d0cfe0cc722e6e974871f96d777b96f9ec64960bd4dbd0fbd'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jul 2021 00:15:35 GMT
CMD ["jshell"]
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
	-	`sha256:00a293d729b43b9de3061f33f6a8bea9919cb10a600dae98748139ad3dee406b`  
		Last Modified: Tue, 13 Jul 2021 00:31:27 GMT  
		Size: 185.9 MB (185948611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
