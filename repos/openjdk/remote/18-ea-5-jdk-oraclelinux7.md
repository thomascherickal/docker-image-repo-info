## `openjdk:18-ea-5-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:90e633dc2f5a72790d1d0db6be5900e636e7113f1084200761e6a6b9c59b1de9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-5-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:f708ae4d771ac56f7f1e1a89f434e9b76379406e3ade22b520317824ab19fdc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.6 MB (251556076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:496198dca8d00245cdf29e36ec9243c152c33c69d139d04e9d3a906a47bfe9c9`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:20 GMT
ADD file:46efe0cb70a1c4f574c3b3e1fb9b9733930d246bb8077c4ec2160a840697e6c8 in / 
# Thu, 17 Jun 2021 16:51:21 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:18 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:08:19 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 17 Jun 2021 17:08:19 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:08:19 GMT
ENV LANG=en_US.UTF-8
# Mon, 12 Jul 2021 23:33:21 GMT
ENV JAVA_VERSION=18-ea+5
# Mon, 12 Jul 2021 23:33:32 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='a50d2f7309f987ee33cfdfdfbd22c18ea8e6dc8a3bb21b582cd67fb97c906a82'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='28e3b50e98e75ae64d200ddcf87ba0664229e0659ccba3cd8ee2e25cbe6de24f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 12 Jul 2021 23:33:33 GMT
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
	-	`sha256:384807ac8abbdfe36b3b8a0b7ab4788c4402943336f18367a11fbc880b28f680`  
		Last Modified: Mon, 12 Jul 2021 23:42:37 GMT  
		Size: 187.9 MB (187868653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-5-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:74a63c13794d9f326e250e42c0e3fed5743ea73f6db9538eaf630f5f875aea3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251851217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15dda915f3a724a1054183450d0cee37c59ac359e57b3860142d1133bd6af80e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 16:51:08 GMT
ADD file:256f7e1c19fbbacd7c7650e1e9991f3617703ba349f259624d78e4393e945665 in / 
# Thu, 17 Jun 2021 16:51:08 GMT
CMD ["/bin/bash"]
# Thu, 17 Jun 2021 17:08:43 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 17 Jun 2021 17:08:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 17 Jun 2021 17:08:43 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Jun 2021 17:08:43 GMT
ENV LANG=en_US.UTF-8
# Tue, 13 Jul 2021 00:13:09 GMT
ENV JAVA_VERSION=18-ea+5
# Tue, 13 Jul 2021 00:13:25 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-x64_bin.tar.gz'; 			downloadSha256='a50d2f7309f987ee33cfdfdfbd22c18ea8e6dc8a3bb21b582cd67fb97c906a82'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/5/GPL/openjdk-18-ea+5_linux-aarch64_bin.tar.gz'; 			downloadSha256='28e3b50e98e75ae64d200ddcf87ba0664229e0659ccba3cd8ee2e25cbe6de24f'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 13 Jul 2021 00:13:26 GMT
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
	-	`sha256:f0b50df21d032cd7dd9966f294237799f0169ee190ec6759a46840d76fa12ca8`  
		Last Modified: Tue, 13 Jul 2021 00:27:53 GMT  
		Size: 186.6 MB (186572930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
